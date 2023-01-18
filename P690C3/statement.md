## Description

<div><p>Breaking news from zombie neurology! It turns out that – contrary to previous beliefs – every zombie is <span class="tex-font-style-it">born</span> with a single brain, and only later it evolves into a complicated brain structure. In fact, whenever a zombie consumes a brain, a new brain appears in its nervous system and gets immediately connected to one of the already existing brains using a single brain connector. Researchers are now interested in monitoring the brain latency of a zombie. Your task is to write a program which, given a history of evolution of a zombie's nervous system, computes its brain latency at every stage.</p></div><div class="input-specification"><p>The first line of the input contains one number <span class="tex-span"><i>n</i></span> – the number of brains in the final nervous system (<span class="tex-span">2 ≤ <i>n</i> ≤ 200000</span>). In the second line a history of zombie's nervous system evolution is given. For convenience, we number all the brains by <span class="tex-span">1, 2, ..., <i>n</i></span> in the same order as they appear in the nervous system (the zombie is born with a single brain, number <span class="tex-span">1</span>, and subsequently brains <span class="tex-span">2, 3, ..., <i>n</i></span> are added). The second line contains <span class="tex-span"><i>n</i> - 1</span> space-separated numbers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, meaning that after a new brain <span class="tex-span"><i>k</i></span> is added to the system, it gets connected to a parent-brain <img align="middle" class="tex-formula" src="file://VvMhcD7N.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i> - 1</span> space-separated numbers – the brain latencies after the brain number <span class="tex-span"><i>k</i></span> is added, for <span class="tex-span"><i>k</i> = 2, 3, ..., <i>n</i></span>.</p></div>

## Input

<p>The first line of the input contains one number <span class="tex-span"><i>n</i></span> – the number of brains in the final nervous system (<span class="tex-span">2 ≤ <i>n</i> ≤ 200000</span>). In the second line a history of zombie's nervous system evolution is given. For convenience, we number all the brains by <span class="tex-span">1, 2, ..., <i>n</i></span> in the same order as they appear in the nervous system (the zombie is born with a single brain, number <span class="tex-span">1</span>, and subsequently brains <span class="tex-span">2, 3, ..., <i>n</i></span> are added). The second line contains <span class="tex-span"><i>n</i> - 1</span> space-separated numbers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, meaning that after a new brain <span class="tex-span"><i>k</i></span> is added to the system, it gets connected to a parent-brain <img align="middle" class="tex-formula" src="file://VvMhcD7N.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>Output <span class="tex-span"><i>n</i> - 1</span> space-separated numbers – the brain latencies after the brain number <span class="tex-span"><i>k</i></span> is added, for <span class="tex-span"><i>k</i> = 2, 3, ..., <i>n</i></span>.</p>





```input1
6
1
2
2
1
5

```




```output1
1 2 2 3 4
```


