# POC 详情统计

> **当前项目 POC 更新时间：**`2026-05-21 06:20`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 77396 | other | 52154 | medium | 32738 |
| 2 | wordpress | 70971 | cve | 37430 | low | 25839 |
| 3 | wp-plugin | 65656 | sql | 5686 | info | 25216 |
| 4 | candidate | 29753 | wordpress | 4637 | high | 22006 |
| 5 | medium | 25133 | auth | 3830 | critical | 12247 |
| 6 | low | 24385 | remote_code_execution | 3085 | unknown | 105 |
| 7 | tech | 18213 | microsoft | 1962 | meduim | 4 |
| 8 | detect | 17540 | detect | 1598 | hight | 3 |
| 9 | service | 13828 | web | 1055 | informative | 1 |
| 10 | high | 12695 | api | 732 | ciritical | 1 |

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

