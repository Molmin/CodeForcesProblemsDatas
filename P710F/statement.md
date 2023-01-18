## Description

<div><p>You should process <span class="tex-span"><i>m</i></span> queries over a set <span class="tex-span"><i>D</i></span> of strings. Each query is one of three kinds:</p><ol> <li> Add a string <span class="tex-span"><i>s</i></span> to the set <span class="tex-span"><i>D</i></span>. It is guaranteed that the string <span class="tex-span"><i>s</i></span> was not added before. </li><li> Delete a string <span class="tex-span"><i>s</i></span> from the set <span class="tex-span"><i>D</i></span>. It is guaranteed that the string <span class="tex-span"><i>s</i></span> is in the set <span class="tex-span"><i>D</i></span>. </li><li> For the given string <span class="tex-span"><i>s</i></span> find the number of occurrences of the strings from the set <span class="tex-span"><i>D</i></span>. If some string <span class="tex-span"><i>p</i></span> from <span class="tex-span"><i>D</i></span> has several occurrences in <span class="tex-span"><i>s</i></span> you should count all of them. </li></ol><p>Note that you should solve the problem in <span class="tex-font-style-tt">online</span> mode. It means that you can't read the whole input at once. You can read each query only after writing the answer for the last query of the third type. Use functions <span class="tex-font-style-tt">fflush</span> in <span class="tex-font-style-tt">C++</span> and <span class="tex-font-style-tt">BufferedWriter.flush</span> in <span class="tex-font-style-tt">Java</span> languages after each writing in your program.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of queries.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 3</span>) and nonempty string <span class="tex-span"><i>s</i></span> — the kind of the query and the string to process. All strings consist of only lowercase English letters.</p><p>The sum of lengths of all strings in the input will not exceed <span class="tex-span">3·10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>For each query of the third kind print the only integer <span class="tex-span"><i>c</i></span> — the desired number of occurrences in the string <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of queries.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 3</span>) and nonempty string <span class="tex-span"><i>s</i></span> — the kind of the query and the string to process. All strings consist of only lowercase English letters.</p><p>The sum of lengths of all strings in the input will not exceed <span class="tex-span">3·10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>For each query of the third kind print the only integer <span class="tex-span"><i>c</i></span> — the desired number of occurrences in the string <span class="tex-span"><i>s</i></span>.</p>





```input1
5
1 abc
3 abcabc
2 abc
1 aba
3 abababc

```




```input2
10
1 abc
1 bcd
1 abcd
3 abcd
2 abcd
3 abcd
2 bcd
3 abcd
2 abc
3 abcd

```




```output1
2
2

```




```output2
3
2
1
0

```


