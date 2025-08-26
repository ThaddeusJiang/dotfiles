# 保存聊天记录

将当前聊天记录完整保存到 `_devlog/chats/` 目录。

## 保存规则

- **目录名**: 使用当前工作目录名
- **文件名**: 格式为 `<YYYY-MM-DD>-核心内容.md` 你可以使用 `date` 命令
- **完整的对话内容**: user message, AI response

## 保存格式

形如：

```markdown
# 核心内容
_Saved on 2025-08-26 from <ChatApp>_

---

**$(whoami)**

/TJ/Save chat

--- Cursor Command: TJ/Save chat.md ---
内容

--- End Command ---

---

**<AI Model name>**

内容

**$(whoami)**

对话内容

**<AI Model name>**

回复

<continue>

```
