# Sibyl: Simple yet Effective Agent Framework for Complex Real-world Reasoning
<p align="center">
<img width="1000px" alt="Sibyl System" src="https://github.com/Ag2S1/Sibyl-System/blob/main/imgs/Sibyl.png?raw=true">
</p>
<p align="center">
      <a href="https://arxiv.org/abs/2407.10718">[📄arXiv]</a>
      <a href="https://huggingface.co/papers/2407.10718">[🤗HF Paper]</a>
      <a href="https://github.com/Ag2S1/Sibyl-System">[🛠️Code]</a> 
</p>

This is an experimental project. We are attempting to design a general assistant system that evolves from System1 to System2. The name Sibyl comes from the multi-agent system composed of numerous human brains in [Psycho-Pass](https://psychopass.fandom.com/wiki/Sibyl_System).

## Citation
If you find our work useful, please cite our paper:
```
@article{wang2024sibyl,
      title={Sibyl: Simple yet Effective Agent Framework for Complex Real-world Reasoning}, 
      author={Yulong Wang and Tianhao Shen and Lifeng Liu and Jian Xie},
      year={2024},
      eprint={2407.10718},
      archivePrefix={arXiv},
      primaryClass={cs.AI},
      url={https://arxiv.org/abs/2407.10718}, 
}
```


## Benchmark
### GAIA
|Model Name|Average score (%)|Level 1 score (%)| Level 2 score (%) | Level 3 score (%)|
|-|-|-|-|-|
|**Sibyl System v0.2**|34.55|47.31|32.7|16.33|
|Multi-Agent Experiment v0.1 (powered by AutoGen)|32.33|47.31|28.93|14.58|
|FRIDAY|24.25|40.86|20.13|6.12|
|GPT4 + manually selected plugins|14.6|30.3|9.7|0|
|GPT4 Turbo|6.67|9.68|6.92|0|
|AutoGPT4|5|15.05|0.63|0|

## Philosophy
### From System1 to System2
  
Currently popular assistant systems like ChatGPT are designed to solve human decision-making problems at the minute level. Even with methods such as CoT and ReAct, they encounter significant difficulties in handling problems at the 10-minute level. Our system aims to gradually solve problems from the minute level to the hour level and even the day level.

### Complexity Control

Decoder-only models have a beneficial characteristic of being pure functions, which allows us to better control complexity. However, as we evolve from System1 to System2, the introduction of states inevitably causes the system's complexity to gradually spiral out of control. Some existing Multi-Agent solutions introduce too many states, making the system difficult to scale sustainably. We aim to control this Multi-Agent characteristic within parts of the system or push it to the system's edges.

## Contact

If you have any inquiries, please feel free to raise an issue or reach out to us via email at: wangyulong@gmail.com, thshen@tju.edu.cn
