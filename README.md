# Videosrt

![Alt text](https://raw.githubusercontent.com/pocketvince/videosrt/main/19h25m11s016.png?raw=true "todo")
![Alt text](https://raw.githubusercontent.com/pocketvince/videosrt/main/19h27m33s978.png?raw=true "done")

Small shell script to export and re-import subtitles and paste them into the video

## Installation
Install ffmpeg 
```shell
git clone https://git.ffmpeg.org/ffmpeg.git ffmpeg
```
or

```shell
apt-get install ffmpeg
```
Download the script and place it in /bin/videosrt

## Usage

```shell
root@pocketvince:~# videosrt
Videosrt
--------

cmd: videosrt info "video.mkv"
result: Stream #0:2(eng) Subtitle: subrip

cmd: videosrt extract "video.mkv" "0:2"
result: Creation of video.mkv.srt

cmd: videosrt convert "video.mkv"
result: Generate file with yellow subtile
```

## Contributing

Readme generator: https://www.makeareadme.com/
Translate subtitles: https://subtitlestranslator.com/en/

## Extra info
My television does not allow to change the color, font and size of the subtitles, script created to save my back 🥴
