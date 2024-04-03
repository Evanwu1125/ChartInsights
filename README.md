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
    - overall evaluation results
    - vary chart element results
    - vary chart quality results
    - Visual prompt and Chain-of-Charts


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
combination of visual and textual prompts lead to enhanced performance in low-level ChartQA tasks with GPT-4V? This question explores the potential for achieving better results by integrating both types of prompts.
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


### Pipeline for dataset construction
<div align=center>
<img src="./pngs/dataset%20construction%20pipeline.png" width="600px" center>
</div>

## Dataset Examples
<div align=center>
<img src="./pngs/dataset_example.png" width="800px" center>
</div>

## Evaluation on ChartInsights
**We conducted a total of four sets of evaluations on GPT-4V.**

- The first set of evaluations was a general assessment of GPT-4V's performance, utilizing the test dataset from ChartInsights.

    You can get the test set in the [overall directory](/overall). The relevant annotations and qa_pairs are all available. This set contains 400 pictures and 17552 questions in total, covering all 10 low-level analysis tasks and 7 charts from different categories.

    The results from GPT-4V are well preserved in [overall directory](/overall) as well.

- The second set of evaluations involved altering 15 types of chart elements.

    You can get altered images in [Vary Chart Element directory](https://github.com/Evanwu1125/ChartInsights/tree/main/evaluations/Vary%20Chart%20Element). This set contains 356 visual variants and 17972 corresponding qa_pairs, covering all 10 low-level analysis tasks and 7 charts from different categories.

    The results from GPT-4V according to this set are well preserved as well.
- The third set of evaluations introduced 6 noise into the images. 

    You can get noised images in [Vary Chart Quality](https://github.com/Evanwu1125/ChartInsights/tree/main/evaluations/Vary%20Image%20Quality). This set contains 245 visual variants and 8456 corresponding qa_pairs, covering all 10 low-level analysis tasks and 7 charts from different categories.

    The results from GPT-4V according to this set are well preserved as well.
  
- The fourth set of evaluations incorporated the addition of visual prompts and the design of Chain-of-Charts to the images.

    You can get visual-prompted images in [Three Types of Visual Prompt](https://github.com/Evanwu1125/ChartInsights/tree/main/evaluations/Three%20Types%20of%20Visual%20Prompt). This set contains 255 visual variants and 1020 corresponding qa_pairs, covering all 10 low-level analysis tasks and 7 charts from different categories.

    The results from GPT-4V according to this set are well preserved as well.
## Evaluation scripts on ChartInsights with GPT-4V
You can directly using
## Evaluation Results
### Overall evaluation results
<div align=center>
<img src="./pngs/overall_results.png" width="800px" center>
</div>

### vary chart element results
<div align=center>
<img src="./pngs/vary_chart_element_results.png" width="800px" center>
</div>

### vary chart quality results
<div align=center>
<img src="./pngs/vary_image_quality.png" width="800px" center>
</div>

### visual prompt and chain-of-charts
<div align=center>
<img src="./pngs/visual_prompt_and_chain_of_charts.png" width="800px" center>
</div>
