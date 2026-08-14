# POC 详情统计

> **当前项目 POC 更新时间：**`2026-08-14 04:08`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 104525 | cve | 59688 | medium | 43131 |
| 2 | wordpress | 97984 | other | 56210 | low | 36660 |
| 3 | wp-plugin | 90109 | wordpress | 5488 | high | 28118 |
| 4 | low | 34527 | sql | 5304 | info | 28001 |
| 5 | candidate | 34330 | auth | 4190 | critical | 16103 |
| 6 | medium | 33945 | remote_code_execution | 1932 | unknown | 131 |
| 7 | tech | 18897 | detect | 1830 | hight | 15 |
| 8 | detect | 18055 | web | 1386 | meduim | 11 |
| 9 | high | 17123 | microsoft | 1313 | informative | 5 |
| 10 | service | 13836 | default | 1178 | cretical | 4 |

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

