![{481A1158-B3FC-408D-0E41-B3AE78DAA7D8}](https://user-images.githubusercontent.com/48104960/171990764-a3071ed9-bf5e-4171-81db-acbc9c0bc23e.png)  

![avatar](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-green)

# 关于本项目
## Famicom 风格 Chiptune FL Studio 工程  
* 本项目用于存放自 2012 年起个人使用 FL Studio 11.1 制作的 Chiptune 音乐 (Famicom 风格, 模拟任天堂 Famicom 2A03 APU 音色及历史上发行的游戏卡中用于增强音频的扩展芯片的音色).  
* 这些作品的编曲及旋律部分均非原创, 每个作品对应的工程文件均已尽最大努力搜集原作者信息, 但仍有少数作品原作者信息暂缺或有误. 如有可靠的发现请在 Issues 中提交.  
* 访客可随意下载本项目中的工程文件用于学习 FL Studio. 由于项目的特殊性, 且为确保唯一, **请勿以任何方式复制或克隆 (包括 Fork) 本项目**.  
* 工程为 zip 格式文件, 打开方式及 FL Studio 版本要求见工程列表顶部.  
* 本项目最早起始于 2010 年, 但早于 2012 年的作品不会在本项目中展示.  
* 本项目使用的音色预置及相关工具现已重新整理, 项目地址: https://github.com/YamatoRyou/2a03presetsforflstudio  

## The 1st or 2nd original author is here:
* To confirm whether your work is referenced by this project, please visit https://yamatoryou.github.io/chiptunes-flp/list.html, press Ctrl + F in the webpage and type your own keywords (song name; author alias or real name).  
* If you:  
a) do not want one of your works to be cited in this project;  
b) think that a project file infringes your copyright;  
c) a project file fails to mark the necessary original author information;  
Please feedback in Issues.  

## 根据知识共享协议 (Creative Commons) 规则, 仅授予访客用户以下权利:  
* 允许下载.  
* 允许保留数字签名, 作者及原作者信息; 未修改工程文件且非盈利性质目的的前提下二次传播.  
* 允许提取工程文件中使用的插件预置 (FST 文件).  

## 根据知识共享协议 (Creative Commons) 规则, 访客用户需遵守以下限制:  
* 不允许提取使用工程文件引用或嵌入的采样文件 (WAV 等); 乐谱 (MIDI / FSC); 自动控制信息 (FSC)  
* 不允许修改工程文件, 且不能将修改后的结果传播.  
* 不允许在抹去作者及原作者信息的情况下传播.  

上述限制不适用于第一; 第二原作者.  

## 工程文件违反知识共享协议 (Creative Commons) 规则的传播  
* 以下是部分示例:  
https://music.163.com/#/song?id=1465111497  
https://music.163.com/#/song?id=1467643593  
以上链接中的试听使用未经数字签名的工程文件生成, 且未按知识共享协议署名.  

## 试听与下载  
* 工程试听:  
豆瓣小站 (首选更新): https://site.douban.com/YamatoRyou/  
**豆瓣自 2022 / 04 / 27 起更新了账号政策, 未来可能不再通过豆瓣提供试听.**  
哔哩哔哩 (走带演示, 不定期更新): https://space.bilibili.com/359841  
* 工程列表; 原作者信息及下载: https://yamatoryou.github.io/chiptunes-flp/list.html  
原地址 http://fuckcjmarketing.com/FL/chiptunes_flp/list.html 中的网页已于 2019 年 5 月 10 日下线.  

## 导出指南  
* 导出时务必取消选中 "禁止最大复音数 (Disable maximum polyphony)".  
* 对于无法裁剪采样末尾的工程 (如 Freeze-Dried (Famicom Version)), 循环模式请务必更换为 "剪切多余 (Cut remainder)".  
* 导出时重采样选择 6 点 Hermite, 既能保证音质足够, 也可以缩短导出耗时.  

## 其它  
* 工程列表使用了 Layui, 项目主页: https://github.com/sentsin/layui  

## 工程数字签名 (相关信息仅在 Windows 下可见):  
* 1  
证书序列号: 7e 50 2e df 77 4a 4d ba 41 37 b5 58 86 ed 18 25  
证书指纹: 94 4b df 11 c8 f7 48 9b c6 35 09 22 74 5d b4 17 8f 29 f5 4c  
对应上述唯一信息的证书于 2020 年 10 月 3 日 起启用, 2024 年 10 月 3 日过期.  
* 2  
证书序列号: 7c 41 92 ad 50 8c 6d b5 4d 13 74 3d 00 bf 54 cc  
证书指纹: c0 1f 2e 77 c1 3d 39 f4 2b 76 77 80 96 30 78 a1 f9 aa be 63  
对应上述唯一信息的证书已于 2020 年 10 月 3 日过期.  

**本仓库公开的每个工程文件均包含数字签名.**  

# 工程文件报毒说明  
* 每个工程包括 1 个工程文件 (扩展名FLP) 与若干采样文件 (扩展名 WAV), 这些文件被打包到 1 个压缩文件 (扩展名 ZIP). 极少数早期工程还会包括 HTML 文档及一些图像素材. ZIP 文件即为工程文件.  
* 为了能让数字签名及其证书能附着到工程, 工程文件头部会被附加一个极小的 Windows 可执行文件. 工程文件尾部会被附加签名及证书数据, 最终组成类似三明治的结构.
* 一个工程文件下载到本地后, 可以直接使用 FL Studio 11 打开. 也可以先解压 (确保采样等素材与 FLP 文件必须位于同一路径), 再使用 FL Studio 打开 FLP 文件.  
* **用于附着签名的 Windows 可执行文件使用易语言编写, 这是导致工程文件被部分杀毒软件报毒的根本原因.** 现阶段没有计划解决此问题.  

# 工程解读  
## 歌曲风格的倾向  
* 接近原曲  
* 接近 Famicom 风格  
* 试验目的, 用于测试音色或移植到其它平台  
* 单纯的自我取悦  

## 工程使用以下 FL Studio 内置插件  
* Sytrus (模拟 2A03 芯片中的 12.5% 矩形波 / 25% 矩形波 / 50% 方波 / 75% 矩形波 / 三角波 / Short Cycle 类型噪波 / Namco 163 / 任天堂 FDS (RP2C33) / Konami VRC7)  
由于 Konami VRC6 芯片中的波形可以被 N163 包括, 因此后续工程几乎不再模拟此芯片.  
由于 SUN5B (FME7) 芯片中的方波 / 矩形波可以被 2A03 或 N163 包括, 因此后续工程几乎不再模拟此芯片.  
* Patcher (除 Sytrus 外, Patcher 将以下插件置入以模拟 Long Cycle 类型噪波)  
* Fruity Parametric EQ 2 (去除不需要的低频部分, 仅限部分工程使用)  
* Fruity Limiter (最大化整首歌曲的响度)  
* Wave Candy (监视声谱图, 不影响歌曲的最终效果)  

## 已放弃使用的 FL Studio 内置插件  
* FPC (采样向下变调丢失高频; 不支持循环点)  
* Effector (Bug)  
* Fruity WaveShaper (无法量化相位导致模拟波表音色效果差)  
* Fruity Envolope Controller (疑似 Bug, 内部包络触发始终晚于音符触发)  
* Fruity DX10 (自由度低, 被 Sytrus 取代)
* Fruity Compressor (已被 Fruity Limiter 取代)  

## 播放列表布局  
* 除 "旧模式" 文件夹中的工程, 其余工程一律遵循与 FamiStudio 相似的视图.  
* "新模式 3" 文件夹中的工程已将参数事件独立到 1 个样式以便重复利用.

## 模拟多台机器同时播放  
* 相当一部分工程不满足于只使用 1 台 Famicom 的通道配置 (即 1 颗 2A03 芯片 + 若干扩展芯片), 因此这些工程会在播放列表中出现多条 DPCM 通道甚至重复出现扩展芯片等模拟多路工作的行为.  

## 音符音高; 力度等属性滑行  
* 在 FL Studio 中无法完美模拟不精确的滑行路径, 这似乎取决于工程 BPM 及 PPQ 设置.  
* "新模式 3" 中的部分工程已开始使用参数事件 + MML 模拟方式模拟不精确的滑行路径.  

## 针对音频信号的后置效果使用  
* 由于部分插件会破坏原始波形, 因此遵循 "拒绝现代混音审美" 原则. 只有一小部分工程额外使用混响及延迟效果, 效果源位于 Sytrus FX 模块. 如果主控音频流低于 50 Hz 的频段影响了响度, 则会使用 Fruity Parametric EQ 2 切除.  

## 乐谱 (样式) 去重  
* 使用 HashMyFiles 对工程构架中的所有乐谱进行哈希值对比, 同一通道, 不同样式编号; 同一哈希值的乐谱视为相同. 最终按上述规则只保留 1 个乐谱.  
* 不适用于 1 个样式内包含多个乐谱或事件的情形.  

## PPQ  
* 即 "每刻钟脉冲数". 可以理解为每拍的 "水平分辨率", 默认为 96. 在本项目中用于劣化音高滑行曲线.  
* 通过 WinHex 修改工程文件 0x0c 处的字节可获取 FL 工程设置中 PPQ 列表没有的值 (硬改). 通常为 8 (0x08); 16 (0x11); 32 (0x20); 64 (0x40)  
* 警告: 通过上述方法修改 PPQ 会导致以下不良后果:  
乐谱不会随 BPM 自动拉伸;  
导出的波形文件有听觉上的异常 (在 11.1.0 上测试发现);  
包含 Effector 的工程硬改 PPQ 会导致该工程打开过程中 FL Studio 出现稳定性问题甚至崩溃 (在 11.1.0 上测试发现, 为插件 bug).  

# 工程文件更新  
## 规则  
* 每个 zip 文件均为相互独立的工程 (包括衍生版本¹), 上传的工程文件会替换已上传的同路径 / 文件名的文件.  
* 被替换的旧版本将被永久删除, 不会保留, 也不会进入其它分支. 衍生版本¹除外.  
* 会不定期对部分工程文件进行修改但不影响歌曲最终效果, 此类修改不计入版本号递增, 且不会在豆瓣小站更新试听, 但会更新数字签名及时间戳签名.  
* 自 2021 年起的工程放弃使用 8 位 16 进制递增作为版本标识, 改用 Windows 风格的版本号, 仅使用前 3 部分.  
¹ 诸如 2A03 BGM - Super Cyborg Area 1 (兼容版本) 与 2A03 BGM - Super Cyborg Steam Edition - Area 1 (兼容版本)  

## 历史  
* 详见 https://github.com/YamatoRyou/chiptunes-flp/blob/master/history.md
