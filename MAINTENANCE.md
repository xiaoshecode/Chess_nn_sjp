# Chess_nn_sjp 维护说明

使用强化学习实现中国象棋，保留 TensorFlow 不同版本入口。

- 上游：https://github.com/east-before-dawn/Check-Chess-Cheer
- 在线文档：https://xiaoshecode.github.io/xiaoshecode/repos/Chess_nn_sjp/
- 检查日期：2026-10-30

## 环境与使用

- 先选择 main.py 或 main_tf2.py 对应的 TensorFlow 环境，参考源码导入项安装依赖。

使用/检查入口（需先满足依赖条件）：

- `python main_tf2.py`

## 目录职责

- main.py / main_tf2.py — 不同 TensorFlow 入口
- ChessBoard.py / ChessPiece.py — 棋盘棋子
- policy_value_network*.py — 策略价值网络
- assets/ / images/ — 界面资源

## 本次整理

- 新增维护文档和在线文档入口，补全用途、目录、使用路径及验证边界。

## 检查记录

- **仓库目录与入口盘点**（passed）：检查 Git 索引中的 194 个路径、README 和项目配置；不等于功能验收。
- **XML parse**（passed）：5 个文件通过解析；不导入依赖、不执行应用。
- **Python AST**（passed）：28 个文件通过解析；不导入依赖、不执行应用。
- **JSON/notebook parse**（passed）：3 个文件通过解析；不导入依赖、不执行应用。
- **完整构建与端到端运行**（not_run）：缺少依赖版本清单；仓库含已跟踪的 __pycache__ 和 IDE 文件。未运行训练或图形界面。

## 验证边界与待办

- 缺少依赖版本清单；仓库含已跟踪的 __pycache__ 和 IDE 文件。未运行训练或图形界面。

## 后续维护约定

保留上游许可证与作者信息。沿用现有模块边界和格式配置；修复功能时同步最小回归验证。依赖或接口变更需写明迁移步骤，避免仅为目录美观搬动公开入口。
