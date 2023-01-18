## Description

<div><p>Genos recently installed the game Zuma on his phone. In Zuma there exists a line of <span class="tex-span"><i>n</i></span> gemstones, the <span class="tex-span"><i>i</i></span>-th of which has color <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. The goal of the game is to destroy all the gemstones in the line as quickly as possible.</p><p>In one second, Genos is able to choose exactly one continuous substring of colored gemstones that is a palindrome and remove it from the line. After the substring is removed, the remaining gemstones shift to form a solid line again. What is the minimum number of seconds needed to destroy the entire line?</p><p>Let us remind, that the string (or substring) is called <span class="tex-font-style-it">palindrome</span>, if it reads same backwards or forward. In our case this means the color of the first gemstone is equal to the color of the last one, the color of the second gemstone is equal to the color of the next to last and so on.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>)&nbsp;— the number of gemstones.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers, the <span class="tex-span"><i>i</i></span>-th of which is <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the color of the <span class="tex-span"><i>i</i></span>-th gemstone in a line.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of seconds needed to destroy the entire line.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>)&nbsp;— the number of gemstones.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers, the <span class="tex-span"><i>i</i></span>-th of which is <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the color of the <span class="tex-span"><i>i</i></span>-th gemstone in a line.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of seconds needed to destroy the entire line.</p>





```input1
3
1 2 1

```




```input2
3
1 2 3

```




```input3
7
1 4 4 2 3 2 1

```




```output1
1

```




```output2
3

```




```output3
2

```



## Note

<p>In the first sample, Genos can destroy the entire line in one second.</p><p>In the second sample, Genos can only destroy one gemstone at a time, so destroying three gemstones takes three seconds.</p><p>In the third sample, to achieve the optimal time of two seconds, destroy palindrome <span class="tex-font-style-tt">4 4</span> first and then destroy palindrome <span class="tex-font-style-tt">1 2 3 2 1</span>.</p>
