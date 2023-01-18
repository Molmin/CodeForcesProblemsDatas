## Description

<div><p>Something happened in Uzhlyandia again... There are riots on the streets... Famous Uzhlyandian superheroes Shean the Sheep and Stas the Giraffe were called in order to save the situation. Upon the arriving, they found that citizens are worried about maximum values of the Main Uzhlyandian Function <span class="tex-span"><i>f</i></span>, which is defined as follows:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://6SsAj1Pc.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>In the above formula, <span class="tex-span">1 ≤ <i>l</i> &lt; <i>r</i> ≤ <i>n</i></span> must hold, where <span class="tex-span"><i>n</i></span> is the size of the Main Uzhlyandian Array <span class="tex-span"><i>a</i></span>, and <span class="tex-span">|<i>x</i>|</span> means absolute value of <span class="tex-span"><i>x</i></span>. But the heroes skipped their math lessons in school, so they asked you for help. Help them calculate the maximum value of <span class="tex-span"><i>f</i></span> among all possible values of <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> for the given array <span class="tex-span"><i>a</i></span>.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the size of the array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (-<span class="tex-span">10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the array elements.</p></div><div class="output-specification"><p>Print the only integer&nbsp;— the maximum value of <span class="tex-span"><i>f</i></span>.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the size of the array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (-<span class="tex-span">10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the array elements.</p>

## Output

<p>Print the only integer&nbsp;— the maximum value of <span class="tex-span"><i>f</i></span>.</p>





```input1
5
1 4 2 3 1

```




```input2
4
1 5 4 7

```




```output1
3
```




```output2
6
```



## Note

<p>In the first sample case, the optimal value of <span class="tex-span"><i>f</i></span> is reached on intervals <span class="tex-span">[1, 2]</span> and <span class="tex-span">[2, 5]</span>.</p><p>In the second case maximal value of <span class="tex-span"><i>f</i></span> is reachable only on the whole array.</p>
