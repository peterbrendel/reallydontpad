# reallydontpad

A tool for Dontpad users in Python + requests + bs4

**Warning**: This app isn't a Dontpad official software.

--- 

## About

This solution aims to keep all data you upload to dontpad safe from editing and deleting.
This is guaranteed with three steps:

* Downloading the page content
* String matching
* Re-upload original content if matching fails

Even tho the tool removes any updates from original content, it does allow adding new content, which means that any user can freely add new lines.

The only way for you to update the page is by editing the file 'original.txt' from your server.

## Instalation

Install `requests` and `bs4` library

```bash
pip3 install requests bs4
```

## Interface usage

This program is a server. You can set everything up the first time you boot it. It will ask for:

- nickname
- URL for your dontpad file

### Command line usage:

Commands:

- -h, --help                Show this help message and exit
- -f FILE, --file FILE      File path (original.txt is default)
- -o, --output              Print actual text in dontpad address
