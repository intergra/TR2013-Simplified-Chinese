<div align="center">

# TR2013 - 简体中文翻译

### Complete Simplified Chinese Translation Mod for Tomb Raider (2013)

**完整简体中文翻译 MOD，覆盖菜单、界面、字幕、过场动画、收集品文本及中文字体资源。**

</div>

## 下载

请前往本仓库的 [Releases](https://github.com/intergra/TR2013-Simplified-Chinese/releases)
页面下载：

```text
TR2013-Simplified-Chinese.zip
```

> [!IMPORTANT]
> 请下载 Release 页面中单独提供的 `TR2013-Simplified-Chinese.zip`。GitHub 自动生成的
> `Source code (zip)` 和 `Source code (tar.gz)` 不是可安装的 MOD。

## Overview / 简介

本 MOD 为《Tomb Raider (2013) / 古墓丽影（2013）》制作完整简体中文翻译，覆盖
游戏菜单、界面、字幕、过场动画、收集品文本、系统提示以及中文字体资源。

翻译以英文原文为主要依据，官方繁体中文仅作为参考，并参照《古墓丽影：崛起》
《古墓丽影：暗影》等后续作品的官方简体用语进行统一。经过多轮迭代，核心术语已
对齐后续作品，并对剧情对白、战斗喊话和文献旁白进行了逐句打磨。

这不是简单的“繁转简”，而是结合剧情、角色语气、玩法语境和玩家阅读习惯重新整理
后的简体中文本地化版本。累计修正了数百处翻译，涵盖误译纠正、术语统一、口语化
润色、仪式台词重译和繁中口吻清理等方面。

本 MOD 同时从官方原始资源重建游戏使用的中文字体。主字体采用 Noto Sans SC / 思源
黑体简体，并以 Noto Sans KR 限定补入韩文玩家名。v7.5 除菜单、HUD、字幕和文档外，
还审计多人动态玩家名中的扩展拉丁、希腊、西里尔、日文、中文和韩文，解决旧字体把
大量字符显示成“口”或“□”的问题。

本 MOD 采用官方 `zhhant` 中文槽位资源覆盖：

- 无需修改 `.exe`
- 无需 DLL 注入
- 与游戏内“中文 / Chinese”语言选项兼容
- 安装后选择中文语言，即可显示简体中文
- 内置重建后的简体中文字体资源，菜单、字幕和长文档均可正常显示

## Important Notes / 重要说明

1. 安装后，请在游戏语言设置中选择“中文 / Chinese”。
2. 本 MOD 不会新增独立的“简体中文”语言选项，而是替换游戏原有的中文本地化资源。
3. 如果游戏语言未设置为中文，简体中文翻译不会生效。
4. 前置工具为 [TR2013 Modding Tools / Tomb Raider (2013) Mod Manager](https://www.nexusmods.com/tombraider2013/mods/112?tab=files&show_file=442)
   **1.10.0**。当前正式发布包只面向 1.10.0 构建与测试，请勿使用 1.11.0 安装本包。
5. 如果 Nexus 下载页面提示 `additional file required`，请先下载并安装该前置工具。
6. 本 MOD 不包含游戏本体，使用前必须拥有并安装正版游戏。

## Package Contents / 文件内容

压缩包内主要包含：

- 1 个主本地化文本文件：`pc-w/local/locals.bin/zhhant.json`
- 2,759 个 `.ips32` 差分补丁和 800 个必要的 `.mul` 字幕流资源
- 11 个 `.sch` 外部影片字幕文件
- 2 个 `.tr9dtp` 资源：中文字体与字幕背景 UI
- Noto Sans SC / KR 相关许可证与来源说明，共 4 个 `.txt`

本 MOD 不包含游戏本体文件、可执行程序、DLL、脚本或额外启动器。

## Main Features / 主要内容

### 1. 完整简体中文界面与菜单

覆盖 `zhhant.json` 中的全部主界面文本，共 3,389 条字符串，包括但不限于：

- 主菜单、暂停菜单和读档界面
- 新游戏、继续、章节选择、难度与辅助选项
- HUD 与系统提示
- 营地、地图、目标和互动提示
- 错误与警告信息
- 多人模式界面
- 匹配、回合、成就与相关说明
- DLC 与额外内容入口文案

界面中的按键图标、颜色标记、占位符与换行结构均已保留，尽量避免按钮说明错位或
排版异常。

营地相关术语已统一：

- `Base Camp` → “大本营”
- `Day Camp / Campsite` → “临时营地”

用语风格与系列后续作品保持一致。图像设置已统一为“画面”，武器精度术语统一为
“精度”，武器命名如“射手步枪”等均已标准化。

### 2. 游戏内对白与字幕

覆盖 `pc-w/audio/streams/vo/` 下与中文语言相关的语音流字幕。整体字幕审校快照包含
6,111 条字幕记录，发布包按安全策略拆分为差分补丁与必要的完整流资源，包括：

- 主线剧情对白
- 支线与环境对话
- 劳拉独白
- 战斗与环境喊话
- 无线电通讯
- 收集品朗读
- 历史文档和 GPS 秘宝旁白
- 多人模式相关语音字幕，如适用

字幕只替换中文语言键，不修改语音本身。中文字幕中的显示用斜体标签已清理，字幕
黑色背景调整为约 50% 不透明度，以减少遮挡并保留可读性。

### 3. 引擎内过场动画字幕

覆盖 `pc-w/cinstream/` 内由游戏引擎播放的实时过场动画字幕。部分过场存在多套中文
子流，本 MOD 对实际会被游戏读取的子流一并进行处理，避免部分 CG 仍显示繁体、缺字
或字幕不完整。

对于文本较长的过场，必要时以完整流方式发布，确保字幕完整可读；能够安全差分发布
的资源则保留轻量补丁形式。

### 4. 外部影片字幕

覆盖 `local/localization/movies/` 下 11 个 `.sch` 外部影片字幕文件。部分原始 `.sch`
文件没有中文字幕行，本 MOD 已补充对应简体中文翻译。

### 5. 技能、武器升级与教程文本

技能树、武器改造、战斗教程和操作提示均已做术语统一与语境修正。例如：

- `Second Wind` → “绝境重生”
- `Scramble` → “蹬墙攀爬”
- `Dodge Kill` → “闪避击杀”
- `Salvaging` → “搜刮”
- `Advanced Salvaging` → “高级搜刮”
- `Survival Instincts` → “生存本能”
- `Climbing Axe` → “攀爬斧”
- `Pain Tolerance` → “耐痛强化”
- `Marksman Rifle` → “射手步枪”
- `accuracy` → “精度”

教程、连杀提示、终结技说明和按键映射提示等均按实际玩法翻译，避免“地面攀爬”
“手把”等过时或不准确译法。

### 6. 文档、遗物与其他收集品

主文本完整覆盖历史文献、日记、文献标题与正文、GPS 秘宝、挑战古墓、遗物描述、
地图区域名、目标文本和章节摘要。收集品朗读内容也在 `.mul` 字幕范围内单独维护；
多篇超长文档朗读经过语义优化，必要时通过完整流资源保证整段可读、不截断。

主要人名与地名已统一：

- `Lara Croft` → “劳拉·克劳馥”
- `Samantha / Sam` → “萨曼莎 / 萨姆”
- `Roth` → “罗斯”
- `Yamatai` → “邪马台”
- `Himiko` → “卑弥呼”
- `Solarii` → “索拉瑞”

### 7. 画面、声音与操作设置

设置菜单全文简体，覆盖 `Graphics / Audio / Controls` 等分类下的选项：

- 画面设置：抗锯齿、曲面细分、纹理质量、纹理过滤、阴影、垂直同步等
- 声音设置：主音量、语音、音效、字幕开关等
- 操作设置：键鼠与手柄映射、灵敏度、反转视角、辅助功能等

图形技术缩写如 MSAA、FXAA 等在必要时保留英文缩写并附中文说明，符合 PC 玩家阅读
习惯。

### 8. 翻译原则

1. 优先遵循英文原文的真实语义。
2. 结合当前场景、角色语气与实际玩法。
3. 参考《古墓丽影：崛起》《古墓丽影：暗影》官方简体术语。
4. 使用游戏行业常见表达。
5. 官方繁体仅作参考，不机械照搬。

目标是在准确的基础上，让文本更符合《Tomb Raider (2013)》的剧情氛围、玩法逻辑
和玩家阅读习惯。

### 9. 简体中文字体支持

本 MOD 替换官方 `fontchinese.drm` 中的字形资源，主字体采用 Noto Sans SC Bold 700，
韩文动态玩家名采用 Noto Sans KR Bold 700 限定补字。每次构建都从官方原始 DTP 开始，
不在旧字体成品上继续叠加补丁。

最终字体包含 42,689 个字形；静态文本、多人固定字幕和 40,230 个多人动态码位审计
均为 0 缺字。手柄图标由游戏引擎渲染，不会被误替换成普通字形。ZIP 内附带两套字体
的 OFL 许可证与来源说明；Mod Manager 不会将这些许可证文件安装进游戏目录。

### 10. 术语统一与文本一致性

本 MOD 对人物称呼、地点名、物品名、任务目标和玩法提示进行了统一。例如：

- `Climbing Axe` → “攀爬斧”
- `Survival Instincts` → “生存本能”
- `Gondola Transport` → “运输缆车”
- `Hall of Ascension` → “登基大殿”
- `Shanty Town` → “贫民窟”
- `Stormguard General` → “风暴将军”
- `Gas Can` → “汽油桶”；气体语境使用“燃气”
- `Solarii Brotherhood` → “索拉瑞兄弟会”
- `Ritual of Flames` → “火祭仪式”
- `Ritual Chamber` → “仪式厅”

对文献、字幕和 UI 中重复出现的同一段文本，也尽量保持语义和称呼一致。

## Recommended Environment / 推荐环境

- 游戏版本：Windows Steam 版 Tomb Raider (2013)
- 前置工具：Tomb Raider (2013) Mod Manager 1.10.0
- 推荐语言设置：中文 / Chinese
- 推荐安装前状态：未安装其他中文文本、字幕或中文字体 MOD

如果此前安装过旧版汉化、测试版 MOD、其他会改动 `.tiger` 文件的 MOD，或遇到过 CG
卡死、文献无声、卸载后仍异常等情况，建议先通过 Steam 验证游戏文件完整性，再重新
安装本 MOD。

## Installation / 安装方法

1. 从 [Releases](https://github.com/intergra/TR2013-Simplified-Chinese/releases)
   下载最新版本的 `TR2013-Simplified-Chinese.zip`。
2. 打开 TR2013 Modding Tools / Tomb Raider (2013) Mod Manager 1.10.0。
3. 选择《Tomb Raider (2013)》。
4. 点击 `Install mod from archive`。
5. 选择本 MOD 的 ZIP，等待 Mod Manager 完成安装。
6. 启动游戏并进入语言设置。
7. 将游戏语言设为“中文 / Chinese”。
8. 完成后，游戏将显示简体中文。

## Updating / 更新方法

1. 关闭游戏。
2. 通过 Mod Manager 卸载已安装的旧版本。
3. 如曾安装过测试版、其他汉化或出现异常，建议先通过 Steam 验证游戏文件完整性。
4. 下载最新版本的 MOD 压缩包。
5. 按照上方安装步骤重新安装。

不建议直接覆盖游戏目录中的 MOD 文件。Mod Manager 安装后生成的 `.tiger` 文件可能
明显大于下载的 ZIP，这是正常现象：ZIP 中的 `.ips32` 是差分补丁，安装时工具会把
差分应用到原始资源并写入 MOD 归档。

## Uninstallation / 卸载方法

1. 关闭游戏。
2. 打开 Tomb Raider (2013) Mod Manager。
3. 选择《Tomb Raider (2013)》。
4. 在已安装 MOD 列表中找到本 MOD。
5. 使用 Mod Manager 卸载或移除。
6. 完成后重新启动游戏。

> [!WARNING]
> 请勿在 MOD 仍处于安装状态时手动删除游戏目录中的 `.tiger` 文件。

## Compatibility / 兼容性说明

- 适用于 Windows Steam 版《Tomb Raider (2013)》。
- 建议不要与其他修改中文文本、字幕或中文字体的 MOD 同时使用。
- 本 MOD 不修改关卡流程、角色属性、敌人 AI、武器数值或存档结构。
- 本 MOD 仅覆盖本地化文本、中文字幕资源、外部影片字幕和中文字体资源。
- 本 MOD 不包含游戏本体，使用前必须拥有并安装正版游戏。

## Technical Safety / 技术安全说明

- 不修改 `TombRaider.exe`。
- 不包含 DLL、脚本、启动器、注入工具或后台程序。
- 不替换配音内容、音乐、外部视频、事件流、关卡脚本、AI、武器数值或存档系统。
- 不发布 `ja` 相关字幕补丁，避免历史文献 VO 在部分安装状态下出现无声问题。
- 发布前检查文本标记泄漏、超槽位字幕覆盖、中文字体字符覆盖、资源路径范围和资源冲突。

## Known Notes / 已知说明

- 本 MOD 使用游戏原有中文槽位，因此游戏中仍显示为“中文 / Chinese”，不会额外出现
  “Simplified Chinese”语言选项。
- 如果安装后仍显示英文或其他语言，请先检查游戏语言设置是否为中文。
- 如果曾手动删除 `.tiger` 文件或使用过不同版本 Mod Manager，建议通过 Steam 验证
  游戏文件完整性后再安装。
- 当前正式发布包按 Mod Manager 1.10.0 制作与测试，不提供 1.11.0 适配包。
- 本 MOD 不建议与其他中文字体、中文文本或字幕类 MOD 同时安装，因为它们可能覆盖
  同一批资源。
- 压缩包体积和安装后的 MOD 归档体积不一定一致，这是 Mod Manager 应用差分补丁后的
  正常结果。

## Troubleshooting / 故障排查

### 安装后没有显示简体中文

- 确认使用的是本页面 Release 中的正式 ZIP，而不是 GitHub 自动生成的 Source code。
- 确认 Mod Manager 版本为 1.10.0。
- 确认游戏语言已经设置为“中文 / Chinese”。
- 确认没有同时启用其他修改中文文本、字幕或字体的 MOD。

### 安装、CG 或返回主菜单异常

- 先通过 Mod Manager 正常卸载相关 MOD，不要手动删除仍在使用的 `.tiger` 文件。
- 通过 Steam 验证游戏文件完整性。
- 使用 Mod Manager 1.10.0，在干净状态下重新安装 v7.5 正式 ZIP。
- 若仍能稳定复现，请反馈游戏平台、MOD 版本、ZIP SHA-256、Mod Manager 版本、其他
  已安装 MOD，以及完整错误信息或截图。

## Credits / 制作信息

**制作人：** NoWindNoMoon / 此情无关风月

**简体中文字形：** Noto Sans SC / Source Han Sans SC

**韩文玩家名补字：** Noto Sans KR

字体衍生内容依据 SIL Open Font License 1.1 使用。完整字体版权声明和许可证位于正式
ZIP 根目录，仓库说明见 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)。

游戏名称、原始文本、资源格式和其他游戏资产归各自权利人所有。本 MOD 是非官方、
非商业的玩家制作项目，与游戏开发商、发行商及相关权利人没有隶属或认可关系。使用
本 MOD 必须拥有通过合法渠道取得的游戏副本。

本仓库没有使用 MIT、GPL 等许可证对全部内容统一再授权，详情见
[LICENSE.md](LICENSE.md)。

## Feedback / 反馈与说明

本 MOD 已完成全量翻译和多轮精细打磨，技术测试通过，但仍可能存在遗漏或兼容性问题。
如果在游玩过程中发现以下问题，欢迎通过
[GitHub Issues](https://github.com/intergra/TR2013-Simplified-Chinese/issues) 反馈：

- 繁体或英文残留
- 字幕缺失、错位或显示时间异常
- 文本溢出或换行不自然
- 字符显示异常
- 翻译不符合剧情或玩法语境
- 安装、更新或卸载异常

反馈时请尽量提供出现位置、当前任务或场景、角色、截图、MOD 版本、ZIP SHA-256、
Mod Manager 版本和其他已安装 MOD。

感谢每一位测试和反馈问题的玩家。
