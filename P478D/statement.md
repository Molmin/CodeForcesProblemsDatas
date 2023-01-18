## Description

<div><p>There are <span class="tex-span"><i>r</i></span> red and <span class="tex-span"><i>g</i></span> green blocks for construction of the <span class="tex-font-style-it">red-green</span> tower. <span class="tex-font-style-it">Red-green</span> tower can be built following next rules:</p><ul><p> </p><li> Red-green tower is consisting of some number of levels;<p> </p></li><li> Let the red-green tower consist of <span class="tex-span"><i>n</i></span> levels, then the first level of this tower should consist of <span class="tex-span"><i>n</i></span> blocks, second level — of <span class="tex-span"><i>n</i> - 1</span> blocks, the third one — of <span class="tex-span"><i>n</i> - 2</span> blocks, and so on — the last level of such tower should consist of the one block. In other words, each successive level should contain one block less than the previous one;<p> </p></li><li> Each level of the red-green tower should contain blocks of the same color.</li></ul><center> <img class="tex-graphics" src="file://mnw3UzOF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Let <span class="tex-span"><i>h</i></span> be the maximum possible number of levels of red-green tower, that can be built out of <span class="tex-span"><i>r</i></span> red and <span class="tex-span"><i>g</i></span> green blocks meeting the rules above. The task is to determine how many different red-green towers having <span class="tex-span"><i>h</i></span> levels can be built out of the available blocks.</p><p>Two red-green towers are considered different if there exists some level, that consists of red blocks in the one tower and consists of green blocks in the other tower.</p><p>You are to write a program that will find the number of different red-green towers of height <span class="tex-span"><i>h</i></span> modulo&nbsp;<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The only line of input contains two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>g</i></span>, separated by a single space — the number of available red and green blocks respectively (<span class="tex-span">0 ≤ <i>r</i>, <i>g</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>r</i> + <i>g</i> ≥ 1</span>).</p></div><div class="output-specification"><p>Output the only integer — the number of different possible red-green towers of height <span class="tex-span"><i>h</i></span> modulo&nbsp;<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The only line of input contains two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>g</i></span>, separated by a single space — the number of available red and green blocks respectively (<span class="tex-span">0 ≤ <i>r</i>, <i>g</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>r</i> + <i>g</i> ≥ 1</span>).</p>

## Output

<p>Output the only integer — the number of different possible red-green towers of height <span class="tex-span"><i>h</i></span> modulo&nbsp;<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
4 6

```




```input2
9 7

```




```input3
1 1

```




```output1
2

```




```output2
6

```




```output3
2

```



## Note

<p>The image in the problem statement shows all possible red-green towers for the first sample.</p>
