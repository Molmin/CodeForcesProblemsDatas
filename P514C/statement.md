## Description

<div><p>Watto, the owner of a spare parts store, has recently got an order for the mechanism that can process strings in a certain way. Initially the memory of the mechanism is filled with <span class="tex-span"><i>n</i></span> strings. Then the mechanism should be able to process queries of the following type: "Given string <span class="tex-span"><i>s</i></span>, determine if the memory of the mechanism contains string <span class="tex-span"><i>t</i></span> that consists of the same number of characters as <span class="tex-span"><i>s</i></span> and differs from <span class="tex-span"><i>s</i></span> in exactly one position".</p><p>Watto has already compiled the mechanism, all that's left is to write a program for it and check it on the data consisting of <span class="tex-span"><i>n</i></span> initial lines and <span class="tex-span"><i>m</i></span> queries. He decided to entrust this job to you.</p></div><div class="input-specification"><p>The first line contains two non-negative numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of the initial strings and the number of queries, respectively.</p><p>Next follow <span class="tex-span"><i>n</i></span> non-empty strings that are uploaded to the memory of the mechanism.</p><p>Next follow <span class="tex-span"><i>m</i></span> non-empty strings that are the queries to the mechanism.</p><p>The total length of lines in the input doesn't exceed <span class="tex-span">6·10<sup class="upper-index">5</sup></span>. Each line consists <span class="tex-font-style-bf">only</span> of letters <span class="tex-font-style-tt">'a'</span>, <span class="tex-font-style-tt">'b'</span>, <span class="tex-font-style-tt">'c'</span>.</p></div><div class="output-specification"><p>For each query print on a single line "<span class="tex-font-style-tt">YES</span>" (without the quotes), if the memory of the mechanism contains the required string, otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first line contains two non-negative numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of the initial strings and the number of queries, respectively.</p><p>Next follow <span class="tex-span"><i>n</i></span> non-empty strings that are uploaded to the memory of the mechanism.</p><p>Next follow <span class="tex-span"><i>m</i></span> non-empty strings that are the queries to the mechanism.</p><p>The total length of lines in the input doesn't exceed <span class="tex-span">6·10<sup class="upper-index">5</sup></span>. Each line consists <span class="tex-font-style-bf">only</span> of letters <span class="tex-font-style-tt">'a'</span>, <span class="tex-font-style-tt">'b'</span>, <span class="tex-font-style-tt">'c'</span>.</p>

## Output

<p>For each query print on a single line "<span class="tex-font-style-tt">YES</span>" (without the quotes), if the memory of the mechanism contains the required string, otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
2 3
aaaaa
acacaca
aabaa
ccacacc
caaac

```




```output1
YES
NO
NO

```


