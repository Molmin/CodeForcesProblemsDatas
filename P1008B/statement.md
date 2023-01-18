## Description

<div><p>There are $n$ rectangles in a row. You can either turn each rectangle by $90$ degrees or leave it as it is. If you turn a rectangle, its width will be height, and its height will be width. Notice that you can turn any number of rectangles, you also can turn all or none of them. <span class="tex-font-style-bf">You can not change the order of the rectangles.</span></p><p>Find out if there is a way to make the rectangles go in order of non-ascending height. In other words, after all the turns, a height of every rectangle has to be not greater than the height of the previous rectangle (if it is such). </p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the number of rectangles.</p><p>Each of the next $n$ lines contains two integers $w_i$ and $h_i$ ($1 \leq w_i, h_i \leq 10^9$)&nbsp;— the width and the height of the $i$-th rectangle.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if there is a way to make the rectangles go in order of non-ascending height, otherwise print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the number of rectangles.</p><p>Each of the next $n$ lines contains two integers $w_i$ and $h_i$ ($1 \leq w_i, h_i \leq 10^9$)&nbsp;— the width and the height of the $i$-th rectangle.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if there is a way to make the rectangles go in order of non-ascending height, otherwise print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower).</p>





```input1
3
3 4
4 6
3 5

```




```input2
2
3 4
5 5

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first test, you can rotate the second and the third rectangles so that the heights will be <span class="tex-font-style-tt">[4, 4, 3]</span>.</p><p>In the second test, there is no way the second rectangle will be not higher than the first one.</p>
