# Videosrt

![Alt text](https://raw.githubusercontent.com/pocketvince/videosrt/main/4-f2ef19ccf7.gif?raw=true "convert-st, convert, convert-ov")

Videosrt is a shell script that extracts subtitles from a video file (or YouTube video) and reinserts them as hard-coded, larger, yellow subtitles on a black background.

## Update
20230408: Cleaner code, now allowing the addition of subtitles in formats other than SRT, and some lines of yt-dlp code have been added to extract subtitles from YouTube videos as well. 

20230409: Added two features:

• Convert-OV: Blur the original video, and superpose at maximum height the same video reduced by 25% and include the subtitles (as on the "convert" command)

• Convert-ST: Incorporates subtitles to the video and keeping standard size and color

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

videosrt convert-ov "video.mkv" "video.mkv.srt"
Blur the original video, and superpose at maximum height the same video reduced by 25% and include the subtitles (as on the "convert" command)

videosrt convert-st "video.mkv" "video.mkv.srt"
Incorporates subtitles to the video and keeping standard size and color

videosrt extract-yt "link"
Displays the list of available subtitles for a YTvideo, choose language & extracts the subtitles into an SRT file and downloads the video in mp4
```

## Contributing

Readme generator: https://www.makeareadme.com/

Translate subtitles: https://subtitlestranslator.com/en/

## Extra info
My television does not allow to change the color, font and size of the subtitles, script created to save my back 🥴
