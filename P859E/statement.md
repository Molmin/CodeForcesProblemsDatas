## Description

<div><p>A new set of desks just arrived, and it's about time! Things were getting quite cramped in the office. You've been put in charge of creating a new seating chart for the engineers. The desks are numbered, and you sent out a survey to the engineering team asking each engineer the number of the desk they currently sit at, and the number of the desk they would like to sit at (which may be the same as their current desk). Each engineer must either remain where they sit, or move to the desired seat they indicated in the survey. No two engineers currently sit at the same desk, nor may any two engineers sit at the same desk in the new seating arrangement.</p><p>How many seating arrangements can you create that meet the specified requirements? The answer may be very large, so compute it modulo <span class="tex-span">1000000007 = 10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>Input will begin with a line containing <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 100000</span>), the number of engineers. </p><p><span class="tex-span"><i>N</i></span> lines follow, each containing exactly two integers. The <span class="tex-span"><i>i</i></span>-th line contains the number of the current desk of the <span class="tex-span"><i>i</i></span>-th engineer and the number of the desk the <span class="tex-span"><i>i</i></span>-th engineer wants to move to. Desks are numbered from <span class="tex-span">1</span> to <span class="tex-span">2·<i>N</i></span>. It is guaranteed that no two engineers sit at the same desk.</p></div><div class="output-specification"><p>Print the number of possible assignments, modulo <span class="tex-span">1000000007 = 10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>Input will begin with a line containing <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 100000</span>), the number of engineers. </p><p><span class="tex-span"><i>N</i></span> lines follow, each containing exactly two integers. The <span class="tex-span"><i>i</i></span>-th line contains the number of the current desk of the <span class="tex-span"><i>i</i></span>-th engineer and the number of the desk the <span class="tex-span"><i>i</i></span>-th engineer wants to move to. Desks are numbered from <span class="tex-span">1</span> to <span class="tex-span">2·<i>N</i></span>. It is guaranteed that no two engineers sit at the same desk.</p>

## Output

<p>Print the number of possible assignments, modulo <span class="tex-span">1000000007 = 10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
4
1 5
5 2
3 7
7 3

```




```input2
5
1 10
2 10
3 10
4 10
5 5

```




```output1
6

```




```output2
5

```



## Note

<p>These are the possible assignments for the first example: </p><ul> <li> 1 5 3 7 </li><li> 1 2 3 7 </li><li> 5 2 3 7 </li><li> 1 5 7 3 </li><li> 1 2 7 3 </li><li> 5 2 7 3 </li></ul>
