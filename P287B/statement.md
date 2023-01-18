## Description

<div><p>Vova, the Ultimate Thule new shaman, wants to build a pipeline. As there are exactly <span class="tex-span"><i>n</i></span> houses in Ultimate Thule, Vova wants the city to have exactly <span class="tex-span"><i>n</i></span> pipes, each such pipe should be connected to the water supply. A pipe can be connected to the water supply if there's water flowing out of it. Initially Vova has only one pipe with flowing water. Besides, Vova has several splitters.</p><p>A splitter is a construction that consists of one input (it can be connected to a water pipe) and <span class="tex-span"><i>x</i></span> output pipes. When a splitter is connected to a water pipe, water flows from each output pipe. You can assume that the output pipes are ordinary pipes. For example, you can connect water supply to such pipe if there's water flowing out from it. At most one splitter can be connected to any water pipe.</p><center> <img class="tex-graphics" src="file://LWQQdqVl.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script">The figure shows a <span class="tex-span">4</span>-output splitter</span> </center><p>Vova has one splitter of each kind: with <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>, ..., <span class="tex-span"><i>k</i></span> outputs. Help Vova use the minimum number of splitters to build the required pipeline or otherwise state that it's impossible.</p><p>Vova needs the pipeline to have exactly <span class="tex-span"><i>n</i></span> pipes with flowing out water. Note that some of those pipes can be the output pipes of the splitters.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of splitters needed to build the pipeline. If it is impossible to build a pipeline with the given splitters, print -1.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print a single integer — the minimum number of splitters needed to build the pipeline. If it is impossible to build a pipeline with the given splitters, print -1.</p>





```input1
4 3

```




```input2
5 5

```




```input3
8 4

```




```output1
2

```




```output2
1

```




```output3
-1

```


