 # Gemini SQL生成微调项目

## 项目简介
本项目展示了如何使用Google Cloud的Gemini模型进行微调，以提升SQL查询生成的准确性。项目使用了来自 Hugging Face 的公共数据集 b-mc2/sql-create-context，通过微调使模型能够更准确地将自然语言问题转换为SQL查询语句。

## 环境要求
- Google Cloud账号和项目
- 必要的Python包：
  - google-cloud-aiplatform
  - google-genai
  - datasets
  - pandas
  - numpy
  - plotly
  - tqdm

## 主要功能
1. 数据准备和预处理
2. 模型微调
3. 性能评估
4. 结果可视化

## 项目结构
- 环境准备：安装必要的依赖包
- 数据处理：加载和处理SQL数据集
- 模型训练：使用Gemini模型进行微调
- 性能评估：使用EM（Exact Match）和F1分数评估模型性能

## 使用方法
1. 环境配置
```bash
pip install google-cloud-aiplatform google-genai datasets
```

2. 认证配置
- 确保已配置Google Cloud认证
- 设置项目ID和位置信息

3. 运行微调
- 准备训练数据
- 配置微调参数
- 启动训练任务

## 实验结果
微调后的模型性能显著提升：
- 原始模型：
  - EM分数：0.0026
  - F1分数：0.8068

- 微调后模型：
  - EM分数：0.7727
  - F1分数：0.9690

## 注意事项
1. 确保有足够的Google Cloud配额
2. 数据集需要符合特定格式要求
3. 微调过程可能需要较长时间

## 参考资料
- [Google Cloud文档](https://cloud.google.com/vertex-ai)
- [Gemini API文档](https://cloud.google.com/vertex-ai/docs/generative-ai/model-reference/gemini)
