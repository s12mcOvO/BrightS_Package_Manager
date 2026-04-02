# BrightS Package Manager (BSPM)

[English](#english) | [中文](#中文)

---

## English

The package manager for BrightS operating system.

### Installation

Copy `bin/bspm` to `/bin/pkg/bspm`:

```bash
cp bin/bspm /bin/pkg/
chmod +x /bin/pkg/bspm
```

### Usage

```bash
bspm [COMMAND] [OPTIONS] [PACKAGE]
```

### Commands

| Command | Alias | Description |
|---------|-------|-------------|
| `install` | `i` | Install a package |
| `remove` | `rm`, `uninstall` | Uninstall a package |
| `update` | `u` | Update package lists |
| `upgrade` | `ug` | Upgrade all packages |
| `search` | `s` | Search for packages |
| `list` | `ls` | List installed packages |
| `info` | `show` | Show package information |
| `clean` | - | Clean cache |
| `version` | `v` | Show version |
| `help` | `h` | Show help |

### Examples

```bash
# Install a package
bspm install firefox

# List installed packages
bspm list

# Search for packages
bspm search editor

# Show package information
bspm info firefox

# Remove a package
bspm remove firefox
```

### Directory Structure

```
/bin/pkg/
├── bspm          # Package manager script
├── .db/          # Package database
│   ├── firefox.info
│   └── ...
└── firefox/      # Installed package
    └── ...
```

### License

This project is licensed under the [GNU General Public License v3.0](LICENSE).

---

## 中文

BrightS 操作系统的包管理器。

### 安装

将 `bin/bspm` 复制到 `/bin/pkg/bspm`：

```bash
cp bin/bspm /bin/pkg/
chmod +x /bin/pkg/bspm
```

### 使用方法

```bash
bspm [命令] [选项] [包名]
```

### 命令

| 命令 | 别名 | 说明 |
|------|------|------|
| `install` | `i` | 安装包 |
| `remove` | `rm`, `uninstall` | 卸载包 |
| `update` | `u` | 更新包列表 |
| `upgrade` | `ug` | 升级所有包 |
| `search` | `s` | 搜索包 |
| `list` | `ls` | 列出已安装包 |
| `info` | `show` | 显示包信息 |
| `clean` | - | 清理缓存 |
| `version` | `v` | 显示版本 |
| `help` | `h` | 显示帮助 |

### 示例

```bash
# 安装包
bspm install firefox

# 列出已安装包
bspm list

# 搜索包
bspm search editor

# 显示包信息
bspm info firefox

# 卸载包
bspm remove firefox
```

### 目录结构

```
/bin/pkg/
├── bspm          # 包管理器脚本
├── .db/          # 包数据库
│   ├── firefox.info
│   └── ...
└── firefox/      # 已安装的包
    └── ...
```

### 许可证

本项目基于 [GNU 通用公共许可证 v3.0](LICENSE) 开源。
