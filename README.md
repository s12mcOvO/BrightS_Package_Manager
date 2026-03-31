# BrightS Package Manager (BSPM)

BrightS 操作系统的包管理器。

## 安装

将 `bin/bspm` 复制到 `/bin/pkg/bspm`：

```bash
cp bin/bspm /bin/pkg/
chmod +x /bin/pkg/bspm
```

## 使用方法

```bash
bspm [COMMAND] [OPTIONS] [PACKAGE]
```

## 命令

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

## 示例

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

## 目录结构

```
/bin/pkg/
├── bspm          # 包管理器脚本
├── .db/          # 包数据库
│   ├── firefox.info
│   └── ...
└── firefox/      # 已安装的包
    └── ...
```

## 许可证

MIT License
