# Data_Analysis

> 数据分析四件套速通仓：Jupyter + Matplotlib + NumPy + Pandas，一键上手基础操作。  
> Quickstart hub for Python data analysis essentials: Jupyter, NumPy, Pandas, Matplotlib.

## 目标 (Goals)
- 快速演示最常用的数据读取、清洗、统计与可视化操作
- 形成可复制的 Notebook 模板
- 积累常见数据分析场景（缺失值处理、分组聚合、时间序列、图形定制）

## 技术栈 (Stack)
| 组件 | 用途 |
|------|------|
| Jupyter Notebook | 交互与教学 |
| NumPy | 数值计算与数组操作 |
| Pandas | 数据清洗、索引、统计聚合 |
| Matplotlib / Seaborn | 可视化与图表增强 |

## 目录规划 (Structure)
```
Data_Analysis/
├── notebooks/
│   ├── 01_numpy_basics.ipynb
│   ├── 02_pandas_io.ipynb
│   ├── 03_pandas_cleaning.ipynb
│   ├── 04_groupby_aggregation.ipynb
│   ├── 05_time_series.ipynb
│   ├── 06_visualization_matplotlib.ipynb
│   ├── 07_visualization_seaborn.ipynb
│   ├── 08_merge_join_concat.ipynb
│   ├── 09_pivot_crosstab.ipynb
│   └── 10_tips_and_tricks.ipynb
├── data/
│   ├── sample.csv
│   └── README.md
├── templates/
│   ├── analysis_report_template.ipynb
│   └── exploration_starter.ipynb
├── docs/
│   ├── cheatsheet_pandas.md
│   ├── cheatsheet_numpy.md
│   └── visualization_guidelines.md
├── requirements.txt
└── README.md
```

## 快速开始 (Quick Start)
```bash
git clone https://github.com/logcoke/Data_Analysis.git
cd Data_Analysis
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

`requirements.txt` 推荐：
```
jupyter
numpy
pandas
matplotlib
seaborn
```

## Notebook 规范
每个 Notebook 建议包含：
1. 背景/目的说明  
2. 步骤分节（读取 → 清洗 → 统计 → 可视化）  
3. 关键 API 总结（放在尾部）  
4. 可复现的随机种子（如涉及模拟数据）  

## 常见场景示例 (Planned Topics)
- 缺失值处理：`isna()`, `fillna()`
- 数据重塑：`pivot`, `melt`, `stack`, `unstack`
- 分组聚合：`groupby`, `agg`, `transform`
- 时间序列：`DatetimeIndex`, 频率重采样
- 合并连接：`merge`, `join`, `concat`
- 可视化：子图布局、风格、颜色映射、注释

## Roadmap
- [ ] 完成基础 10 个 Notebook
- [ ] 补充 Pandas 与 NumPy 速查表
- [ ] 加入时间序列案例
- [ ] 增加数据清洗常见模式总结
- [ ] 模板化报告输出
- [ ] 增加性能优化片段（`vectorization`, `query`, `eval`）
- [ ] 扩展简单交互式可视化（Plotly 可选）

## 贡献 (Contributing)
欢迎：
- 新增典型数据场景示例
- 优化可视化风格与统一主题
- 添加更多速查表与最佳实践

提交流程：
1. 新建分支并添加 Notebook
2. 确保 Notebook 可从头顺序运行
3. 删除中间冗长输出（必要图表保留）

## License
尚未设置，可选 MIT 以便自由使用与分发。

## FAQ
Q: 为什么不用复杂 BI 或大数据工具？  
A: 专注“入门与高频操作”，保持学习曲线平缓。  
Q: 数据来源？  
A: 使用轻量示例数据或公开 CSV；不直接提交敏感数据。

---

学习、整理、复用，一仓搞定基础数据分析。
