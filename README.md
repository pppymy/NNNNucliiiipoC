# POC 详情统计

> **当前项目 POC 更新时间：**`2026-06-14 06:40`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 42487 | cve | 34571 | medium | 22939 |
| 2 | wordpress | 37551 | other | 27545 | info | 19851 |
| 3 | wp-plugin | 34858 | auth | 1867 | high | 14002 |
| 4 | medium | 16352 | wordpress | 1396 | low | 10889 |
| 1 | cve | 104714 | cve | 57023 | medium | 43186 |
| 2 | wordpress | 98228 | other | 55956 | low | 36915 |
| 3 | wp-plugin | 90594 | sql | 10784 | high | 27801 |
| 4 | low | 34801 | wordpress | 7193 | info | 26861 |
| 5 | medium | 34369 | auth | 4451 | critical | 16039 |
| 6 | candidate | 33656 | remote_code_execution | 1845 | unknown | 135 |
| 7 | tech | 17848 | detect | 1836 | informative | 19 |
| 8 | detect | 17025 | microsoft | 1412 | meduim | 19 |
| 9 | high | 16813 | web | 1391 | hight | 15 |
| 10 | service | 13835 | api | 1116 | cretical | 4 |

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

