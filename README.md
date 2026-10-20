# RoomTracker rules

RoomTracker App 读取的公开规则参数（每年的 TFSA / RRSP 上限、FHSA、HBP）。只有公开的 CRA 数字，没有任何个人资料。

Public rule parameters used by the RoomTracker app (annual TFSA / RRSP limits, FHSA, HBP). CRA public figures only — no personal data.

## 怎么更新

1. 改 `rules.json` 里的数字（金额单位是元，不是分）。
2. **`version` 一定要改成今天的日期，格式 `YYYY.MM.DD`，月和日补零**（例：`2026.11.05`）。App 只接受比自己现有版本新的文件。
3. 提交、推送。App 每天最多检查一次，用户下次打开 App 时更新。

App 会拒绝明显有问题的文件（版本比 App 内置的旧、少了年份、格式不对），这时继续用原来的数字。
