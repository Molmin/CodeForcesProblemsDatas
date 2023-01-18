## Description

<div><p>As Sherlock Holmes was investigating another crime, he found a certain number of clues. Also, he has already found <span class="tex-font-style-underline">direct links</span> between some of those clues. The direct links between the clues are mutual. That is, the direct link between clues <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> and the direct link between clues <span class="tex-span"><i>B</i></span> and <span class="tex-span"><i>A</i></span> is the same thing. No more than one direct link can exist between two clues.</p><p>Of course Sherlock is able to find direct links between all clues. But it will take too much time and the criminals can use this extra time to hide. To solve the crime, Sherlock needs each clue to be linked to all other clues (maybe not directly, via some other clues). Clues <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> are considered linked either if there is a direct link between them or if there is a direct link between <span class="tex-span"><i>A</i></span> and some other clue <span class="tex-span"><i>C</i></span> which is linked to <span class="tex-span"><i>B</i></span>. </p><p>Sherlock Holmes counted the minimum number of additional direct links that he needs to find to solve the crime. As it turns out, it equals <span class="tex-span"><i>T</i></span>.</p><p>Please count the number of different ways to find exactly <span class="tex-span"><i>T</i></span> direct links between the clues so that the crime is solved in the end. Two ways to find direct links are considered different if there exist two clues which have a direct link in one way and do not have a direct link in the other way. </p><p>As the number of different ways can turn out rather big, print it modulo <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of clues, the number of direct clue links that Holmes has already found and the divisor for the modulo operation.</p><p>Each of next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>, <i>a</i> ≠ <i>b</i></span>), that represent a direct link between clues. It is guaranteed that any two clues are linked by no more than one direct link. Note that the direct links between the clues are mutual.</p></div><div class="output-specification"><p>Print the single number — the answer to the problem modulo <span class="tex-span"><i>k</i></span>.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of clues, the number of direct clue links that Holmes has already found and the divisor for the modulo operation.</p><p>Each of next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>, <i>a</i> ≠ <i>b</i></span>), that represent a direct link between clues. It is guaranteed that any two clues are linked by no more than one direct link. Note that the direct links between the clues are mutual.</p>

## Output

<p>Print the single number — the answer to the problem modulo <span class="tex-span"><i>k</i></span>.</p>





```input1
2 0 1000000000

```




```input2
3 0 100

```




```input3
4 1 1000000000
1 4

```




```output1
1

```




```output2
3

```




```output3
8

```



## Note

<p>The first sample only has two clues and Sherlock hasn't found any direct link between them yet. The only way to solve the crime is to find the link.</p><p>The second sample has three clues and Sherlock hasn't found any direct links between them. He has to find two of three possible direct links between clues to solve the crime — there are <span class="tex-span">3</span> ways to do it.</p><p>The third sample has four clues and the detective has already found one direct link between the first and the fourth clue. There are <span class="tex-span">8</span> ways to find two remaining clues to solve the crime.</p>
