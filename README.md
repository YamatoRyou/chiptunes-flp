# 关于本项目
## 红白机风格 Chiptune FL Studio 工程  
* 本项目用于存放自 2012 年起个人使用 FL Studio 11.1 制作的 Chiptune 音乐 (Famicom 风格, 模拟任天堂 Famicom 2A03 APU 音色及历史上发行的游戏卡中用于增强音频的扩展芯片的音色).  
* 这些作品均非原创, 每个作品对应的工程文件均已尽最大努力搜集原作者信息, 但仍有少数作品原作者信息暂缺. 如有可靠的发现请在 Issues 中提交.  
* 访客可随意下载本项目中的工程文件用于学习 FL Studio. 由于项目的特殊性, 且为确保唯一, 请勿以任何方式复制或克隆本项目.  
* 工程为 zip 格式文件, 打开方式及 FL Studio 版本要求见工程列表顶部.  
* ![avatar](https://licensebuttons.net/l/by-nc-nd/4.0/88x31.png)  

## 试听与下载  
* 工程试听:  
豆瓣小站 (首选更新): https://site.douban.com/YamatoRyou/  
哔哩哔哩 (走带演示, 不定期更新): https://space.bilibili.com/359841  
* 工程列表; 原作者信息及下载: https://yamatoryou.github.io/chiptunes-flp/list.html  
原地址 http://fuckcjmarketing.com/FL/chiptunes_flp/list.html 中的网页已于 2019 年 5 月 10 日下线.  

## 导出指南  
* 导出时务必选中 "禁止最大复音数 (Disable maximum polyphony)".  
* 对于无法裁剪采样末尾的工程 (如 Freeze-Dried (Famicom Version)), 循环模式请务必更换为 "剪切多余 (Cut remainder)".  
* 导出时重采样选择 6 点 Hermite, 既能保证音质足够, 也可以缩短导出耗时.  

## 其它  
* 工程列表使用了 Layui, 项目主页: https://www.layui.com  
* 2A03 预置 for FL Studio 帮助文档现已迁移到 GitHub, 项目主页: https://yamatoryou.github.io/2a03presetsforflstudio/help/2a03presetsforflstudio.html, 预置组套将择期上传.  
* 工程数字签名 (相关信息仅在 Windows 下可见):  
证书序列号: 7c 41 92 ad 50 8c 6d b5 4d 13 74 3d 00 bf 54 cc  
证书指纹: c0 1f 2e 77 c1 3d 39 f4 2b 76 77 80 96 30 78 a1 f9 aa be 63  
对应上述唯一信息的证书于 2020 年 10 月 3 日过期.

# 工程解读  
## 歌曲风格的倾向  
* 接近原曲  
* 接近 Famicom 风格  
* 试验目的, 用于测试音色  
* 单纯的自我取悦  

## 所有工程使用以下 FL Studio 内置插件  
* Sytrus (模拟 2A03 芯片中的 12.5% 矩形波 / 25% 矩形波 / 50% 方波 / 75% 矩形波 / 三角波 / Short Cycle 类型噪波 / Namco 163 / 任天堂 FDS (RP2C33))  
由于 Konami VRC6 芯片中的波形可以被 N163 包括, 因此后续工程几乎不再模拟此芯片.  
由于 SUN5B (FME7) 芯片中的波形可以被 2A03 或 N163 包括, 因此后续工程几乎不再模拟此芯片.  
* Fruity DX10 (模拟 Konami VRC7 芯片 FM)  
* FPC / DirectWave (加载 DPCM 采样, 有时会随工程需要将采样变调或定义循环区域)  
* Patcher (除 Sytrus 外, Patcher 将以下插件置入以模拟 Long Cycle 类型噪波)  
Effector (模拟 2A03 芯片中的噪波, Long Cycle 类型)  
Fruity WaveShaper (二值化并最大化 Long Cycle 类型噪波)  
Fruity Envolope Controller (重映射 Long Cycle 类型噪波的音符力度)  
* Fruity Parametric EQ 2 (去除不需要的低频部分, 仅限部分工程使用)  
* Fruity Compressor (最大化整首歌曲的响度)  
* Wave Candy (监视声谱图, 不影响歌曲的最终效果)  

## 播放列表布局  
* 除 "旧模式" 文件夹中的工程, 其余工程一律遵循与 FamiTracker 相似的视图.  
* "新模式 3" 文件夹中的工程已将参数事件独立到 1 个样式以便重复利用.

## 模拟多台机器同时播放  
* 相当一部分工程不满足于只使用 1 台 Famicom 的通道配置 (即 1 颗 2A03 芯片 + 若干扩展芯片), 因此这些工程会在播放列表中出现多条 DPCM 通道甚至重复出现扩展芯片等模拟多路工作的行为.  

## 音符音高; 力度等属性滑行  
* 在 FL Studio 中无法完美模拟不精确的滑行路径, 这似乎取决于工程 BPM 及 PPQ 设置.  
* "新模式 3" 中的部分工程已开始使用参数事件 + MML 模拟方式模拟不精确的滑行路径.  

## 效果的使用  
* 由于部分插件会破坏原始波形, 因此遵循 "拒绝现代混音审美" 原则. 只有一小部分工程额外使用混响及延迟效果, 效果源位于 Sytrus FX 模块.

## PPQ  
* 即 "每刻钟脉冲数". 可以理解为每拍的 "水平分辨率", 默认为 96. 在本项目中用于劣化音高滑行曲线.  
* 通过 WinHex 修改工程文件 0x0c 处的字节可获取 FL 工程设置中 PPQ 列表没有的值. 通常为 8 (0x08); 16 (0x11); 32 (0x20); 64 (0x40)  
* 警告: 通过上述方法修改 PPQ 乐谱不会随 BPM 自动拉伸, 且有可能导致 FL Studio 崩溃并使未保存的工程丢失.  

# 工程文件更新  
## 规则  
* 每个 zip 文件均为相互独立的工程 (包括衍生版本¹), 上传的工程文件会替换已上传的同路径 / 文件名的文件.  
* 旧版本将被永久删除, 不会保留, 也不会进入其它分支. 衍生版本¹除外.  
¹ 诸如 2A03 BGM - Super Cyborg Area 1 (兼容版本) 与 2A03 BGM - Super Cyborg Steam Edition - Area 1 (兼容版本)

## 历史  
* 2019 / 06 / 09  
更新 Transglobal (Famicom Version)  
版本标识: 04 (最后修改于 2019 / 06 / 11)  
试听地址: https://site.douban.com/YamatoRyou/room/1072933/?s=745710  

* 2019 / 06 / 09  
上传 / 创建 Transglobal (Famicom Version)  
版本标识: 03 (最后修改于 2019 / 06 / 09)  
试听地址: 无效  

* 2019 / 04 / 28:  
更新 Pond Scunk (Famicom Version)  
版本标识: 06 (最后修改于 2019 / 04 / 27)  
试听地址: https://site.douban.com/YamatoRyou/room/1072933/?s=744008  

* 2019 / 04 / 25:  
更新 Pond Scunk (Famicom Version)  
版本标识: 05 (最后修改于 2019 / 04 / 23)  
试听地址: 无效  

  更新 Deadline (Famicom Version)  
  版本标识: 04 (最后修改于 2019 / 04 / 25)  
  试听地址: https://site.douban.com/YamatoRyou/room/1072933/?s=744007  

  更新 Tale of the Cave (Famicom Version)  
  版本标识: 0C (最后修改于 2019 / 04 / 25)  
  试听地址: https://site.douban.com/YamatoRyou/room/1072933/?s=744009  

* 2019 / 04 / 22:  
上传 / 创建 Pond Scunk (Famicom Version)  
版本标识: 04 (最后修改于 2019 / 04 / 21)  
试听地址: 无效  

* 2019 / 04 / 20:  
上传 / 创建 Pond Scunk (Famicom Version)  
版本标识: 03 (最后修改于 2019 / 04 / 20)  
试听地址: 无效  

* 2019 / 04 / 15:  
上传 / 创建 Deadline (Famicom Version)  
版本标识: 03 (最后修改于 2019 / 04 / 15)  
试听地址: 无效  

* 2019 / 03 / 30  
更新 Rule the World (Famicom Version)  
版本标识: 09 (最后修改于 2019 / 03 / 30)  
试听地址: https://site.douban.com/YamatoRyou/room/1072933/?s=742914   

* 2019 / 03 / 22  
更新 Rule the World (Famicom Version)  
版本标识: 08 (最后修改于 2019 / 03 / 21)  
试听地址: 无效   

* 2019 / 03 / 21  
更新 Rule the World (Famicom Version)  
版本标识: 07 (最后修改于 2019 / 03 / 20)  
试听地址: 无效  

  更新 Lunar Flight (Famicom Version)  
  版本标识: 04 (最后修改于 2019 / 03 / 20)  
  试听地址: https://site.douban.com/YamatoRyou/room/1072933/?s=741103  

  更新 Crystal Ice Caves (Famicom Version)  
  版本标识: 03 (最后修改于 2019 / 03 / 20)  
  试听地址: https://site.douban.com/YamatoRyou/room/1072933/?s=722106  

* 2019 / 03 / 19:  
更新 Rule the World (Famicom Version)  
版本标识: 06 (最后修改于 2019 / 03 / 19)  
试听地址: 无效  

* 2019 / 03 / 18:  
更新 Rule the World (Famicom Version)  
版本标识: 05 (最后修改于 2019 / 03 / 18)  
试听地址: 无效  

* 2019 / 03 / 17:  
上传 / 创建 Rule the World (Famicom Version)  
版本标识: 04 (最后修改于 2019 / 03 / 17)  
试听地址: 无效  

* 2019 / 03 / 01:  
项目迁移完毕.  
