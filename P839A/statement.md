## Description

<div><p>Bran and his older sister Arya are from the same house. Bran like candies so much, so Arya is going to give him some Candies.</p><p>At first, Arya and Bran have <span class="tex-span">0</span> Candies. There are <span class="tex-span"><i>n</i></span> days, at the <span class="tex-span"><i>i</i></span>-th day, Arya finds <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> candies in a box, that is given by the Many-Faced God. Every day she can give Bran <span class="tex-font-style-bf">at most</span> <span class="tex-span">8</span> of her candies. If she don't give him the candies at the same day, they are saved for her and she can give them to him later.</p><p>Your task is to find the minimum number of days Arya needs to give Bran <span class="tex-span"><i>k</i></span> candies <span class="tex-font-style-bf">before</span> the end of the <span class="tex-span"><i>n</i></span>-th day. Formally, you need to output the minimum day index to the end of which <span class="tex-span"><i>k</i></span> candies will be given out (the days are indexed from 1 to <span class="tex-span"><i>n</i></span>).</p><p>Print <span class="tex-font-style-tt">-1</span> if she can't give him <span class="tex-span"><i>k</i></span> candies during <span class="tex-span"><i>n</i></span> given days.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p></div><div class="output-specification"><p>If it is impossible for Arya to give Bran <span class="tex-span"><i>k</i></span> candies within <span class="tex-span"><i>n</i></span> days, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise print a single integer&nbsp;— the minimum number of days Arya needs to give Bran <span class="tex-span"><i>k</i></span> candies before the end of the <span class="tex-span"><i>n</i></span>-th day.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p>

## Output

<p>If it is impossible for Arya to give Bran <span class="tex-span"><i>k</i></span> candies within <span class="tex-span"><i>n</i></span> days, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise print a single integer&nbsp;— the minimum number of days Arya needs to give Bran <span class="tex-span"><i>k</i></span> candies before the end of the <span class="tex-span"><i>n</i></span>-th day.</p>





```input1
2 3
1 2

```




```input2
3 17
10 10 10

```




```input3
1 9
10

```




```output1
2
```




```output2
3
```




```output3
-1
```



## Note

<p>In the first sample, Arya can give Bran <span class="tex-span">3</span> candies in <span class="tex-span">2</span> days.</p><p>In the second sample, Arya can give Bran <span class="tex-span">17</span> candies in <span class="tex-span">3</span> days, because she can give him at most <span class="tex-span">8</span> candies per day.</p><p>In the third sample, Arya can't give Bran <span class="tex-span">9</span> candies, because she can give him at most <span class="tex-span">8</span> candies per day and she must give him the candies within <span class="tex-span">1</span> day.</p>
