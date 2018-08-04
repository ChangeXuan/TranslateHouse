# 原文来自[keijiro/FFmpegOut](https://github.com/keijiro/FFmpegOut)

![gif](http://i.imgur.com/bkQlFxX.gif)

**FFmpegOut**是一个用于记录和导出视频的Unity插件，并使用[FFmpeg]视频编码器来对Unity的视频进行加载。
FFmpegOut的主要作用是在Unity对视频进行预渲染是可以有效的减少渲染的时间。
与导出原图像相比，它大大的减少了文件的I/O数量，
所以当带宽遇到较大的瓶颈时，FFmpegOut是一种有效的解决办法。
另一方面，FFmpegOut在时时捕捉图像上并没有做到最优,
因此，不太推荐把FFmpegOut使用在交互式的应用上。

[FFmpeg]: https://ffmpeg.org/
