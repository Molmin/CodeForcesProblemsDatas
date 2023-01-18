## Description

<div><p>There are <span class="tex-span"><i>n</i></span> piles of stones of sizes <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> lying on the table in front of you.</p><p>During one move you can take one pile and add it to the other. As you add pile <span class="tex-span"><i>i</i></span> to pile <span class="tex-span"><i>j</i></span>, the size of pile <span class="tex-span"><i>j</i></span> increases by the current size of pile <span class="tex-span"><i>i</i></span>, and pile <span class="tex-span"><i>i</i></span> stops existing. The cost of the adding operation equals the size of the added pile.</p><p>Your task is to determine the minimum cost at which you can gather all stones in one pile. </p><p>To add some challenge, the stone piles built up conspiracy and decided that each pile will let you add to it not more than <span class="tex-span"><i>k</i></span> times (after that it can only be added to another pile). </p><p>Moreover, the piles decided to puzzle you completely and told you <span class="tex-span"><i>q</i></span> variants (not necessarily distinct) of what <span class="tex-span"><i>k</i></span> might equal. </p><p>Your task is to find the minimum cost for each of <span class="tex-span"><i>q</i></span> variants.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of stone piles. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the initial sizes of the stone piles. </p><p>The third line contains integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. The last line contains <span class="tex-span"><i>q</i></span> space-separated integers <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>q</i></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the values of number <span class="tex-span"><i>k</i></span> for distinct queries. Note that numbers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> can repeat.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> whitespace-separated integers — the answers to the queries in the order, in which the queries are given in the input.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of stone piles. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the initial sizes of the stone piles. </p><p>The third line contains integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. The last line contains <span class="tex-span"><i>q</i></span> space-separated integers <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>q</i></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the values of number <span class="tex-span"><i>k</i></span> for distinct queries. Note that numbers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> can repeat.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> whitespace-separated integers — the answers to the queries in the order, in which the queries are given in the input.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
5
2 3 4 1 1
2
2 3

```




```output1
9 8
```



## Note

<p>In the first sample one way to get the optimal answer goes like this: we add in turns the <span class="tex-span">4</span>-th and the <span class="tex-span">5</span>-th piles to the <span class="tex-span">2</span>-nd one; then we add the <span class="tex-span">1</span>-st pile to the <span class="tex-span">3</span>-rd one; we add the <span class="tex-span">2</span>-nd pile to the <span class="tex-span">3</span>-rd one. The first two operations cost <span class="tex-span">1</span> each; the third one costs <span class="tex-span">2</span>, the fourth one costs <span class="tex-span">5</span> (the size of the <span class="tex-span">2</span>-nd pile after the first two operations is not <span class="tex-span">3</span>, it already is <span class="tex-span">5</span>). </p><p>In the second sample you can add the <span class="tex-span">2</span>-nd pile to the <span class="tex-span">3</span>-rd one (the operations costs <span class="tex-span">3</span>); then the <span class="tex-span">1</span>-st one to the <span class="tex-span">3</span>-th one (the cost is <span class="tex-span">2</span>); then the <span class="tex-span">5</span>-th one to the <span class="tex-span">4</span>-th one (the costs is <span class="tex-span">1</span>); and at last, the <span class="tex-span">4</span>-th one to the <span class="tex-span">3</span>-rd one (the cost is <span class="tex-span">2</span>).</p>
