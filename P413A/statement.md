## Description

<div><p>Not so long ago company R2 bought company R1 and consequently, all its developments in the field of multicore processors. Now the R2 laboratory is testing one of the R1 processors.</p><p>The testing goes in <span class="tex-span"><i>n</i></span> steps, at each step the processor gets some instructions, and then its temperature is measured. The head engineer in R2 is keeping a report record on the work of the processor: he writes down the minimum and the maximum measured temperature in his notebook. His assistant had to write down all temperatures into his notebook, but (for unknown reasons) he recorded only <span class="tex-span"><i>m</i></span>.</p><p>The next day, the engineer's assistant filed in a report with all the <span class="tex-span"><i>m</i></span> temperatures. However, the chief engineer doubts that the assistant wrote down everything correctly (naturally, the chief engineer doesn't doubt his notes). So he asked you to help him. Given numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>min</i></span>, <span class="tex-span"><i>max</i></span> and the list of <span class="tex-span"><i>m</i></span> temperatures determine whether you can upgrade the set of <span class="tex-span"><i>m</i></span> temperatures to the set of <span class="tex-span"><i>n</i></span> temperatures (that is add <span class="tex-span"><i>n</i> - <i>m</i></span> temperatures), so that the minimum temperature was <span class="tex-span"><i>min</i></span> and the maximum one was <span class="tex-span"><i>max</i></span>.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>min</i>, <i>max</i></span> <span class="tex-span">(1 ≤ <i>m</i> &lt; <i>n</i> ≤ 100;&nbsp;1 ≤ <i>min</i> &lt; <i>max</i> ≤ 100)</span>. The second line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the temperatures reported by the assistant.</p><p>Note, that the reported temperatures, and the temperatures you want to add can contain equal temperatures.</p></div><div class="output-specification"><p>If the data is consistent, print '<span class="tex-font-style-tt">Correct</span>' (without the quotes). Otherwise, print '<span class="tex-font-style-tt">Incorrect</span>' (without the quotes).</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>min</i>, <i>max</i></span> <span class="tex-span">(1 ≤ <i>m</i> &lt; <i>n</i> ≤ 100;&nbsp;1 ≤ <i>min</i> &lt; <i>max</i> ≤ 100)</span>. The second line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the temperatures reported by the assistant.</p><p>Note, that the reported temperatures, and the temperatures you want to add can contain equal temperatures.</p>

## Output

<p>If the data is consistent, print '<span class="tex-font-style-tt">Correct</span>' (without the quotes). Otherwise, print '<span class="tex-font-style-tt">Incorrect</span>' (without the quotes).</p>





```input1
2 1 1 2
1

```




```input2
3 1 1 3
2

```




```input3
2 1 1 3
2

```




```output1
Correct

```




```output2
Correct

```




```output3
Incorrect

```



## Note

<p>In the first test sample one of the possible initial configurations of temperatures is [1, 2].</p><p>In the second test sample one of the possible initial configurations of temperatures is [2, 1, 3].</p><p>In the third test sample it is impossible to add one temperature to obtain the minimum equal to 1 and the maximum equal to 3.</p>
