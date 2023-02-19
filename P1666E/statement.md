## Description

<div><p>A revolution has recently happened in Segmentland. The new government is committed to equality, and they hired you to help with land redistribution in the country.</p><p>Segmentland is a segment of length $l$ kilometers, with the capital in one of its ends. There are $n$ citizens in Segmentland, the home of $i$-th citizen is located at the point $a_i$ kilometers from the capital. No two homes are located at the same point. Each citizen should receive a segment of positive length with ends at integer distances from the capital that contains her home. The union of these segments should be the&nbsp;whole of Segmentland, and they should not have common points besides their ends. To ensure equality, the difference between the lengths of the longest and the shortest segments should be as small as possible.</p></div><div class="input-specification"><p>The first line of the input contains two integers $l$ and $n$ ($2 \leq l \leq 10^9; 1 \leq n \leq 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 &lt; a_1 &lt; a_2 &lt; \dots &lt; a_n &lt; l$).</p></div><div class="output-specification"><p>Output $n$ pairs of numbers $s_i, f_i$ ($0 \leq s_i &lt; f_i \leq l$), one pair per line. The pair on $i$-th line denotes the&nbsp;ends of the $[s_i, f_i]$ segment that $i$-th citizen receives.</p><p>If there are many possible arrangements with the same difference between the lengths of the longest and the shortest segments, you can output any of them.</p></div>

## Input

<p>The first line of the input contains two integers $l$ and $n$ ($2 \leq l \leq 10^9; 1 \leq n \leq 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 &lt; a_1 &lt; a_2 &lt; \dots &lt; a_n &lt; l$).</p>

## Output

<p>Output $n$ pairs of numbers $s_i, f_i$ ($0 \leq s_i &lt; f_i \leq l$), one pair per line. The pair on $i$-th line denotes the&nbsp;ends of the $[s_i, f_i]$ segment that $i$-th citizen receives.</p><p>If there are many possible arrangements with the same difference between the lengths of the longest and the shortest segments, you can output any of them.</p>





```input1
6 3
1 3 5
```




```input2
10 2
1 2
```




```output1
0 2
2 4
4 6
```




```output2
0 2
2 10
```



## Note

<p>In the first example, it is possible to make all segments equal. <span class="tex-font-style-it">Viva la revolucion!</span></p><center> <img class="tex-graphics" src="file://RUOZdhhD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, citizens live close to the capital, so the length of the shortest segment is 2 and the&nbsp;length of the longest segment is 8.</p><center> <img class="tex-graphics" src="file://GqhaPwKo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
