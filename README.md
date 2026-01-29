# POC 详情统计

> **当前项目 POC 更新时间：**`2026-01-29 04:26`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 70201 | cve | 52765 | medium | 32694 |
| 2 | wordpress | 64365 | other | 38900 | info | 25514 |
| 3 | wp-plugin | 59809 | sql | 3196 | low | 23219 |
| 4 | medium | 24851 | wordpress | 2459 | high | 19281 |
| 5 | low | 21589 | auth | 2089 | critical | 11355 |
| 6 | tech | 18280 | detect | 1328 | unknown | 127 |
| 7 | detect | 17559 | microsoft | 1029 | meduim | 4 |
| 8 | production | 16247 | default | 1015 | hight | 3 |
| 9 | service | 13830 | remote_code_execution | 1010 | none | 1 |
| 10 | candidate | 10901 | api | 998 | ciritical | 1 |

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

