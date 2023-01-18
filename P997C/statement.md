## Description

<div><p>On one of the planets of Solar system, in Atmosphere University, many students are fans of bingo game.</p><p>It is well known that one month on this planet consists of $n^2$ days, so calendars, represented as square matrix $n$ by $n$ are extremely popular.</p><p>Weather conditions are even more unusual. Due to the unique composition of the atmosphere, when interacting with sunlight, every day sky takes one of three colors: blue, green or red.</p><p>To play the bingo, you need to observe the sky for one month&nbsp;— after each day, its cell is painted with the color of the sky in that day, that is, blue, green or red.</p><p>At the end of the month, students examine the calendar. If at least one row or column contains only cells of one color, that month is called lucky.</p><p>Let's call two colorings of calendar different, if at least one cell has different colors in them. It is easy to see that there are $3^{n \cdot n}$ different colorings. How much of them are lucky? Since this number can be quite large, print it modulo $998244353$.</p></div><div class="input-specification"><p>The first and only line of input contains a single integer $n$ ($1 \le n \le 1000\,000$)&nbsp;— the number of rows and columns in the calendar.</p></div><div class="output-specification"><p>Print one number&nbsp;— number of lucky colorings of the calendar modulo $998244353$</p></div>

## Input

<p>The first and only line of input contains a single integer $n$ ($1 \le n \le 1000\,000$)&nbsp;— the number of rows and columns in the calendar.</p>

## Output

<p>Print one number&nbsp;— number of lucky colorings of the calendar modulo $998244353$</p>





```input1
1

```




```input2
2

```




```input3
3

```




```output1
3

```




```output2
63

```




```output3
9933

```



## Note

<p>In the first sample any coloring is lucky, since the only column contains cells of only one color.</p><p>In the second sample, there are a lot of lucky colorings, in particular, the following colorings are lucky:</p><center> <img class="tex-graphics" src="file://kKixkWDe.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>While these colorings are not lucky:</p><center> <img class="tex-graphics" src="file://bLLhJ1cT.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
