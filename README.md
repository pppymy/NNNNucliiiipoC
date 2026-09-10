# POC 详情统计

> **当前项目 POC 更新时间：**`2026-09-10 06:12`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 95240 | other | 56683 | medium | 39349 |
| 2 | wordpress | 88719 | cve | 51938 | low | 33989 |
| 3 | wp-plugin | 82258 | wordpress | 6840 | high | 27406 |
| 4 | low | 31657 | sql | 4589 | info | 26932 |
| 5 | candidate | 31562 | auth | 4100 | critical | 14830 |
| 6 | medium | 30105 | detect | 2464 | unknown | 135 |
| 7 | tech | 17416 | microsoft | 2031 | meduim | 19 |
| 8 | detect | 16587 | remote_code_execution | 1581 | informative | 17 |
| 9 | high | 16029 | api | 1123 | hight | 15 |
| 10 | service | 13833 | web | 999 | cretical | 4 |

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

