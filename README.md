## Let's go AIPshit microservices (OS X)

A collection of automator workflows to be installed as OS X Services (right-click menu tasks). I put these together primarily for my students and staff who are not comfortable using terminal commands, but I use the hell out of them myself.

[![IMAGE ALT TEXT HERE](http://people.oregonstate.edu/~davibria/files/1.png)](http://people.oregonstate.edu/~davibria/files/1.png)

### Installation

Simplest way is to [download zip package](https://github.com/tvc15brian/dpu-microservices/archive/master.zip) and copy the workflows to `~/Library/Services/`. You can also just double-click each workflow file and install via Service Installer.

### Other Notes

Please note that most workflows are using third-party scripts, the default path of them (for example `ffmpeg`) is `/usr/local/bin/ffmpeg`. I recommend using [Homebrew] (http://brew.sh) to install/manage all packages.

### Available Workflows
##### BagBatch 

This workflow builds upon the bagbatch.py script from [Carleton Archives] (https://github.com/CarletonArchives/BagBatch) and requires that BagIt be installed as well as Python. This workflow will ask you to locate your BagIt install the first time you use it. This workflow also requires that the assets to be bagged exist in subdirectories. If you have a lot of files then the files-into-folders workflow below should help with that. 

[![IMAGE ALT TEXT HERE](http://people.oregonstate.edu/~davibria/files/2.png)](https://youtu.be/f5mIuS3_5Fg)

##### FFV1 

The FFV1 video codec is a simple and efficient lossless intra-frame only codec. This workflow wraps an FFV1 in a Matroska wrapper. See workflow for specifc transcoding/encoding specs. This workflow results in a matroska-wrapped FFV1 file (orignalfilename.mkv) in the same directory as original file.

##### framemd5

The FFmpeg ​framemd5 format used to decode input audiovisual data to produce one checksum per frame. These formats facilitate testing functions such as verifying that an adjusted decoder maintains intended results or that an FFmpeg decoder decodes a stream to the same data as another decoder. This workflow results in a framemd5 document (orignalfilename.framemd5) in the same directory as original file.
 
##### BagIt-SHA256

BagIt is a hierarchical file packaging format designed to support disk-based storage and network transfer of arbitrary digital content. This workflow opts for the SHA256 algorithm since it's stronger against random and deliberate collisions when compared to MD5. SHA256 is more ideal for video files. This workflow depends on bagit.py living in /usr/local/bin/.

##### BagIt-Verify

BagIt is a hierarchical file packaging format designed to support disk-based storage and network transfer of arbitrary digital content. This workflow verifies bags. This workflow depends on bagit.py living in /usr/local/bin/.

##### CRC (Cyclic Redundancy Check) Testing Format

This muxer computes and prints the Adler-32 CRC of all the input audio and video frames. By default audio frames are converted to signed 16-bit raw audio and video frames to raw video before computing the CRC. This workflow results in a crc document (orignalfilename.crc) in the same directory as original file.


##### MediaInfo

MediaInfo is a free and open-source program that displays technical information about media files, as well as tag information for many audio and video files. This workflow results in a plain text file (orignalfilename_pbcore.txt) in the same directory as original file.

##### PBCore

PBCore is a metadata schema designed for sound and moving images. This workflow results in an XML file (orignalfilename_pbcore.xml) in the same directory as original file.


##### MediaTrace

MediaTrace is a technical report that expresses the binary architecture of a file, as interpreted by MediaArea’s principal software, MediaInfo. This workflow results in an XML file (orignalfilename_mediatrace.xml) in the same directory as original file.


##### FITS

The File Information Tool Set (FITS) identifies, validates and extracts technical metadata for a wide range of file formats. It acts as a wrapper, invoking and managing the output from several other open source tools. Output from these tools are converted into a common format, compared to one another and consolidated into a single XML output file. This workflow results in an XML file (orignalfilename_fits.xml) in the same directory as original file.

##### files-into-folders

This workflow moves files into appropriately named folders. 


##### SHA256

Secure cryptographic hash function. With an output hash value of 256 bits, SHA-256 requires more relative time to compute for a given number of processing cycles CPU and processing time than MD5. This workflow results in a plain text file (orignalfilename.sha256) in the same directory as original file.


##### MD5

The MD5 message-digest algorithm is a widely used cryptographic hash function producing a 128-bit (16-byte) hash value, typically expressed in text format as a 32 digit hexadecimal number. This workflow results in a plain text file (orignalfilename.md5) in the same directory as original file.


##### folders-sha256

This workflow runs a SHA-256 checksum on each object in a directory and lists those hash values in a plain text file (sha256.txt).

##### folders-md5

This workflow runs a MD5 checksum on each object in a directory and lists those hash values in a plain text file (md5.txt).


##### clamAV

This workflow runs a clamscan clamAV virus check on each object in a directory and dumps output in a plain text file (clamscan.txt).


