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

<<<<<<< Updated upstream
- [cyclic redundancy check]
CRC (Cyclic Redundancy Check) testing format.

This muxer computes and prints the Adler-32 CRC of all the input audio and video frames. By default audio frames are converted to signed 16-bit raw audio and video frames to raw video before computing the CRC.

- [ffv1 (.mkv)](#coming)
Video Codec Specification

The FFV1 video codec is a simple and efficient lossless intra-frame only codec. This workflow wraps ffv1 in a Matroska wrapper.

- [framemd5](#coming)
Per-packet MD5 testing format.

This muxer computes and prints the MD5 hash for each audio and video packet. By default audio frames are converted to signed 16-bit raw audio and video frames to raw video before computing the hash.

- [m4v(640x480)](#coming)
- [md5_txt](#coming)
- [mediainfo_txt](#coming)
- [mediatrace_xml](#coming)
=======
CRC (Cyclic Redundancy Check) Testing Format

This muxer computes and prints the Adler-32 CRC of all the input audio and video frames. By default audio frames are converted to signed 16-bit raw audio and video frames to raw video before computing the CRC.


FFV1 Video Codec 

The FFV1 video codec is a simple and efficient lossless intra-frame only codec. This workflow wraps an ffv1 in a Matroska wrapper. See workflow for specifc transcoding/encoding specs.


framemd5

The FFmpeg ​framemd5 format used to decode input audiovisual data to produce one checksum per frame. These formats facilitate testing functions such as verifying that an adjusted decoder maintains intended results or that an FFmpeg decoder decodes a stream to the same data as another decoder.


MediaInfo

MediaInfo is a free and open-source program that displays technical information about media files, as well as tag information for many audio and video files. This workflow results in a plain text file (.txt) with same filename as video file.


MediaTrace

MediaTrace is a technical report that expresses the binary architecture of a file, as interpreted by MediaArea’s principal software, MediaInfo.


FITS

The File Information Tool Set (FITS) identifies, validates and extracts technical metadata for a wide range of file formats. It acts as a wrapper, invoking and managing the output from several other open source tools. Output from these tools are converted into a common format, compared to one another and consolidated into a single XML output file. This workflow results in an xml file (.xml) with same filename as video file.


SHA256

Secure cryptographic hash function. With an output hash value of 256 bits, SHA-256 requires more relative time to compute for a given number of processing cycles CPU and processing time than MD5.

>>>>>>> Stashed changes
- [sha256_txt](#coming)
- [md5_txt](#coming)
- [m4v(640x480)](#coming)
