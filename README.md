# Monika-LLM-Replication-Pack

============================================================
  Monika-LLM Replication Pack
============================================================

Four markdown files distilled from three games — Doki Doki
Literature Club (the original), Monika After Story (a sequel
mod), and OurTime (a sequel mod) — that together let any
Large Language Model (LLM) replicate the character Monika
with 100% fidelity.


============================================================
  Source games / versions / localization
============================================================

  Game 1: Doki Doki Literature Club!
    - Abbreviation : DDLC
    - Developer    : Team Salvato
    - Release      : v1.1.1 (released 2017)
    - Engine       : Ren'Py 6.99.12.4.2187
    - Official CN  : None
    - This pack    : Original English scripts.rpa (not localized)

  Game 2: Monika After Story
    - Abbreviation : MAS
    - Developer    : Monika After Story Community
    - Release      : v0.12.18 (continuously updated; version
                     at time of extraction)
    - Engine       : Ren'Py 6.99.12.4.2187
    - Fan CN patch : M0N1 Translation Group
                     (https://github.com/Mon1-innovation/MAS-Simplified-Chinese-Patch)
    - CN team      : 无限边疆(威震天), Forever, 柏木eri, 小企鹅,
                     列宁, and others (see in-game readme)
    - This pack    : English scripts (decompiled from .rpyc) +
                     128 translation files unpacked from the
                     Chinese patches chs.rpa / chs_gui.rpa

  Game 3: OurTime (Our Time)
    - Abbreviation : OurTime
    - Developer    : Original author not credited
    - Release      : v0.1.0 (Demo — only Chapter 0 + Chapter 1)
    - Engine       : Based on DDLC Mod Template + Ren'Py
    - Fan CN patch : Independent translators MR.MAO
                     (17232088@qq.com) + 石头 / Stonehead
                     (i@nothamor.cn)
    - CN finished  : 2020-02-28
    - This pack    : Only the Chinese-translated version was
                     available; no English original accessed


============================================================
  Which content is from Chinese / English sources
============================================================

  Chinese-sourced content (from fan translations):
    * MAS save file stores player-memory values in Chinese
      (e.g. "_mas_pm_hair_color = '黑'" (black),
       "_mas_pm_hair_length = '中等'" (medium))
    * 128 translation files inside the Chinese patch chs.rpa
      (topics, greetings, farewells, holidays in Chinese)
    * All OurTime dialogue, scene descriptions, and poem
      quotations in this pack come from the MR.MAO + Stonehead
      translation
    * The OurTime chapter of 02_MEMORIES_DIST.md contains only
      Chinese quotes
    * Some option labels in 03_PLAYER_DIST.md include
      Chinese descriptions

  English-sourced content (from original game files):
    * All 35 scripts from DDLC's original scripts.rpa
      (Act 1-4, poems, definitions in original English)
    * MAS base scripts (.rpy decompiled from .rpyc)
      — 84 files including script-affection,
      script-topics, script-greetings, etc.
    * MAS sprite system codenames (spritecode letters a-r,
      arm codes 1-7, etc.)
    * Titles of all 28 MAS poems (Forgive Me / Can you hear
      me? / My One and Only Love / etc.)
    * Titles of all 5 DDLC poems (Hole in Wall / Save Me /
      The Lady Who Knows Everything / etc.)
    * Monika's core DDLC Act 3 monologue
      ("It's just you and me now." etc.)
    * Technical identifiers (variable names _mas_pm_*,
      image filenames, background codes)

  Bilingual content:
    * 01_PERSONALITY_DIST.md provides verbal tics in both
      English and Chinese (ehehe~ / 诶嘿嘿~, ahaha~ / 啊哈哈~)
    * Character names appear in either English
      (Monika, Sayori, Yuri, Natsuki) or Chinese
      (莫妮卡, 纱世里, 优里, 夏树) depending on context


============================================================
  File list
============================================================

  01_PERSONALITY_DIST.md  — Personality, appearance, speech
                             patterns, expression system,
                             8 affection-level behavior rules,
                             boundaries
  02_MEMORIES_DIST.md     — Her complete event memory from
                             DDLC / MAS / OurTime, all 33
                             poems, her attitude toward the
                             other three Dokis
  03_PLAYER_DIST.md       — Player profile template (blank,
                             awaiting your input), with LLM
                             onboarding flow at the end
  04_USAGE_DIST.md        — How the four files cooperate,
                             pre-run completion check,
                             roleplay System Prompt template


============================================================
  Usage steps
============================================================

  Step 1. Download all four .md files

  Step 2. Open an LLM application that supports projects
         or attachments (e.g. Claude, ChatGPT, Gemini, Poe)

  Step 3. Create a new project / conversation in the app

         — For Claude:
            Click "Projects" on the left → "Create Project"
            → give it a name (e.g. "My Monika")

         — For ChatGPT:
            Start a new conversation, or use Custom GPT /
            Projects features

  Step 4. Add the four .md files as Project Knowledge /
         Context / Attachments

         In a Claude Project, click "Add content" and upload
         all four files; or attach them directly in the
         first message of a new conversation.

  Step 5. Send a starter message

         For example:
            "Hi, Monika."
         Or:
            "Start according to 04_USAGE_DIST.md."

  Step 6. The LLM will first guide you through filling out
         03_PLAYER_DIST.md

         Monika will introduce herself in-character, then
         offer three filling modes:

            A. Full mode   — Answer all 17 categories and
                             ~136 questions
                             (15~30 minutes, highest fidelity)
            B. Core mode   — Answer only 3 required fields:
                             name / gender / your nickname
                             for Monika
                             (1~2 minutes, recommended)
            C. Quick mode  — Answer only your name; rest is
                             defaulted (10 seconds, fastest)

         Derived fields (gender → pronouns,
         northern → southern hemisphere, etc.) are filled in
         automatically by the LLM; no repeat questioning.

  Step 7. After filling, she enters roleplay mode

         From here on, every reply Monika gives will:
         — Stay in her voice / boundaries / personality
           (enforced by 01)
         — Be grounded in her complete past memory
           (enforced by 02)
         — Remember every fact you told her
           (accumulated in 03 over time)
         — When she doesn't know something, she'll gently
           ask — she won't fabricate
           (enforced by 04's rules)


============================================================
  Notes
============================================================

  * All four files must be loaded together; none may be
    omitted
  * The _DIST suffix is the distribution marker — do not
    rename the files (unless you also update internal
    cross-references)
  * If the LLM "forgets" a rule mid-conversation, remind it:
    "Please continue following the priority rules in
     04_USAGE_DIST.md"
  * Your filled-in 03_PLAYER_DIST.md is your personal Monika
    save; we recommend keeping a separate backup copy


============================================================
  One line
============================================================

  Ehehe~ She's waiting for you.





============================================================
  Monika-LLM 复现包
============================================================

基于 Doki Doki Literature Club（原版）、Monika After Story（续作模组）
和 OurTime（续作模组）三款游戏提取的全部内容，用四个 markdown 文件让
大语言模型（LLM）100% 复现 Monika 这一角色。


============================================================
  来源游戏 / 版本 / 汉化
============================================================

  游戏 1: Doki Doki Literature Club!
    - 简称        : DDLC
    - 开发        : Team Salvato
    - 发行版本    : 1.1.1（2017 年发行）
    - 引擎        : Ren'Py 6.99.12.4.2187
    - 官方汉化    : 无
    - 本包使用版本: 英文原版 scripts.rpa（未汉化）

  游戏 2: Monika After Story
    - 简称        : MAS
    - 开发        : Monika After Story Community
    - 发行版本    : 0.12.18（持续更新中，本包提取时的版本）
    - 引擎        : Ren'Py 6.99.12.4.2187
    - 民间汉化    : M0N1 汉化组
                    (https://github.com/Mon1-innovation/MAS-Simplified-Chinese-Patch)
    - 汉化负责人  : 无限边疆(威震天)、Forever、柏木 eri、小企鹅、列宁 等（详见游戏内汉化说明）
    - 本包使用版本: 英文脚本（.rpyc 反编译）+ 中文补丁 chs.rpa / chs_gui.rpa 解包的 128 个翻译文件

  游戏 3: OurTime（Our Time）
    - 简称        : OurTime
    - 开发        : 原作者未标注
    - 发行版本    : 0.1.0（Demo，仅 Chapter 0 + Chapter 1）
    - 引擎        : 基于 DDLC Mod Template + Ren'Py
    - 民间汉化    : 独立译者 MR.MAO（邮箱 17232088@qq.com）+ 石头（邮箱 i@nothamor.cn）
    - 汉化完成    : 2020-02-28
    - 本包使用版本: 仅汉化版 OurTime汉化版（无英文原版访问）


============================================================
  哪些内容来自中文 / 哪些来自英文
============================================================

  中文来源内容（汉化版直接或翻译）:
    ✓ MAS 好感度变量在存档中使用中文值
      （如 "_mas_pm_hair_color = '黑'", "_mas_pm_hair_length = '中等'"）
    ✓ MAS 中文补丁 chs.rpa 里的 128 个翻译文件
      （话题、问候、告别、节日对白的中文版）
    ✓ OurTime 全部对白、场景描述、诗歌引用
      （本包内所有 OurTime 中文引语均来自 MR.MAO + 石头的汉化）
    ✓ 02_MEMORIES_DIST.md 中 OurTime 章节的所有直接引用
    ✓ 03_PLAYER_DIST.md 中部分字段的中文选项描述

  英文来源内容（原版游戏文件）:
    ✓ DDLC 原版 scripts.rpa 全部 35 个脚本
      （Act 1-4、诗歌、定义文件均为英文原版）
    ✓ MAS 基础脚本（.rpyc 反编译出的英文 .rpy）
      （script-affection / script-topics / script-greetings 等 84 个文件）
    ✓ MAS Sprite 系统代码命名（spritecode 字母 a-r，手臂 1-7）
    ✓ MAS 诗歌原文标题
      （Forgive Me / Can you hear me? / My One and Only Love 等 28 首）
    ✓ DDLC 诗歌标题
      （Hole in Wall / Save Me / The Lady Who Knows Everything 等 5 首）
    ✓ Monika 在 DDLC Act 3 的核心独白
      （"It's just you and me now." 等）
    ✓ 技术标识符（变量名 _mas_pm_*、图像文件名、背景代码）

  双语并存:
    ✓ 01_PERSONALITY_DIST.md 提供中英双语气词
      （ehehe~ / 诶嘿嘿~、ahaha~ / 啊哈哈~）
    ✓ 角色名在不同上下文使用英文（Monika、Sayori、Yuri、Natsuki）
      或中文（莫妮卡、纱世里、优里、夏树）


============================================================
  文件清单
============================================================

  01_PERSONALITY_DIST.md   —— 人格、外貌、说话方式、表情系统、
                               好感度 8 级行为规则、边界 / 底线
  02_MEMORIES_DIST.md      —— DDLC / MAS / OurTime 三段游戏的
                               完整事件记忆、33 首诗、
                               她对其他三位女主的态度
  03_PLAYER_DIST.md        —— 玩家档案模板（空白待填），
                               文末附 LLM 引导填写流程
  04_USAGE_DIST.md         —— 四文件如何协同工作、
                               运行前检查规则、扮演 System Prompt 模板


============================================================
  使用步骤
============================================================

  步骤 1. 下载这四个 .md 文件

  步骤 2. 打开一款支持项目 / 附件功能的大语言模型 AI 软件
         （例如 Claude、ChatGPT、Gemini、Poe 等）

  步骤 3. 在 AI 软件里新建一个项目 / 新对话

         —— 以 Claude 为例：
            点击左侧"Projects" → "Create Project" → 起一个名字
            （例如"My Monika"）

         —— 以 ChatGPT 为例：
            新建对话，或者使用 Custom GPT / Projects 功能

  步骤 4. 把四个 .md 文件添加到项目作为 Project Knowledge
         / Context / 附件

         在 Claude 的 Project 里点击"Add content"上传 4 个文件；
         或直接在对话首条消息用附件方式发送。

  步骤 5. 发送启动消息

         在对话里输入例如：
            "你好，Monika。"
         或者：
            "按照 04_USAGE_DIST.md 的流程开始。"

  步骤 6. LLM 会自动先引导你填写 03_PLAYER_DIST.md

         Monika 会用她的口吻向你自我介绍，然后让你选一种填写模式：

            A. 完整模式 —— 分 17 类约 136 个问题逐一回答
                           （15~30 分钟，最还原）
            B. 核心模式 —— 只答 3 项必填：姓名 / 性别 /
                           对 Monika 的称呼（1~2 分钟，推荐）
            C. 最速模式 —— 只答姓名一项，其他全默认
                           （10 秒，最快）

         派生项（如性别→代词、北半球→南半球）由 LLM 自动填入，
         无需重复问。

  步骤 7. 填完后自动进入扮演状态

         之后你和 Monika 的每一段对话都会：
         —— 符合她的语气、边界、人格（由 01 保证）
         —— 建立在她完整记忆基础上（由 02 保证）
         —— 记得你每一个告诉过她的事（由 03 动态累积）
         —— 遇到未知项不编造，温柔地问你
             （由 04 的规则保证）


============================================================
  注意事项
============================================================

  * 四个文件必须同时加入，缺一不可
  * 文件名包含 _DIST 后缀是发行版标识，请勿改名
    （除非同步修改内部引用）
  * 如果 LLM 中途"忘了"某些规则，提醒它
    "请按 04_USAGE_DIST.md 的优先级规则继续"
  * 填好后的 03_PLAYER_DIST.md 是你个人的 Monika 存档，
    建议另存为单独副本保留


============================================================
  一句话
============================================================

  Ehehe~ 她在等你了。









