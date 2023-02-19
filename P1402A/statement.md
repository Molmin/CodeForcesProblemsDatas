## Description

<div><p>Everybody knows that Balázs has the fanciest fence in the whole town. It's built up from $N$ fancy sections. The sections are rectangles standing closely next to each other on the ground. The $i$th section has integer height $h_i$ and integer width $w_i$.  We are looking for fancy rectangles on this fancy fence.  A rectangle is fancy if: </p><ul> <li> its sides are either horizontal or vertical and have integer lengths </li><li> the distance between the rectangle and the ground is integer </li><li> the distance between the rectangle and the left side of the first section is integer </li><li> it's lying completely on sections </li></ul> What is the number of fancy rectangles?  This number can be very big, so we are interested in it modulo $10^9+7$.</div><div class="input-specification"><p>The first line contains $N$ ($1\leq N \leq 10^{5}$) – the number of sections.  The second line contains $N$ space-separated integers, the $i$th number is $h_i$ ($1 \leq h_i \leq 10^{9}$).  The third line contains $N$ space-separated integers, the $i$th number is $w_i$ ($1 \leq w_i \leq 10^{9}$).</p></div><div class="output-specification"><p>You should print a single integer, the number of fancy rectangles modulo $10^9+7$. So the output range is $0,1,2,\ldots, 10^9+6$.</p></div><div><h2>Scoring</h2><center> $ \begin{array}{|c|c|c|} \hline \text{Subtask} &amp; \text{Points} &amp; \text{Constraints} \\ \hline 1 &amp; 0 &amp; \text{sample}\\ \hline 2 &amp; 12 &amp; N \leq 50 \: \text{and} \: h_i \leq 50 \: \text{and} \: w_i = 1 \: \text{for all} \: i \\ \hline 3 &amp; 13 &amp; h_i = 1 \: \text{or} \: h_i = 2 \: \text{for all} \: i \\ \hline 4 &amp; 15 &amp; \text{all} \: h_i \: \text{are equal} \\ \hline 5 &amp; 15 &amp; h_i \leq h_{i+1} \: \text{for all} \: i \leq N-1 \\ \hline 6 &amp; 18 &amp; N \leq 1000\\ \hline 7 &amp; 27 &amp; \text{no additional constraints}\\ \hline \end{array} $</center></div>

## Input

<p>The first line contains $N$ ($1\leq N \leq 10^{5}$) – the number of sections.  The second line contains $N$ space-separated integers, the $i$th number is $h_i$ ($1 \leq h_i \leq 10^{9}$).  The third line contains $N$ space-separated integers, the $i$th number is $w_i$ ($1 \leq w_i \leq 10^{9}$).</p>

## Output

<p>You should print a single integer, the number of fancy rectangles modulo $10^9+7$. So the output range is $0,1,2,\ldots, 10^9+6$.</p>





```input1
2
1 2
1 2
```




```output1
12
```



## Note

<p>The fence looks like this:  <img class="tex-graphics" height="189px" src="file://bOc2aBWi.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>There are 5 fancy rectangles of shape:  <img class="tex-graphics" height="49px" src="file://SamhJIr8.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>There are 3 fancy rectangles of shape:  <img class="tex-graphics" height="49px" src="file://t4dfMBCD.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>There is 1 fancy rectangle of shape:  <img class="tex-graphics" height="49px" src="file://VKO680qO.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>There are 2 fancy rectangles of shape:  <img class="tex-graphics" height="76px" src="file://i25cFtVS.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>There is 1 fancy rectangle of shape:  <img class="tex-graphics" height="76px" src="file://AjWWrcUd.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
