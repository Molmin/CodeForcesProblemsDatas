## Description

<div><p>John Doe has a list of all Fibonacci numbers modulo <span class="tex-span">10<sup class="upper-index">13</sup></span>. This list is infinite, it starts with numbers <span class="tex-span">0</span> and <span class="tex-span">1</span>. Each number in the list, apart from the first two, is a sum of previous two modulo <span class="tex-span">10<sup class="upper-index">13</sup></span>. That is, John's list is made from the Fibonacci numbers' list by replacing each number there by the remainder when divided by <span class="tex-span">10<sup class="upper-index">13</sup></span>. </p><p>John got interested in number <span class="tex-span"><i>f</i></span> (<span class="tex-span">0 ≤ <i>f</i> &lt; 10<sup class="upper-index">13</sup></span>) and now wants to find its first occurrence in the list given above. Help John and find the number of the first occurence of number <span class="tex-span"><i>f</i></span> in the list or otherwise state that number <span class="tex-span"><i>f</i></span> does not occur in the list. </p><p>The numeration in John's list starts from zero. There, the <span class="tex-span">0</span>-th position is the number <span class="tex-span">0</span>, the <span class="tex-span">1</span>-st position is the number <span class="tex-span">1</span>, the <span class="tex-span">2</span>-nd position is the number <span class="tex-span">1</span>, the <span class="tex-span">3</span>-rd position is the number <span class="tex-span">2</span>, the <span class="tex-span">4</span>-th position is the number <span class="tex-span">3</span> and so on. Thus, the beginning of the list looks like this: <span class="tex-span">0, 1, 1, 2, 3, 5, 8, 13, 21, ...</span></p></div><div class="input-specification"><p>The first line contains the single integer <span class="tex-span"><i>f</i></span> (<span class="tex-span">0 ≤ <i>f</i> &lt; 10<sup class="upper-index">13</sup></span>) — the number, which position in the list we should find.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p></div><div class="output-specification"><p>Print a single number — the number of the first occurrence of the given number in John's list. If this number doesn't occur in John's list, print -1.</p></div>

## Input

<p>The first line contains the single integer <span class="tex-span"><i>f</i></span> (<span class="tex-span">0 ≤ <i>f</i> &lt; 10<sup class="upper-index">13</sup></span>) — the number, which position in the list we should find.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p>

## Output

<p>Print a single number — the number of the first occurrence of the given number in John's list. If this number doesn't occur in John's list, print -1.</p>





```input1
13

```




```input2
377

```




```output1
7

```




```output2
14

```


