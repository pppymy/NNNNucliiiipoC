# POC 详情统计

> **当前项目 POC 更新时间：**`2026-03-14 04:19`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 76502 | cve | 46234 | medium | 34232 |
| 2 | wordpress | 70721 | other | 42192 | low | 25585 |
| 3 | wp-plugin | 65464 | sql | 4993 | info | 25161 |
| 4 | medium | 26815 | wordpress | 4720 | high | 19905 |
| 5 | low | 24177 | auth | 3848 | critical | 12029 |
| 6 | production | 21313 | remote_code_execution | 2873 | unknown | 96 |
| 7 | tech | 18269 | detect | 1677 | hight | 16 |
| 8 | detect | 17523 | microsoft | 1290 | informative | 9 |
| 9 | service | 13824 | social | 906 | meduim | 8 |
| 10 | candidate | 12062 | exposed | 844 | cretical | 2 |

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

