# POC 详情统计

> **当前项目 POC 更新时间：**`2026-07-04 05:51`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 107998 | cve | 58700 | medium | 44312 |
| 2 | wordpress | 101370 | other | 56687 | low | 38221 |
| 3 | wp-plugin | 93398 | sql | 11155 | high | 28398 |
| 4 | low | 35983 | wordpress | 7855 | info | 27224 |
| 5 | medium | 35357 | auth | 4597 | critical | 16577 |
| 6 | candidate | 34436 | remote_code_execution | 1959 | unknown | 137 |
| 7 | tech | 17939 | detect | 1861 | informative | 19 |
| 8 | high | 17177 | web | 1460 | meduim | 19 |
| 9 | detect | 17154 | microsoft | 1432 | hight | 15 |
| 10 | production | 15799 | api | 1129 | cretical | 4 |

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

