## Description

<div><p>You want to advertise your new business, so you are going to place two posters on a billboard in the city center. The billboard consists of $n$ vertical panels of width $1$ and varying integer heights, held together by a horizontal bar. The $i$-th of the $n$ panels has height $h_i$.</p><center> <img class="tex-graphics" src="file://LcfN9evd.png" style="max-width: 100.0%;max-height: 100.0%;" width="265px"> </center><p>Initially, all panels hang down from the bar (their top edges lie on it), but before placing the two posters, you are allowed to move each panel up by any integer length, as long as it is still connected to the bar (its bottom edge lies below or on it).</p><p>After the moves are done, you will place two posters: one below the bar and one above it. They are not allowed to go over the bar and they must be positioned completely inside of the panels.</p><p>What is the maximum total area the two posters can cover together if you make the optimal moves? <span class="tex-font-style-bf">Note that you can also place a poster of $0$ area. This case is equivalent to placing a single poster.</span></p></div><div class="input-specification"><p>The first line of input contains one integer $n$ ($1 \le n \le 10^4$)&nbsp;— the number of vertical panels.</p><p>The second line of input contains $n$ integers $h_1, h_2, ..., h_n$ ($1 \le h_i \le 10^{12}$)&nbsp;— the heights of the $n$ vertical panels.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum total area the two posters can cover together.</p></div>

## Input

<p>The first line of input contains one integer $n$ ($1 \le n \le 10^4$)&nbsp;— the number of vertical panels.</p><p>The second line of input contains $n$ integers $h_1, h_2, ..., h_n$ ($1 \le h_i \le 10^{12}$)&nbsp;— the heights of the $n$ vertical panels.</p>

## Output

<p>Print a single integer&nbsp;— the maximum total area the two posters can cover together.</p>





```input1
6
2 2 3 5 4 5
```




```input2
1
1
```




```output1
18
```




```output2
1
```



## Note

<p>In the first sample test, we can choose an upper poster with area $12$ and a lower poster of area $6$ as in the image below.</p><center> <img class="tex-graphics" src="file://FS0ynmLn.png" style="max-width: 100.0%;max-height: 100.0%;" width="265px"> </center><p>In the second sample test, we can cover the whole billboard using a single poster.</p>
