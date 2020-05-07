# Download Web Pages for Offline Viewing

## Requirements

### Linux
Both Wget and Python are installed and ready for use.

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

## View Web Page

Navigate to directory and open  the `index.html` file in your web browser.

Serve files
```shell
python -m http.server <PORT>
```
