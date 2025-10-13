# POC 详情统计

> **当前项目 POC 更新时间：**`2025-10-13 03:24`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 44031 | cve | 37296 | info | 25250 |
| 2 | wordpress | 38777 | other | 31389 | medium | 24474 |
| 3 | wp-plugin | 35879 | wordpress | 1836 | high | 15205 |
| 4 | tech | 18248 | auth | 1823 | low | 11453 |
| 5 | detect | 17535 | sql | 1741 | critical | 8589 |
| 6 | medium | 16766 | detect | 1256 | unknown | 127 |
| 7 | service | 13824 | default | 962 | meduim | 4 |
| 8 | low | 9890 | remote_code_execution | 951 | hight | 3 |
| 9 | high | 6556 | api | 897 | none | 1 |
| 10 | http | 4566 | microsoft | 814 | ciritical | 1 |

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

