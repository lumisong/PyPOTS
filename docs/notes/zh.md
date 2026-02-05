# PyPOTS 文档目录说明

本文档用于说明 `docs/` 目录结构与维护要点，属于内部维护说明。
当前并未在 `index.rst` 中引用，因此不会被 Sphinx 自动渲染。

## 目录结构（docs/）

```
docs/
├─ about_us.rst
├─ algo_table.rst
├─ benchpots.rst
├─ conf.py
├─ examples.rst
├─ faq.rst
├─ index.rst
├─ install.rst
├─ make.bat
├─ Makefile
├─ milestones.rst
├─ model_api.rst
├─ pygrinder.rst
├─ pypots.anomaly_detection.rst
├─ pypots.classification.rst
├─ pypots.clustering.rst
├─ pypots.data.rst
├─ pypots.forecasting.rst
├─ pypots.imputation.rst
├─ pypots.nn.rst
├─ pypots.optim.rst
├─ pypots.representation.rst
├─ pypots.rst
├─ pypots.utils.rst
├─ references.bib
├─ references.rst
├─ tsdb.rst
└─ notes/
   └─ zh.md
```

## 文档入口与构建

- `index.rst` 是 Sphinx 的主入口。
- `conf.py` 是 Sphinx 配置文件。
- `Makefile` 与 `make.bat` 提供构建命令。

构建示例：

```powershell
# Windows
.\make.bat html
```

```bash
# Linux/macOS
make html
```

默认输出目录为 `docs/_build/html`。

## 内容页面（介绍与使用）

- `about_us.rst` 项目介绍
- `install.rst` 安装指南
- `examples.rst` 使用示例
- `faq.rst` 常见问题
- `milestones.rst` 里程碑
- `benchpots.rst` BenchPOTS 说明
- `algo_table.rst` 算法总览表
- `model_api.rst` 模型 API 概览
- `references.rst` 与 `references.bib` 文献引用
- `tsdb.rst` TSDB 相关说明
- `pygrinder.rst` PyGrinder 子项目说明

## 模块 API 文档

- `pypots.rst` 顶层模块
- `pypots.imputation.rst` 插补模块
- `pypots.classification.rst` 分类模块
- `pypots.clustering.rst` 聚类模块
- `pypots.forecasting.rst` 预测模块
- `pypots.anomaly_detection.rst` 异常检测模块
- `pypots.representation.rst` 表征学习模块
- `pypots.data.rst` 数据处理模块
- `pypots.nn.rst` 通用神经网络组件
- `pypots.optim.rst` 优化器与学习率调度
- `pypots.utils.rst` 工具函数

## 维护建议

- 新增模型或模块后，更新对应的 `pypots.*.rst`。
- 新增算法时同步更新 `algo_table.rst`。
- 新增引用请补充 `references.bib`。
- 若需要中文文档纳入 Sphinx，请在 `index.rst` 中显式引用。
