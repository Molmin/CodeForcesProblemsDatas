## Description

<div><p>Codehorses has just hosted the second Codehorses Cup. This year, the same as the previous one, organizers are giving T-shirts for the winners.</p><p>The valid sizes of T-shirts are either <span class="tex-font-style-tt">"M"</span> or from $0$ to $3$ <span class="tex-font-style-tt">"X"</span> followed by <span class="tex-font-style-tt">"S"</span> or <span class="tex-font-style-tt">"L"</span>. For example, sizes <span class="tex-font-style-tt">"M"</span>, <span class="tex-font-style-tt">"XXS"</span>, <span class="tex-font-style-tt">"L"</span>, <span class="tex-font-style-tt">"XXXL"</span> are valid and <span class="tex-font-style-tt">"XM"</span>, <span class="tex-font-style-tt">"Z"</span>, <span class="tex-font-style-tt">"XXXXL"</span> are not.</p><p>There are $n$ winners to the cup for both the previous year and the current year. Ksenia has a list with the T-shirt sizes printed for the last year cup and is yet to send the new list to the printing office. </p><p>Organizers want to distribute the prizes as soon as possible, so now Ksenia is required not to write the whole list from the scratch but just make some changes to the list of the previous year. In one second she can choose arbitrary position in any word and replace its character with some uppercase Latin letter. Ksenia can't remove or add letters in any of the words.</p><p>What is the minimal number of seconds Ksenia is required to spend to change the last year list to the current one?</p><p><span class="tex-font-style-it">The lists are unordered</span>. That means, two lists are considered equal if and only if the number of occurrences of any string is the same in both lists.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 100$) — the number of T-shirts.</p><p>The $i$-th of the next $n$ lines contains $a_i$ — the size of the $i$-th T-shirt of the list for the previous year.</p><p>The $i$-th of the next $n$ lines contains $b_i$ — the size of the $i$-th T-shirt of the list for the current year.</p><p>It is guaranteed that all the sizes in the input are valid. It is also guaranteed that Ksenia can produce list $b$ from the list $a$.</p></div><div class="output-specification"><p>Print the minimal number of seconds Ksenia is required to spend to change the last year list to the current one. If the lists are already equal, print <span class="tex-font-style-tt">0</span>.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 100$) — the number of T-shirts.</p><p>The $i$-th of the next $n$ lines contains $a_i$ — the size of the $i$-th T-shirt of the list for the previous year.</p><p>The $i$-th of the next $n$ lines contains $b_i$ — the size of the $i$-th T-shirt of the list for the current year.</p><p>It is guaranteed that all the sizes in the input are valid. It is also guaranteed that Ksenia can produce list $b$ from the list $a$.</p>

## Output

<p>Print the minimal number of seconds Ksenia is required to spend to change the last year list to the current one. If the lists are already equal, print <span class="tex-font-style-tt">0</span>.</p>





```input1
3
XS
XS
M
XL
S
XS

```




```input2
2
XXXL
XXL
XXL
XXXS

```




```input3
2
M
XS
XS
M

```




```output1
2

```




```output2
1

```




```output3
0

```



## Note

<p>In the first example Ksenia can replace <span class="tex-font-style-tt">"M"</span> with <span class="tex-font-style-tt">"S"</span> and <span class="tex-font-style-tt">"S"</span> in one of the occurrences of <span class="tex-font-style-tt">"XS"</span> with <span class="tex-font-style-tt">"L"</span>.</p><p>In the second example Ksenia should replace <span class="tex-font-style-tt">"L"</span> in <span class="tex-font-style-tt">"XXXL"</span> with <span class="tex-font-style-tt">"S"</span>.</p><p>In the third example lists are equal.</p>
