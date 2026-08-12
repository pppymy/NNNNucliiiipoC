# POC 详情统计

> **当前项目 POC 更新时间：**`2026-08-12 04:06`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 108373 | cve | 58289 | medium | 43894 |
| 2 | wordpress | 101714 | other | 56539 | low | 38580 |
| 3 | wp-plugin | 93644 | sql | 10211 | high | 28494 |
| 4 | low | 36347 | wordpress | 5653 | info | 26440 |
| 5 | candidate | 35965 | remote_code_execution | 4318 | critical | 16472 |
| 6 | medium | 35154 | auth | 4309 | unknown | 133 |
| 7 | high | 17525 | detect | 1871 | informative | 16 |
| 8 | tech | 17163 | web | 1532 | hight | 15 |
| 9 | detect | 16475 | microsoft | 1299 | meduim | 9 |
| 10 | production | 14663 | api | 1108 | cretical | 4 |

**81 个目录，44572 个文件**

### 克隆项目

克隆这个项目到本地：

```bash
git clone https://github.com/lianqingsec/NucleiPocGather.git
```

进入项目目录：

```bash
cd NucleiPocGather
```

### 配置

在 `repo.txt` 文件中配置监控 GitHub 项目信息。

### 运行脚本

运行 Python 脚本：

```bash
python NucleiPocGather.py
```

### GitHub Action

在 GitHub 仓库中设置 Action，以便每日自动运行脚本。

> 需要配置`Workflow permissions`为`Read and write`权限

## 文件结构

- `NucleiPocGather.py`: 收集全网 Nuclei POC 的脚本文件。
- `DeWeight.py`: 对现有的 Nuclei POC 进行进一步去重的脚本文件。
- `WirteREADME.py`: 统计现有的 POC 并更新 README.md 文件。
- `repo.txt`: Nuclei POC 仓库列表。
- `poc.txt`: 已存档 POC 列表。
- `poc/`: 存放分类后的 Nuclei POC 文件夹。

