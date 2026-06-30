# 2022_09_16_ConvertVideoForPlayer
Allow to convert with FFmpeg video in 360 to 360 downgrade to fit in Unity.

```
 public string m_ffmpegCommand4K = "FFMPEG -y -i \"INPUT\" -c:v libx264 -preset fast -crf 18 -x264-params mvrange=511 -maxrate 50M -bufsize 25M -vf \"scale=WIDTHxHEIGHT\" - pix_fmt yuv420p -c:a aac -b:a 160k -movflags faststart \"OUTPUT\"";
```
   
