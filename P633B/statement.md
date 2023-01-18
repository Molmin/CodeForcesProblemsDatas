## Description

<div><p>Mr. Santa asks all the great programmers of the world to solve a trivial problem. He gives them an integer <span class="tex-span"><i>m</i></span> and asks for the number of positive integers <span class="tex-span"><i>n</i></span>, such that the factorial of <span class="tex-span"><i>n</i></span> ends with exactly <span class="tex-span"><i>m</i></span> zeroes. Are you among those great programmers who can solve this problem?</p></div><div class="input-specification"><p>The only line of input contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the required number of trailing zeroes in factorial.</p></div><div class="output-specification"><p>First print <span class="tex-span"><i>k</i></span>&nbsp;— the number of values of <span class="tex-span"><i>n</i></span> such that the factorial of <span class="tex-span"><i>n</i></span> ends with <span class="tex-span"><i>m</i></span> zeroes. Then print these <span class="tex-span"><i>k</i></span> integers in increasing order.</p></div>

## Input

<p>The only line of input contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the required number of trailing zeroes in factorial.</p>

## Output

<p>First print <span class="tex-span"><i>k</i></span>&nbsp;— the number of values of <span class="tex-span"><i>n</i></span> such that the factorial of <span class="tex-span"><i>n</i></span> ends with <span class="tex-span"><i>m</i></span> zeroes. Then print these <span class="tex-span"><i>k</i></span> integers in increasing order.</p>





```input1
1

```




```input2
5

```




```output1
5
5 6 7 8 9
```




```output2
0
```



## Note

<p>The factorial of <span class="tex-span"><i>n</i></span> is equal to the product of all integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> inclusive, that is <span class="tex-span"><i>n</i>! = 1·2·3·...·<i>n</i></span>.</p><p>In the first sample, <span class="tex-span">5! = 120</span>, <span class="tex-span">6! = 720</span>, <span class="tex-span">7! = 5040</span>, <span class="tex-span">8! = 40320</span> and <span class="tex-span">9! = 362880</span>.</p>
