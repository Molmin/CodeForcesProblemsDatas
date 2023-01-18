## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers very much. Everybody knows that lucky numbers are positive integers whose decimal record contains only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Petya has two strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> of the same length <span class="tex-span"><i>n</i></span>. The strings consist only of lucky digits. Petya can perform <span class="tex-font-style-underline">operations</span> of two types: </p><ul> <li> replace any one digit from string <span class="tex-span"><i>a</i></span> by its opposite (i.e., replace <span class="tex-span">4</span> by <span class="tex-span">7</span> and <span class="tex-span">7</span> by <span class="tex-span">4</span>); </li><li> swap any pair of digits in string <span class="tex-span"><i>a</i></span>. </li></ul><p>Petya is interested in the minimum number of operations that are needed to make string <span class="tex-span"><i>a</i></span> equal to string <span class="tex-span"><i>b</i></span>. Help him with the task.</p></div><div class="input-specification"><p>The first and the second line contains strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, correspondingly. Strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> have equal lengths and contain only lucky digits. The strings are not empty, their length does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Print on the single line the single number — the minimum number of operations needed to convert string <span class="tex-span"><i>a</i></span> into string <span class="tex-span"><i>b</i></span>.</p></div>

## Input

<p>The first and the second line contains strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, correspondingly. Strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> have equal lengths and contain only lucky digits. The strings are not empty, their length does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Print on the single line the single number — the minimum number of operations needed to convert string <span class="tex-span"><i>a</i></span> into string <span class="tex-span"><i>b</i></span>.</p>





```input1
47
74

```




```input2
774
744

```




```input3
777
444

```




```output1
1

```




```output2
1

```




```output3
3

```



## Note

<p>In the first sample it is enough simply to swap the first and the second digit.</p><p>In the second sample we should replace the second digit with its opposite.</p><p>In the third number we should replace all three digits with their opposites.</p>
