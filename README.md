# POC 详情统计

> **当前项目 POC 更新时间：**`2025-10-06 03:16`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 43855 | cve | 37045 | medium | 24313 |
| 2 | wordpress | 38714 | other | 29183 | info | 22870 |
| 3 | wp-plugin | 35824 | wordpress | 1836 | high | 15082 |
| 4 | medium | 16705 | auth | 1762 | low | 11465 |
| 5 | tech | 16010 | sql | 1746 | critical | 8516 |
| 6 | detect | 15209 | detect | 1248 | unknown | 126 |
| 7 | service | 11696 | default | 956 | meduim | 4 |
| 8 | low | 9914 | remote_code_execution | 947 | hight | 3 |
| 9 | high | 6552 | api | 868 | none | 1 |
| 10 | http | 4360 | microsoft | 784 | ciritical | 1 |

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

