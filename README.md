# POC 详情统计

> **当前项目 POC 更新时间：**`2026-08-18 02:51`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 108728 | cve | 58410 | medium | 43918 |
| 2 | wordpress | 102069 | other | 56669 | low | 38743 |
| 3 | wp-plugin | 93982 | sql | 10240 | high | 28616 |
| 4 | low | 36510 | wordpress | 5687 | info | 26451 |
| 5 | candidate | 36324 | remote_code_execution | 4346 | critical | 16527 |
| 6 | medium | 35183 | auth | 4325 | unknown | 133 |
| 7 | high | 17637 | detect | 1869 | informative | 16 |
| 8 | tech | 17176 | web | 1532 | hight | 15 |
| 9 | detect | 16486 | microsoft | 1307 | meduim | 9 |
| 10 | production | 14663 | api | 1111 | cretical | 4 |

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

