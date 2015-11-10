# Brian's digital production microservices (OS X)

A collection of Automator workflows that speed up your digital produciton and digital presevation processes. 

## Installation

Paste the following code at a Terminal prompt:

```shell
bash <(curl -fsSL https://raw.github.com/tvc15brian/dpu-microservices/go/install)
```

The script explains what it will do and then pauses before it does it. If you don’t trust it, [download zip package](https://github.com/tvc15brian/dpu-microservices) and manually copy the workflows to `~/Library/Services/`.

## Other Notes

Please note that most workflows are using third-party scripts, the default path of them (for example `ffmpeg`) is `/usr/local/bin/ffmpeg`. (Installed by [Homebrew](http://brew.sh/)).

## Available Workflows

- [Create App Iconset](#create-app-iconset)
- [Create .icns](#create-icns)
- [Unpack .icns](#unpack-icns)
- [Create `favicon.ico`](#create-faviconico)
- [Create `favicon.ico` (multi-resource)](#create-faviconico-multi-resource)
- [Add `@2x` (`@3x`) Suffix](#add-2x-3x-suffix)
- [Copy & Add `@2x` (`@3x`) Suffix](#copy--add-2x-3x-suffix)
- [Create `@2x` (`@3x`) Image](#create-2x-3x-image)
- [Remove `@2x` (`@3x`) Suffix](#remove-2x-3x-suffix)
- [Convert Image Format](#convert-image-format)
- [Resize Images](#resize-images)
- [Rename Selected Files](#rename-selected-files)
- [Create DMG Image](#create-dmg-image)
- [Open with rmate](#open-with-rmate)
- [Compress Images](#compress-images)
- [Encode Selected Files Using Base64](#encode-selected-files-using-base64)
- [Convert Selected Text to Audio File](#convert-selected-text-to-audio-file)
- [Convert .ass to .srt](#convert-ass-to-srt)
