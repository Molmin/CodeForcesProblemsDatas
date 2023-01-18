## Description

<div><p>You are given string <span class="tex-span"><i>s</i></span>. Your task is to determine if the given string <span class="tex-span"><i>s</i></span> contains two non-overlapping substrings "<span class="tex-font-style-tt">AB</span>" and "<span class="tex-font-style-tt">BA</span>" (the substrings can go in any order).</p></div><div class="input-specification"><p>The only line of input contains a string <span class="tex-span"><i>s</i></span> of length between <span class="tex-span">1</span> and <span class="tex-span">10<sup class="upper-index">5</sup></span> consisting of uppercase Latin letters.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if string <span class="tex-span"><i>s</i></span> contains two non-overlapping substrings "<span class="tex-font-style-tt">AB</span>" and "<span class="tex-font-style-tt">BA</span>", and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The only line of input contains a string <span class="tex-span"><i>s</i></span> of length between <span class="tex-span">1</span> and <span class="tex-span">10<sup class="upper-index">5</sup></span> consisting of uppercase Latin letters.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if string <span class="tex-span"><i>s</i></span> contains two non-overlapping substrings "<span class="tex-font-style-tt">AB</span>" and "<span class="tex-font-style-tt">BA</span>", and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
ABA

```




```input2
BACFAB

```




```input3
AXBYBXA

```




```output1
NO

```




```output2
YES

```




```output3
NO

```



## Note

<p>In the first sample test, despite the fact that there are substrings "<span class="tex-font-style-tt">AB</span>" and "<span class="tex-font-style-tt">BA</span>", their occurrences overlap, so the answer is "<span class="tex-font-style-tt">NO</span>".</p><p>In the second sample test there are the following occurrences of the substrings: <span class="tex-font-style-bf">BA</span>CF<span class="tex-font-style-bf">AB</span>.</p><p>In the third sample test there is no substring "<span class="tex-font-style-tt">AB</span>" nor substring "<span class="tex-font-style-tt">BA</span>".</p>
