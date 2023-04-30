# whisper subtitles

使用 whisper 为小众的生肉视频转录字幕，并使用 Google Translate API 翻译字幕，能够让我观看那些没有字幕的经典 80、90 年代日剧。

虽然 whisper subtitles 的字幕质量与字幕组的质量不能完全相比，字幕缺少校对，有时会被遗漏或错翻，但对于常年看日剧的观众来说，80% 的机翻水平已经足够使用。这解决了从无到有的问题。

主要针对以下视频进行转录：

- 没有字幕的视频，特别是 80、90 年代的经典日剧。
- 视频有字幕，但字幕时间轴对不上，需要手动调节。

转录翻译流程：

1. 参考 [whisper 转录教程](https://newzone.top/posts/2022-11-18-whisper_ai_subtitles.html)。
2. 使用[字幕翻译](https://tools.newzone.top/subtitle-translator)工具。如果没有 Google Translate API，可使用转录教程中的网页翻译方法。

<a href="https://discord.gg/PZTQfJ4GjX">
   <img src="https://img.shields.io/discord/1048780149899939881?color=%2385c8c8&label=Discord&logo=discord&style=for-the-badge" alt="chat on Discord">
</a>

文档目录结构如下：

```bash
TV
|── NAME(YEAR)                   # 电视剧名称（年份）
│   ├── Season&Episode           # 电视剧名称-季+集数，比如 S01E01
│   └── ja                       # 转录的源语言字幕，ja 为日语
└── NAME(YEAR)                   # 电视剧名称（年份）
    ├── SEASON 01                # 第一季。两季以上才会单独建文件夹。
    │     ├── Season&Episode     # 电视剧名称-季+集数，比如 S01E01
    │     └── ja                 # 转录的源语言字幕，ja 为日语
    └── SEASON 0X                # 第X季
```
