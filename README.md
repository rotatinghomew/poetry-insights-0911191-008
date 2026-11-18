# 诗词节售检票异常诊断与值班派单

本项目保存票务异常分析所需的合成出票批次、设备区间、节目变更和人工点数资料，均使用 UTF-8 CSV。空字段表示记录未提供。

## 数据

- `data/ticket_batches.csv`：场次、渠道和出票可用数量。
- `data/device_intervals.csv`：终端分段扫描及上传状态。
- `data/show_changes.csv`：移场、停开及生效时间。
- `data/manual_counts.csv`：人工点数和覆盖区域。

## 环境与验证

需要 Python 3.11 或更新版本；项目仅使用 Python 标准库。可用 `python3 -m unittest discover -s tests -v` 检查 CSV 结构与本地资料完整性。
