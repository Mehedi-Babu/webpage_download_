# Download Web Pages for Offline Viewing
Download an entire website or save selected pages and view them offline.

**Table of Contents**  
1. [Requirements](#requirements)
    1. [Linux](#linux)
    2. [Windows](#windows)
    3. [Android](#android)
2. [Download Web Page](#download-web-page)
    1. [Wget Options](#wget-options)
3. [View Content Offline](#view-content-offline)
    1. [GUI](#gui)
    2. [Serve Files Locally](#serve-files-locally)

## Requirements
Wget and Python are used in this tutorial.

### Linux
Both Wget and Python are already installed.

### Windows
1. [Wget for Windows](https://eternallybored.org/misc/wget/)
2. [Python](https://www.python.org/downloads/)

### Android
1. Termux
2. pkg install wget
3. pkg install python

## Download Web Page
Retrieve file located at specified web address.
```shell
wget -p -k <URL>
```
### Wget Options

| Switch | Description |
|:-------|:------------|
| -r     | Download pages recursively up to a maximum of 5 levels deep |
| -l     | Set the number of levels you wish to go |
| -k     | Convert all links on the pages downloaded to point to local file paths |
| -m     | Get a complete mirror of a website |
| -b     | Run in the background, even when you are not logged on |

## View Content Offline

### GUI
Navigate to directory and open  the `index.html` file in your web browser.

### Serve Files Locally
It's best to serve files from the location of the downloaded content as to not share unwanted content.

**Navigate to the downloaded content directory**  
```shell
cd /directory/for/files/
```

**Start server**  
```shell
python -m http.server <PORT>
```

**Navigate to server IP address**  
Open your browser and enter in the device's IP address along with the port number you specified.

If you are using Linux you can locate your IP address with
```shell
ifconfig
```

If you are using Windows you can locate your IP address with
```shell
ipconfig
```
