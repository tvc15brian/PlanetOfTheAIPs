# @pixels_per_inch's digital production microservices (OS X)

A collection of automator workflows to be installed as OS X Services (right-click menu tasks). I use these to speed up my digital produciton/presevation processes. 

## Installation

Paste the following code at a Terminal prompt:

```shell
bash <(curl -fsSL https://raw.github.com/tvc15brian/dpu-microservices/go/install)
```

The script explains what it will do and then pauses before it does it. If you don’t trust it, [download zip package](https://github.com/tvc15brian/dpu-microservices/archive/master.zip) and manually copy the workflows to `~/Library/Services/`.

## Other Notes

Please note that most workflows are using third-party scripts, the default path of them (for example `ffmpeg`) is `/usr/local/bin/ffmpeg`. (Installed by [Homebrew](http://brew.sh/)).

## Available Workflows

- [cyclic redundancy check](#coming)
- [ffv1](#coming)
- [framemd5](#coming)
- [m4v(640x480)](#coming)
- [md5_txt](#coming)
- [mediainfo_txt](#coming)
- [mediatrace_xml](#coming)
- [sha256_txt](#coming)
- [FITS](#coming)