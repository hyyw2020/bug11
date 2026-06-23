# 分支保护规则配置指南

## 📋 配置目标

- ✅ 禁止除所有者外任何人直接推送到 main 分支
- ✅ 强制 PR 审查机制
- ✅ 确保代码合并前的安全检查
- ✅ 防止强制推送和分支删除

## 🔐 main 分支保护规则

### 步骤 1: 访问分支设置

1. 前往仓库页面
2. 点击 **Settings** (设置)
3. 左侧菜单选择 **Branches** (分支)
4. 点击 **Add rule** (添加规则)

### 步骤 2: 配置规则

| 设置项 | 配置值 |
|--------|--------|
| Branch name pattern | `main` |
| Require a pull request before merging | ✅ 启用 |
| Require approvals | ✅ 启用 (1个) |
| Dismiss stale pull request approvals | ✅ 启用 |
| Require review from Code Owners | ✅ 启用 |
| Require branches to be up to date | ✅ 启用 |
| Require conversation resolution | ✅ 启用 |
| Restrict who can push | ✅ 启用 |

### 步骤 3: 配置权限限制

**Restrict who can push to matching branches:**
- ✅ 启用此选项
- **允许推送的用户：** `hyyw2020`

### 步骤 4: 配置删除保护

| 设置项 | 配置值 |
|--------|--------|
| Allow force pushes | ❌ 禁止 |
| Allow deletions | ❌ 禁止 |

### 步骤 5: 完成配置

点击 **Create** (创建)

---

完成以上配置后，main 分支将得到完全保护！
