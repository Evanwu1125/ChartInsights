# Evaluating Task-based Effectiveness of GPT4-V on Charts
- [About ChartsInsights](main/README.md)
    - [Scale of ChartInsights](main/README.md)
    - [10 Low-Level analysis tasks](main/README.md)
    - [Distribution of 7 charts on 10 tasks](main/README.md)
    - [Pipeline for Dataset Construction](main/README.md)
- [Dataset Examples](main/README.md)
- [Evaluations on ChartInsights](main/README.md)
    - [Evaluation Set](main/README.md)
    - [Vary the Chart Elements](main/README.md)
    - [Vary the Chart Quality](main/README.md)
    - [Three types of Visual Prompts and Chain-of-Thought](main/README.md)
- [Evaluation Scripts on ChartInsights with GPT-4V](main/README.md)
- [Evaluations Results](main/README.md)


## About ChartInsights
In this paper, we aim to systematically investigate the capabilities of GPT-4V in addressing 10 low-level data analysis tasks. Our study seeks to answer the following critical questions, shedding light on the potential of MLLMs in performing detailed, granular analyses.

__Q1__: Impact of Textual Prompt Variations. What is the impact of
different textual prompts on GPT-4V ’s output accuracy? This
question aims to assess the baseline performance and capabilities
of GPT-4V in different low-level tasks.

__Q2__: Impact of Visual Variations and Visual Prompts: How do
different visual prompts, such as alterations in color schemes,
layout configurations (e.g., aspect ratio), and image quality, affect
the performance of GPT-4V in low-level tasks?

__Q3__: Impact of Chain-of-Thoughts. Can we enhance basic textual
prompts in Q1 with a chain-of-thoughts like approach?

__Q4__: Synergistic Effect of Visual and Textual Prompts: Can the
combination of visual and textual prompts lead to enhanced performance in low-level ChartQA tasks with GPT-4V? This questionexplores the potential for achieving better results by integratingboth types of prompts.
### Scale of ChartInsights
The ChartInsights dataset contains 89,388 (chart, task, query, answer)
ChartQA samples across 7 chart types for 10 low-level data analysis
tasks on charts. The Donut chart shows the proportion of 10 low-level tasks
(3 task groups) in ChartInsights. Among them, the analysis task group
is the largest, accounting for 42.46%. This task group examines the
reasoning power of multi-modal large models on charts. The heatmap
shows the distribution of 10 low-level tasks and 7 chart types.
### Donut chart showing the distribution of 10 low-level tasks
<div align=center>
<img src="./pngs/donut%20chart.png" width="400px" center>
</div>


### Heatmap for showing the distribution of 7 charts on 10 tasks
<div align=center>
<img src="./pngs/heatmap.png" width="600px" center>
</div>

### pipeline for dataset construction
<div align=center>
<img src="./pngs/dataset%20construction%20pipeline.png" width="600px" center>
</div>

