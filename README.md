# learning-log
Date = October 18 2026
Tools i have met = ffmpeg and qrencode

What each tool is for:
1.ffmpeg is basically a command line app to convert videos into gifs or edit media
2.qrencode just takes a web link or text and spits out a qr code image

The commands that worked:
1.For the video to gif, ffmpeg -i video.mp4 videotogif.gif
2.For the qr code, qrencode -o repo.png "github link"

What broke and what fixed it:
First I tried running qrencode without telling it the output file name and it threw an error
Fixed it by checking the documentation and realizing I needed the o option
With ffmpeg I typed a non existant filetype, Fixed it by fixing the typo in the filetype

The five steps:
1. ffmpeg :
  brew install ffmpeg
  ffmpeg -i input.file output.file #simple
  ffmpeg -t "timeinseconds" -i input.file output.file #resizing time
  ffmpeg -i input.file scale = "100x100" output.file #resizing frame
  ffmpeg -i input.mp4 -vn output.mp3 # extract audio from video
2. qrencode :
   brew install qrencode
   qrencode -o website.png "https://example.com"
   qrencode -t we.png "Hello World"

One thing I want to try next:
  how to make rainbow qr codes and create pdfs from docs
