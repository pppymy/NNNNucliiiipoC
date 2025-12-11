# POC 详情统计

> **当前项目 POC 更新时间：**`2025-12-11 03:56`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 68082 | cve | 52287 | medium | 32367 |
| 2 | wordpress | 62542 | other | 37700 | info | 25490 |
| 3 | wp-plugin | 58342 | sql | 3060 | low | 22420 |
| 4 | medium | 24603 | wordpress | 2285 | high | 18701 |
| 5 | low | 20807 | auth | 2060 | critical | 10914 |
| 6 | tech | 18268 | detect | 1317 | unknown | 127 |
| 7 | detect | 17557 | default | 1012 | meduim | 4 |
| 8 | production | 16123 | remote_code_execution | 1009 | hight | 3 |
| 9 | service | 13829 | microsoft | 997 | none | 1 |
| 10 | high | 9574 | api | 994 | ciritical | 1 |

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

