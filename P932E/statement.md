## Description

<div><p>You have a team of <span class="tex-span"><i>N</i></span> people. For a particular task, you can pick any non-empty subset of people. The cost of having <span class="tex-span"><i>x</i></span> people for the task is <span class="tex-span"><i>x</i><sup class="upper-index"><i>k</i></sup></span>. </p><p>Output the sum of costs over all non-empty subsets of people.</p></div><div class="input-specification"><p>Only line of input contains two integers <span class="tex-span"><i>N</i></span> <span class="tex-span">(1 ≤ <i>N</i> ≤ 10<sup class="upper-index">9</sup>)</span> representing total number of people and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 5000)</span>.</p></div><div class="output-specification"><p>Output the sum of costs for all non empty subsets modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>Only line of input contains two integers <span class="tex-span"><i>N</i></span> <span class="tex-span">(1 ≤ <i>N</i> ≤ 10<sup class="upper-index">9</sup>)</span> representing total number of people and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 5000)</span>.</p>

## Output

<p>Output the sum of costs for all non empty subsets modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
1 1

```




```input2
3 2

```




```output1
1

```




```output2
24

```



## Note

<p>In the first example, there is only one non-empty subset <span class="tex-span">{1}</span> with cost <span class="tex-span">1<sup class="upper-index">1</sup> = 1</span>.</p><p>In the second example, there are seven non-empty subsets.</p><p>- <span class="tex-span">{1}</span> with cost <span class="tex-span">1<sup class="upper-index">2</sup> = 1</span></p><p>- <span class="tex-span">{2}</span> with cost <span class="tex-span">1<sup class="upper-index">2</sup> = 1</span></p><p>- <span class="tex-span">{1, 2}</span> with cost <span class="tex-span">2<sup class="upper-index">2</sup> = 4</span></p><p>- <span class="tex-span">{3}</span> with cost <span class="tex-span">1<sup class="upper-index">2</sup> = 1</span></p><p>- <span class="tex-span">{1, 3}</span> with cost <span class="tex-span">2<sup class="upper-index">2</sup> = 4</span></p><p>- <span class="tex-span">{2, 3}</span> with cost <span class="tex-span">2<sup class="upper-index">2</sup> = 4</span></p><p>- <span class="tex-span">{1, 2, 3}</span> with cost <span class="tex-span">3<sup class="upper-index">2</sup> = 9</span></p><p>The total cost is <span class="tex-span">1 + 1 + 4 + 1 + 4 + 4 + 9 = 24</span>.</p>
