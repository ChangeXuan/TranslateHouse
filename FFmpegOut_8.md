# 原文来自[keijiro/FFmpegOut](https://github.com/keijiro/FFmpegOut)

![gif](http://i.imgur.com/bkQlFxX.gif)

**FFmpegOut**是一个用于记录和导出视频的Unity插件，并使用[FFmpeg]视频编码器来对Unity的视频进行加载。

The main scope of FFmpegOut is to reduce rendering time when using Unity for
pre-rendering. It greatly reduces the amount of file I/O compared to exporting
raw image sequences, so that it can be an effective solution when the bandwidth
is the most significant bottleneck. On the other hand, FFmpegOut is not
optimized for real-time capturing. It's not strongly recommended to use it in
an interactive application.

[FFmpeg]: https://ffmpeg.org/
