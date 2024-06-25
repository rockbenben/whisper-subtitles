# whisper subtitles

很多国外的纪录片、电视剧，往往缺乏合适的字幕。即使有字幕，时间轴也常常对不上，需要手动调整。为了解决这一问题，可以使用 Whisper 工具为这些视频转录字幕，并通过多种翻译接口将字幕翻译成中文。

Whisper subtitles 虽然在字幕质量上不能与专业字幕组相比，字幕缺乏校对，有时会出现遗漏或错误翻译，但对于常年观看剧的人来说，80% 的机翻水平已经足够使用。这解决了从无到有的问题，让大家可以直接看生肉视频。

转录翻译流程：

1. 参考 [Whisper 转录教程](https://newzone.top/posts/2022-11-18-whisper_ai_subtitles.html)，了解如何使用 Whisper 工具进行字幕转录。
2. 使用自制的 [字幕翻译工具](https://tools.newzone.top/subtitle-translator) 将转录的字幕翻译为中文或其他目标语言。目前，该工具支持多个免费翻译接口。如果需要进行大量翻译，可以自行开通 API 进行翻译。

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
