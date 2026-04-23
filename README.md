# POC 详情统计

> **当前项目 POC 更新时间：**`2026-04-23 05:16`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 76193 | cve | 47105 | medium | 33894 |
| 2 | wordpress | 70042 | other | 40890 | low | 25735 |
| 3 | wp-plugin | 64887 | sql | 6764 | info | 25222 |
| 4 | medium | 26297 | wordpress | 4720 | high | 19956 |
| 5 | low | 24281 | remote_code_execution | 2506 | critical | 12085 |
| 6 | production | 19431 | auth | 2102 | unknown | 106 |
| 7 | tech | 18233 | microsoft | 1762 | meduim | 4 |
| 8 | detect | 17556 | detect | 1674 | informative | 3 |
| 9 | service | 13826 | web | 980 | hight | 2 |
| 10 | candidate | 13338 | api | 875 | __cve_severity__ | 1 |

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

