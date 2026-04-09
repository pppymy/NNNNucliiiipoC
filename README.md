# POC 详情统计

> **当前项目 POC 更新时间：**`2026-04-09 04:38`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 72066 | cve | 49318 | medium | 32255 |
| 2 | wordpress | 66172 | other | 41008 | info | 25022 |
| 3 | wp-plugin | 61243 | auth | 3544 | low | 23982 |
| 4 | medium | 24828 | remote_code_execution | 2795 | high | 19261 |
| 5 | low | 22605 | sql | 2163 | critical | 11647 |
| 6 | tech | 18288 | wordpress | 1946 | unknown | 99 |
| 7 | detect | 17525 | microsoft | 1620 | hight | 15 |
| 8 | production | 16075 | detect | 1410 | meduim | 14 |
| 9 | service | 13826 | sql_injection | 1135 | informative | 8 |
| 10 | candidate | 12751 | social | 723 | cretical | 2 |

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

