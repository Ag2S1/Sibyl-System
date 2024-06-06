# Sibyl System

This is an experimental project. We are attempting to design a general assistant system that evolves from System1 to System2. The name Sibyl comes from the multi-agent system composed of numerous human brains in [Psycho-Pass](https://psychopass.fandom.com/wiki/Sibyl_System).

## Philosophy
* From System1 to System2
Currently popular assistant systems like ChatGPT are designed to solve human decision-making problems at the minute level. Even with methods such as CoT and ReAct, they encounter significant difficulties in handling problems at the 10-minute level. Our system aims to gradually solve problems from the minute level to the hour level and even the day level.
* Complexity Control
Decoder-only models have a beneficial characteristic of being pure functions, which allows us to better control complexity. However, as we evolve from System1 to System2, the introduction of states inevitably causes the system's complexity to gradually spiral out of control. Some existing Multi-Agent solutions introduce too many states, making the system difficult to scale sustainably. We aim to control this Multi-Agent characteristic within parts of the system or push it to the system's edges.

## Architecture
![Sibyl System](./imgs/sibyl.jpeg)