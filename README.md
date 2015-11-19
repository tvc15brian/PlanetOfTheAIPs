## [@pixels_per_inch](https://twitter.com/pixels_per_inch)'s digital production microservices (OS X)

A collection of automator workflows to be installed as OS X Services (right-click menu tasks). I use these to speed up my digital produciton/presevation processes. 

### Installation

Simplest way is to [download zip package](https://github.com/tvc15brian/dpu-microservices/archive/master.zip) and copy the workflows to `~/Library/Services/`. You can also just double-click each workflow file and install via Service Installer.

### Other Notes

Please note that most workflows are using third-party scripts, the default path of them (for example `ffmpeg`) is `/usr/local/bin/ffmpeg`. (Installed by [Homebrew](http://brew.sh/)). I recommend using Homebrew to install/manage all packages.

### Available Workflows
#####FFV1 Video Codec 

The FFV1 video codec is a simple and efficient lossless intra-frame only codec. This workflow wraps an ffv1 in a Matroska wrapper. See workflow for specifc transcoding/encoding specs. This workflow results in a matroska-wrapped ffv1 file (orignalfilename.mkv) in the same directory as original file.


#####framemd5

The FFmpeg ​framemd5 format used to decode input audiovisual data to produce one checksum per frame. These formats facilitate testing functions such as verifying that an adjusted decoder maintains intended results or that an FFmpeg decoder decodes a stream to the same data as another decoder. This workflow results in a framemd5 document (orignalfilename.framemd5) in the same directory as original file.


#####CRC (Cyclic Redundancy Check) Testing Format

This muxer computes and prints the Adler-32 CRC of all the input audio and video frames. By default audio frames are converted to signed 16-bit raw audio and video frames to raw video before computing the CRC. This workflow results in a crc document (orignalfilename.crc) in the same directory as original file.


#####MediaInfo

MediaInfo is a free and open-source program that displays technical information about media files, as well as tag information for many audio and video files. This workflow results in a plain text file (orignalfilename.txt) in the same directory as original file.


#####MediaTrace

MediaTrace is a technical report that expresses the binary architecture of a file, as interpreted by MediaArea’s principal software, MediaInfo. This workflow results in an xml file (orignalfilename.xml) in the same directory as original file.


#####FITS

The File Information Tool Set (FITS) identifies, validates and extracts technical metadata for a wide range of file formats. It acts as a wrapper, invoking and managing the output from several other open source tools. Output from these tools are converted into a common format, compared to one another and consolidated into a single XML output file. This workflow results in an xml file (orignalfilename.xml) in the same directory as original file.


#####SHA256

Secure cryptographic hash function. With an output hash value of 256 bits, SHA-256 requires more relative time to compute for a given number of processing cycles CPU and processing time than MD5. This workflow results in a plain text file (orignalfilename_sha256.txt) in the same directory as original file.


#####MD5

The MD5 message-digest algorithm is a widely used cryptographic hash function producing a 128-bit (16-byte) hash value, typically expressed in text format as a 32 digit hexadecimal number. This workflow results in a plain text file (orignalfilename_md5.txt) in the same directory as original file.

