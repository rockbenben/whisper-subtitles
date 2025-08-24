# whisper subtitles

很多国外的纪录片、电视剧，往往缺乏合适的字幕。即使有，也常常存在时间轴不同步、翻译不准确等问题。为了解决这一痛点，我们可以借助 OpenAI 的开源语音识别工具 **Whisper**，快速为视频生成字幕，并结合多种翻译接口实现母语化。

与专业字幕组的人工翻译相比，Whisper 自动生成的字幕在准确度和流畅度上仍有差距，偶尔会出现遗漏或误译。但对于习惯观看原声的观众而言，自动字幕已经能提供约八成的可理解度，足以满足“从无到有”的需求。换句话说，它解决了从零开始的问题，让观众无需等待字幕组资源就能直接观看“生肉”视频。

转录翻译流程：

1. 参考 [Whisper 转录教程](https://newzone.top/posts/2022-11-18-whisper_ai_subtitles.html)，了解如何使用 Whisper 工具进行字幕转录。
2. 使用开源字幕翻译工具 [Subtitle Translator](https://tools.newzone.top/zh/subtitle-translator) 将转录的字幕翻译为中文或其他目标语言。目前，该工具支持多个免费翻译接口。如果需要进行大量翻译，可以自行开通 API。

文档目录结构如下：

```bash
类型                             # 电视剧/纪录片
|── NAME(YEAR)                   # 电视剧名称（年份）
│   ├── Season&Episode           # 电视剧名称-季+集数，比如 S01E01
│   └── ja                       # 转录的源语言字幕，ja 为日语
└── NAME(YEAR)                   # 电视剧名称（年份）
    ├── S01                      # 第一季。两季以上才会单独建文件夹。
    │     ├── Season&Episode     # 电视剧名称-季+集数，比如 S01E01
    │     └── ja                 # 转录的源语言字幕，ja 为日语
    └── S0X                      # 第X季
```

<a href="https://discord.gg/PZTQfJ4GjX">
   <img src="https://img.shields.io/discord/1048780149899939881?color=%2385c8c8&label=Discord&logo=discord&style=for-the-badge" alt="chat on Discord" />
</a>
