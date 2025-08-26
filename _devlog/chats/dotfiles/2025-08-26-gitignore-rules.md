# 聊天记录 - Git 忽略规则管理

**日期**: 2025-08-26
**项目**: dotfiles
**主题**: Git 忽略规则管理

## 主要决策和更改

1. 在 `.gitignore_global` 中使用相对路径模式来忽略所有仓库中的 `.cursor/commands/` 和 `_devlog/chats/` 目录
2. 在 dotfiles 仓库中使用 `!` 前缀取消忽略这些目录

## 技术细节

- `.gitignore_global` 配置：
  ```
  .cursor/commands/
  _devlog/chats/
  ```

- dotfiles 仓库 `.gitignore` 配置：
  ```
  # macOS
  .DS_Store

  # 取消忽略被全局 gitignore 忽略的目录
  !.cursor/commands/
  !_devlog/chats/
  ```

---

*此文件由 TJ/Archive 命令自动生成*
