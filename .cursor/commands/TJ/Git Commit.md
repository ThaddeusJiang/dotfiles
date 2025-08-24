# Git Commit Message 生成器

生成符合规范的 commit message，遵循 Conventional Commits 标准。

## 格式规范

```
<type>(<scope>): <description>

[optional body]

[optional footer(s)]
```

## 主要类型

- **feat**: 新功能
- **fix**: 修复 bug
- **docs**: 文档更新
- **style**: 代码格式调整
- **refactor**: 代码重构
- **test**: 测试相关
- **chore**: 构建过程或辅助工具的变动

## 示例

```
feat: 添加用户登录功能
fix(auth): 修复登录验证失败问题
docs: 更新 API 文档
refactor(utils): 重构日期处理函数
chore: 更新依赖包版本
```

## 生成原则

- **简洁明了**: 用一行描述核心变更
- **技术导向**: 突出技术细节和影响范围
- **问题定位**: 便于快速定位和回溯问题
- **符合规范**: 遵循项目约定的格式

## 自动执行

选择 message 后，自动执行：
```bash
git add . && git commit -m "生成的 message"
```
