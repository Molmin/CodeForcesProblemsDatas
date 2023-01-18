## Description

<div><p>There are <span class="tex-span"><i>n</i></span> walruses sitting in a circle. All of them are numbered in the clockwise order: the walrus number <span class="tex-span">2</span> sits to the left of the walrus number <span class="tex-span">1</span>, the walrus number <span class="tex-span">3</span> sits to the left of the walrus number <span class="tex-span">2</span>, ..., the walrus number <span class="tex-span">1</span> sits to the left of the walrus number <span class="tex-span"><i>n</i></span>.</p><p>The presenter has <span class="tex-span"><i>m</i></span> chips. The presenter stands in the middle of the circle and starts giving the chips to the walruses starting from walrus number <span class="tex-span">1</span> and moving clockwise. The walrus number <span class="tex-span"><i>i</i></span> gets <span class="tex-span"><i>i</i></span> chips. If the presenter can't give the current walrus the required number of chips, then the presenter takes the remaining chips and the process ends. Determine by the given <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> how many chips the presenter will get in the end.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of walruses and the number of chips correspondingly.</p></div><div class="output-specification"><p>Print the number of chips the presenter ended up with.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of walruses and the number of chips correspondingly.</p>

## Output

<p>Print the number of chips the presenter ended up with.</p>





```input1
4 11

```




```input2
17 107

```




```input3
3 8

```




```output1
0

```




```output2
2

```




```output3
1

```



## Note

<p>In the first sample the presenter gives one chip to the walrus number <span class="tex-span">1</span>, two chips to the walrus number <span class="tex-span">2</span>, three chips to the walrus number <span class="tex-span">3</span>, four chips to the walrus number <span class="tex-span">4</span>, then again one chip to the walrus number <span class="tex-span">1</span>. After that the presenter runs out of chips. He can't give anything to the walrus number <span class="tex-span">2</span> and the process finishes.</p><p>In the third sample the presenter gives one chip to the walrus number <span class="tex-span">1</span>, two chips to the walrus number <span class="tex-span">2</span>, three chips to the walrus number <span class="tex-span">3</span>, then again one chip to the walrus number <span class="tex-span">1</span>. The presenter has one chip left and he can't give two chips to the walrus number <span class="tex-span">2</span>, that's why the presenter takes the last chip.</p>
