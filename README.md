# scuesplit
Simple Cue Splitter. Split audio files via CUE sheet without re-encoding.

## Supported Audio formats
As far as I am aware, this should work with any audio formats that ffmpeg can split. I have confirmed it works with: `wav` `flac` `m4a` `mp3` `aac` `opus`

## Use
```
Usage: scuesplit.sh [-h] [-a <audio file>] [-c <cue file>] [-l <log file>]
   -a Audio file to process
   -c Cue file to use when processing the audio file (-a)
   -h Help
   -l Log ffmpeg output to <file>
```
The output will be in the following format:
```
TRACKNUM - PERFORMER - TITLE.ext
```
Example output:
```
01 - Bodyguard - HUM2ER.ext
02 - Bodyguard - E-CIG.ext
...
```
## Dependencies
`ffmpeg`

