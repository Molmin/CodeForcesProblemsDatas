## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers. Everybody knows that lucky numbers are positive integers whose decimal representation contains only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Petya has an array consisting of <span class="tex-span"><i>n</i></span> numbers. He wants to perform <span class="tex-span"><i>m</i></span> operations of two types: </p><ul> <li> <span class="tex-font-style-underline">add <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>d</i></span></span> — add an integer <span class="tex-span"><i>d</i></span> to all elements whose indexes belong to the interval from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>, inclusive <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>, 1 ≤ <i>d</i> ≤ 10<sup class="upper-index">4</sup>)</span>; </li><li> <span class="tex-font-style-underline">count <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span></span> — find and print on the screen how many lucky numbers there are among elements with indexes that belong to the interval from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> inclusive <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span>. Each lucky number should be counted as many times as it appears in the interval. </li></ul><p>Petya has a list of all operations. The operations are such that after all additions the array won't have numbers that would exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>. Help Petya write a program that would perform these operations.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of numbers in the array and the number of operations correspondingly. The second line contains <span class="tex-span"><i>n</i></span> positive integers, none of which exceeds <span class="tex-span">10<sup class="upper-index">4</sup></span> — those are the array numbers. Next <span class="tex-span"><i>m</i></span> lines contain operations, one per line. They correspond to the description given in the statement.</p><p>It is guaranteed that after all operations are fulfilled each number in the array will not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p></div><div class="output-specification"><p>For each operation of the second type print the single number on the single line — the number of lucky numbers in the corresponding interval.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of numbers in the array and the number of operations correspondingly. The second line contains <span class="tex-span"><i>n</i></span> positive integers, none of which exceeds <span class="tex-span">10<sup class="upper-index">4</sup></span> — those are the array numbers. Next <span class="tex-span"><i>m</i></span> lines contain operations, one per line. They correspond to the description given in the statement.</p><p>It is guaranteed that after all operations are fulfilled each number in the array will not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p>

## Output

<p>For each operation of the second type print the single number on the single line — the number of lucky numbers in the corresponding interval.</p>





```input1
3 6
2 3 4
count 1 3
count 1 2
add 1 3 2
count 1 3
add 2 3 3
count 1 3

```




```input2
4 5
4 4 4 4
count 1 4
add 1 4 3
count 1 4
add 2 3 40
count 1 4

```




```output1
1
0
1
1

```




```output2
4
4
4

```



## Note

<p>In the first sample after the first addition the array will look in the following manner:</p><p><span class="tex-font-style-tt">4 5 6</span></p><p>After the second addition:</p><p><span class="tex-font-style-tt">4 8 9</span></p><p>The second sample after the first addition:</p><p><span class="tex-font-style-tt">7 7 7 7</span></p><p>After the second addition:</p><p><span class="tex-font-style-tt">7 47 47 7</span></p>
