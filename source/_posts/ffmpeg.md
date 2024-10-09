---
title: 音视频下载&剪辑
cover: https://article.biliimg.com/bfs/article/4bd6124a6862d400f08986f032ff4a6564587936.jpg
---

ffmpeg&yt-dlp

<!-- more --><!-- more -->

## FFmpeg自用教程

下载链接:https://github.com/BtbN/FFmpeg-Builds/releases

### 视频格式转换

在cmd输入ffmpeg -encoders查看编码器

```cmd
ffmpeg -i input.mkv -c:v copy -c:aac output.mp4
```

**-c copy**复制音视频流

**-c:v**选择视频编码器

常用av1编码器

**h264_amf** amd的av1编码 speed:9

**libsvtav1** intel的CPU speed:2.6

**av1_qsv** intel的GPU编码器

**-c:a**选择音频编码器

**aac** 有损

**pcm_s16le** 无损

批处理转换：

新建文本文档.txt，重命名为.bat，右键编辑粘贴

```cmd
cd /d "%~dp0"
:softshare
IF "%~1"=="" GOTO :EOF
ffmpeg -i "%~1" -c:v copy -c:a pcm_s16le -y "%~dpn1_ok.mp4"
SHIFT & GOTO:softshare
```

"%\~dp0" 是批处理文件所在目录，"%\~1" 是拖入文件完整路径，包含后缀，"%~dpn1" 是拖入文件完整路径，不含后缀

### 添加字幕

<!DOCTYPE html>
<html>
<head>
    <title>调试窗口</title>
    <style>
        #myInput {
            width: 300px; /* 调整宽度为300像素 */
            height: 40px; /* 设置高度为100像素 */
            border: 3px solid #69b0ac;
            }
    </style>
</head>
<body>
    <input type="text" value="ffmpeg -i 1.mp4 -vf subtitles=1.ass output.mp4" id="myInput">
    <button onclick="copyText()" style="color: #26453d;">复制命令</button>
    <script>
        function copyText() {
            var input = document.getElementById("myInput");
            input.select();
            document.execCommand("copy");}
            // alert("已复制内容: " + input.value);
        }
    </script>
</body>
</html>

**软字幕（悬挂在视频上方，可选择加载）**

{% copy ffmpeg -i 1.mp4 -i 1.ass -c:s mov_text -c:v copy -c:a copy output.mp4 %}

**硬字幕（与视频融为一体，不可拆分）**

**用cpu合成**

> ffmpeg -i 1.mp4 -vf subtitles=1.ass output.mp4

注意，按默认配置大概率会损失画质，请查看视频码率后按高于原视频的码率进行编解码（-b:v 6000k ）

> ffmpeg -i 1.mp4 -vf subtitles=1.ass -b:v 6000k output.mp4

**用AMD显卡合成**

> ffmpeg -i 1.mp4 -vf subtitles=1.ass -c:v h264_amf output.mp4
>
> ffmpeg -i 1.mp4 -vf subtitles=1.ass -c:v h264_amf -b:v 6000k output.mp4

**用NVIDIA显卡合成**

>ffmpeg -hwaccel cuda -c:v h264_cuvid -i 1.mp4 -vf subtitles=1.ass  -c:v h264_nvenc  output.mp4

字体样式设置

> subtitles=input.srt:force_style='Fontsize=10'


### 合并文件

考虑到合并文件一般不多，所以通过文件重命名来进行合成，也方便排序

```cmd
#合并多个文件
file '1.mp4'
file '2.mp4'
file '3.mp4'
#ffmpeg -f concat -i input.txt -c copy output.mp4
```
### [字体](/font)
我做了一个大部分免费商业字体汇总的页面
但为了实时预览，牺牲了大量负载,会加载很久（优化中）
[点击跳转](/font)

### 使用yt-dlp下载视频

下载链接:https://github.com/yt-dlp/yt-dlp/releases

常用，支持youtube，bilibili(需关闭浏览器以获取cookie)

```cmd
yt-dlp -f ba+bv --merge-output-format mp4 --cookies-from edge 视频链接
```

其中的--cookies-from edge其实也可以修改为--cookies-from chrome(但chrome新版在使用时外部无法获取cookie,需要关闭浏览器,取决于你在哪个浏览器登陆了账号)

保存并嵌入字幕

```cmd
 --sub-langs all --embed-subs --embed-thumbnail
```

b站:

```cmd
 --sub-langs zh-CN --embed-subs --embed-thumbnail
```

可以这样添加到用户词典方便调用

![自定义短语](https://images.weserv.nl/?url=https://article.biliimg.com/bfs/article/c8cb22b79773fa888cf8b338c46bbc162fcffa1c.png)

