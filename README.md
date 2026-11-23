# Pet Chat Stickers · 猫狗聊天贴纸

用自家猫狗照片或虚构主角，做一套聊天里常用的贴纸。默认六张，逐张交付透明 PNG；可以只做一张，也可以点名要预览。本项目不设付费解锁或登录；图片生成能力由使用的客户端提供。

## 开始使用

[下载 v0.1.0 完整包](https://github.com/coder999o/pet-chat-stickers/releases/download/v0.1.0/pet-chat-stickers-v0.1.zip)。请下载这个附件，不要选 GitHub 自动生成的 Source code；首版 Skill 和示例图在附件里。

解压后打开 `pet-chat-stickers-release/`。在 Codex 中，把里面的 `skills/pet-chat-stickers/` 整个文件夹复制到项目的 `.agents/skills/` 下，最终文件路径应为 `.agents/skills/pet-chat-stickers/SKILL.md`。其他支持 `SKILL.md` 的客户端请按各自的技能目录放置。如客户端支持手动调用，可在消息中写 `$pet-chat-stickers`。技能本身是一套工作流程，不绑定 API 或额外依赖。实际生成图片需要客户端已有的图片能力；没有该能力时，会给可复用的分镜提示词，不会把提示词当作做好的贴纸。

例如：

> $pet-chat-stickers 用这张狗狗照片做四张：收到、马上到、谢谢、晚安。保留狗狗自己左耳黑、右耳白，直接给独立透明 PNG，不用预览。

> $pet-chat-stickers 做一套虚构橘猫贴纸，用中文短句，先只给我看预览。

工作流程默认以 512 × 512 为目标，可按目标平台调整；下载包里的示例保留原始尺寸。技能不会把照片上传到无关平台或公共图床。

灵感来自 [Vane GPT Image Skills](https://github.com/VaneAi888/vane-gpt-image-skills) 的示例与教程组织方式。此包为独立编写，不包含 Vane 的代码、图像或模板。

## 看效果：原照 → 贴纸

输入照片均为虚构宠物的 AI 示意图，不是真实用户照片。各贴纸都是单独的透明 PNG，可分别下载。这里展示两组各两张的自定义短句；默认六张流程并未在第二个客户端上验证。

- 奶牛猫：黑下巴、白鼻口。示例短句：收到、不想上班。
- 三色柯基：左耳折尖（照片右侧）、窄白鼻线。示例短句：好耶、在吗。

参考图、成品 PNG 和复现记录都在完整包里，分别位于 `examples/` 和 `docs/demo.md`。
