# POC 详情统计

> **当前项目 POC 更新时间：**`2025-12-26 03:51`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 68911 | cve | 52449 | medium | 32475 |
| 2 | wordpress | 63246 | other | 38207 | info | 25497 |
| 3 | wp-plugin | 58890 | sql | 3105 | low | 22726 |
| 4 | medium | 24681 | wordpress | 2351 | high | 18923 |
| 5 | low | 21111 | auth | 2070 | critical | 11116 |
| 6 | tech | 18271 | detect | 1320 | unknown | 127 |
| 7 | detect | 17558 | default | 1011 | meduim | 4 |
| 8 | production | 16146 | remote_code_execution | 1010 | hight | 3 |
| 9 | service | 13830 | microsoft | 1008 | none | 1 |
| 10 | candidate | 9928 | api | 996 | ciritical | 1 |

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

