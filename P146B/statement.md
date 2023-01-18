## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers very much. Everybody knows that lucky numbers are positive integers whose decimal record contains only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Petya calls a <span class="tex-font-style-underline">mask</span> of a positive integer <span class="tex-span"><i>n</i></span> the number that is obtained after successive writing of all lucky digits of number <span class="tex-span"><i>n</i></span> from the left to the right. For example, the mask of number <span class="tex-span">72174994</span> is number <span class="tex-span">7744</span>, the mask of <span class="tex-span">7</span> is <span class="tex-span">7</span>, the mask of <span class="tex-span">9999047</span> is <span class="tex-span">47</span>. Obviously, mask of any number is always a lucky number.</p><p>Petya has two numbers — an arbitrary integer <span class="tex-span"><i>a</i></span> and a lucky number <span class="tex-span"><i>b</i></span>. Help him find the minimum number <span class="tex-span"><i>c</i></span> <span class="tex-span">(<i>c</i> &gt; <i>a</i>)</span> such that the mask of number <span class="tex-span"><i>c</i></span> equals <span class="tex-span"><i>b</i></span>.</p></div><div class="input-specification"><p>The only line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">5</sup>)</span>. It is guaranteed that number <span class="tex-span"><i>b</i></span> is lucky.</p></div><div class="output-specification"><p>In the only line print a single number — the number <span class="tex-span"><i>c</i></span> that is sought by Petya.</p></div>

## Input

<p>The only line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">5</sup>)</span>. It is guaranteed that number <span class="tex-span"><i>b</i></span> is lucky.</p>

## Output

<p>In the only line print a single number — the number <span class="tex-span"><i>c</i></span> that is sought by Petya.</p>





```input1
1 7

```




```input2
100 47

```




```output1
7

```




```output2
147

```


