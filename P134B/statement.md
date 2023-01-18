## Description

<div><p>Let's assume that we have a pair of numbers (<span class="tex-span"><i>a</i>, <i>b</i></span>). We can get a new pair (<span class="tex-span"><i>a</i> + <i>b</i>, <i>b</i></span>) or (<span class="tex-span"><i>a</i>, <i>a</i> + <i>b</i></span>) from the given pair in a single step.</p><p>Let the initial pair of numbers be (1,1). Your task is to find number <span class="tex-span"><i>k</i></span>, that is, the least number of steps needed to transform (1,1) into the pair where at least one number equals <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The input contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>k</i></span>.</p></div>

## Input

<p>The input contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>Print the only integer <span class="tex-span"><i>k</i></span>.</p>





```input1
5

```




```input2
1

```




```output1
3

```




```output2
0

```



## Note

<p>The pair (1,1) can be transformed into a pair containing 5 in three moves: (1,1) <span class="tex-span"> → </span> (1,2) <span class="tex-span"> → </span> (3,2) <span class="tex-span"> → </span> (5,2).</p>
