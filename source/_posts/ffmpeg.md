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

"%~dp0" 是批处理文件所在目录，"%~1" 是拖入文件完整路径，包含后缀，"%~dpn1" 是拖入文件完整路径，不含后缀

### 合并文件

考虑到合并文件一般不多，所以通过文件重命名来进行合成，也方便排序

```cmd
#合并多个文件
file '1.mp4'
file '2.mp4'
file '3.mp4'
#ffmpeg -f concat -i input.txt -c copy output.mp4
```



### 使用yt-dlp下载视频

下载链接:https://github.com/yt-dlp/yt-dlp/releases

常用，支持youtube，bilibili(需关闭浏览器以获取cookie)

```cmd
yt-dlp -f ba+bv --merge-output-format mp4 --cookies-from chrome 视频链接
```

保存并嵌入字幕

```cmd
--sub-langs all --embed-subs --embed-thumbnail
```

b站:

```cmd
 --sub-langs zh-CN --embed-subs --embed-thumbnail
```

可以这样添加到用户词典方便调用

![image-20230705214226252](https://article.biliimg.com/bfs/article/c8cb22b79773fa888cf8b338c46bbc162fcffa1c.png)

