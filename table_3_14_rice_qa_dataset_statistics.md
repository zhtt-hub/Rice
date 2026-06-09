表3-14 水稻问答数据集统计结果
Table 3-14 Statistics of the Rice Question Answering Dataset

| 问题类型 | 样本数量 | 占比 | 主要证据来源 | 推荐处理路径 |
| --- | ---: | ---: | --- | --- |
| 事实型问题 | 1,700 | 15.43% | 文档知识库、农业标准题录、政府公开文件 | GraphRAG-MCP 快路径 |
| 关系型问题 | 1,667 | 15.13% | 文档知识库、水稻应用知识图谱 | GraphRAG-MCP 快路径 |
| 轻量多跳问题 | 2,345 | 21.28% | 水稻应用知识图谱、农业标准题录、政府公开文件 | GraphRAG-MCP 快路径 |
| 复杂推理问题 | 1,924 | 17.46% | 水稻应用知识图谱 | CoT-MCP 慢路径 |
| 文献综合问题 | 3,382 | 30.70% | 开放获取论文全文、科研文献题录 | CoT-MCP 慢路径 |
| 合计 | 11,018 | 100.00% | — | — |

数据质量检查结果：
- 样本总数：11,018
- question_id 重复：否，重复数量 0
- question 为空：0
- reference_answer 或 answer 为空：0
- evidence_source 为空：0
- route_label 为空：0
- question_type 未识别类别：0
- 每类问题数量过少：无
- route_label 不一致类别：无
- key_entities 为空或字段不存在：0

CSV 文件：D:\download\大论文\large_scale\qa\rice_qa_dataset_statistics.csv
质量检查 JSON：D:\download\大论文\large_scale\qa\rice_qa_dataset_quality_check.json