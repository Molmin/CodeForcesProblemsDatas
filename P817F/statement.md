## Description

<div><p>You are given a set of integer numbers, initially it is empty. You should perform <span class="tex-span"><i>n</i></span> queries.</p><p>There are three different types of queries: </p><ul> <li> <span class="tex-font-style-tt">1</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> — Add all missing numbers from the interval <span class="tex-span">[<i>l</i>, <i>r</i>]</span> </li><li> <span class="tex-font-style-tt">2</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> — Remove all present numbers from the interval <span class="tex-span">[<i>l</i>, <i>r</i>]</span> </li><li> <span class="tex-font-style-tt">3</span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> — Invert the interval <span class="tex-span">[<i>l</i>, <i>r</i>]</span> — add all missing and remove all present numbers from the interval <span class="tex-span">[<i>l</i>, <i>r</i>]</span> </li></ul><p>After each query you should output <span class="tex-font-style-it">MEX</span> of the set — the smallest positive (<span class="tex-font-style-it">MEX</span> <span class="tex-span"> ≥ 1</span>) integer number which is not presented in the set.</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain three integer numbers <span class="tex-span"><i>t</i>, <i>l</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 3, 1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>) — type of the query, left and right bounds.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-it">MEX</span> of the set after each query.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain three integer numbers <span class="tex-span"><i>t</i>, <i>l</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 3, 1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>) — type of the query, left and right bounds.</p>

## Output

<p>Print <span class="tex-font-style-it">MEX</span> of the set after each query.</p>





```input1
3
1 3 4
3 1 6
2 1 3

```




```input2
4
1 1 3
3 5 6
2 4 4
3 1 6

```




```output1
1
3
1

```




```output2
4
4
4
1

```



## Note

<p>Here are contents of the set after each query in the first example:</p><ol> <li> <span class="tex-span">{3, 4}</span> — the interval <span class="tex-span">[3, 4]</span> is added </li><li> <span class="tex-span">{1, 2, 5, 6}</span> — numbers <span class="tex-span">{3, 4}</span> from the interval <span class="tex-span">[1, 6]</span> got deleted and all the others are added </li><li> <span class="tex-span">{5, 6}</span> — numbers <span class="tex-span">{1, 2}</span> got deleted </li></ol>
