# Videosrt

![Alt text](https://raw.githubusercontent.com/pocketvince/videosrt/main/19h25m11s016.png?raw=true "todo")
![Alt text](https://raw.githubusercontent.com/pocketvince/videosrt/main/19h27m33s978.png?raw=true "done")

videosrt is a shell script that extracts subtitles from a video file (or YouTube video) and reinserts them as hard-coded, larger, yellow subtitles on a black background.

## Update
20230408: Cleaner code, now allowing the addition of subtitles in formats other than SRT, and some lines of yt-dlp code have been added to extract subtitles from YouTube videos as well. 

## Installation
Install ffmpeg & yt-dlp
```shell
apt-get install ffmpeg yt-dlp -y
```
Download the script and place it in /bin/videosrt

## Usage

```shell
root@pocketvince:~# videosrt
videosrt info "video.mkv"
Displays information about the subtitles of the specified video

videosrt extract "video.mkv" "0:0"
Extracts subtitles from the specified video and saves them to an SRT file

videosrt convert "video.mkv" "video.mkv.srt"
Incorporates subtitles from an SRT file into a video in large, yellow and with a black background

videosrt extract-yt "link"
Displays the list of available subtitles for a YTvideo, choose language & extracts the subtitles into an SRT file and downloads the video in mp4

## Contributing

Readme generator: https://www.makeareadme.com/

Translate subtitles: https://subtitlestranslator.com/en/

## Extra info
My television does not allow to change the color, font and size of the subtitles, script created to save my back 🥴
