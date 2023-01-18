## Description

<div><p>Arya has <span class="tex-span"><i>n</i></span> opponents in the school. Each day he will fight with all opponents who are present this day. His opponents have some fighting plan that guarantees they will win, but implementing this plan requires presence of them all. That means if one day at least one of Arya's opponents is absent at the school, then Arya will beat all present opponents. Otherwise, if all opponents are present, then they will beat Arya.</p><p>For each opponent Arya knows his schedule&nbsp;— whether or not he is going to present on each particular day. Tell him the maximum number of <span class="tex-font-style-bf">consecutive</span> days that he will beat all present opponents.</p><p>Note, that if some day there are no opponents present, Arya still considers he beats all the present opponents.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>d</i> ≤ 100</span>)&nbsp;— the number of opponents and the number of days, respectively.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>d</i></span> lines contains a string of length <span class="tex-span"><i>n</i></span> consisting of characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'. The <span class="tex-span"><i>j</i></span>-th character of this string is '<span class="tex-font-style-tt">0</span>' if the <span class="tex-span"><i>j</i></span>-th opponent is going to be absent on the <span class="tex-span"><i>i</i></span>-th day.</p></div><div class="output-specification"><p>Print the only integer&nbsp;— the maximum number of consecutive days that Arya will beat all present opponents.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>d</i> ≤ 100</span>)&nbsp;— the number of opponents and the number of days, respectively.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>d</i></span> lines contains a string of length <span class="tex-span"><i>n</i></span> consisting of characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'. The <span class="tex-span"><i>j</i></span>-th character of this string is '<span class="tex-font-style-tt">0</span>' if the <span class="tex-span"><i>j</i></span>-th opponent is going to be absent on the <span class="tex-span"><i>i</i></span>-th day.</p>

## Output

<p>Print the only integer&nbsp;— the maximum number of consecutive days that Arya will beat all present opponents.</p>





```input1
2 2
10
00

```




```input2
4 1
0100

```




```input3
4 5
1101
1111
0110
1011
1111

```




```output1
2

```




```output2
1

```




```output3
2

```



## Note

<p>In the first and the second samples, Arya will beat all present opponents each of the <span class="tex-span"><i>d</i></span> days.</p><p>In the third sample, Arya will beat his opponents on days <span class="tex-span">1</span>, <span class="tex-span">3</span> and <span class="tex-span">4</span> and his opponents will beat him on days <span class="tex-span">2</span> and <span class="tex-span">5</span>. Thus, the maximum number of consecutive winning days is <span class="tex-span">2</span>, which happens on days <span class="tex-span">3</span> and <span class="tex-span">4</span>.</p>
