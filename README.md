# POC 详情统计

> **当前项目 POC 更新时间：**`2025-12-06 03:32`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 62272 | cve | 54082 | medium | 31077 |
| 2 | wordpress | 56758 | other | 32317 | info | 25483 |
| 3 | wp-plugin | 52919 | sql | 2045 | low | 19629 |
| 4 | medium | 23324 | wordpress | 1980 | high | 17630 |
| 5 | tech | 18266 | auth | 1908 | critical | 10254 |
| 6 | low | 18015 | detect | 1308 | unknown | 127 |
| 7 | detect | 17555 | default | 1009 | meduim | 4 |
| 8 | production | 17240 | remote_code_execution | 981 | hight | 3 |
| 9 | service | 13829 | api | 972 | none | 1 |
| 10 | high | 8518 | microsoft | 844 | ciritical | 1 |

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

