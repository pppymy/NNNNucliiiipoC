# POC 详情统计

> **当前项目 POC 更新时间：**`2026-08-13 04:05`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 110933 | cve | 63385 | medium | 45482 |
| 2 | wordpress | 104392 | other | 57598 | low | 38566 |
| 3 | wp-plugin | 96006 | wordpress | 5785 | high | 29531 |
| 4 | low | 36431 | sql | 5352 | info | 28028 |
| 5 | medium | 36285 | auth | 4396 | critical | 17074 |
| 6 | candidate | 35144 | remote_code_execution | 2296 | unknown | 131 |
| 7 | tech | 18902 | detect | 1841 | hight | 15 |
| 8 | high | 18440 | web | 1495 | meduim | 11 |
| 9 | detect | 18064 | microsoft | 1345 | informative | 5 |
| 10 | production | 15900 | social | 1261 | cretical | 4 |

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

