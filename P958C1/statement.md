## Description

<div><p>Rebel spy Heidi has just obtained the plans for the Death Star from the Empire and, now on her way to safety, she is trying to break the encryption of the plans (of course they are encrypted – the Empire may be evil, but it is not stupid!). The encryption has several levels of security, and here is how the first one looks.</p><p>Heidi is presented with a screen that shows her a sequence of integers <span class="tex-span"><i>A</i></span> and a positive integer <span class="tex-span"><i>p</i></span>. She knows that the encryption code is a single number <span class="tex-span"><i>S</i></span>, which is defined as follows:</p><p>Define the <span class="tex-font-style-underline">score</span> of <span class="tex-span"><i>X</i></span> to be the sum of the elements of <span class="tex-span"><i>X</i></span> modulo <span class="tex-span"><i>p</i></span>.</p><p>Heidi is given a sequence <span class="tex-span"><i>A</i></span> that consists of <span class="tex-span"><i>N</i></span> integers, and also given an integer <span class="tex-span"><i>p</i></span>. She needs to split <span class="tex-span"><i>A</i></span> into <span class="tex-span">2</span> parts such that: </p><ul> <li> Each part contains at least <span class="tex-span">1</span> element of <span class="tex-span"><i>A</i></span>, and each part consists of contiguous elements of <span class="tex-span"><i>A</i></span>. </li><li> The two parts do not overlap. </li><li> The total sum <span class="tex-span"><i>S</i></span> of the scores of those two parts is maximized. This is the encryption code. </li></ul><p>Output the sum <span class="tex-span"><i>S</i></span>, which is the encryption code.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integer <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">2 ≤ <i>N</i> ≤ 100 000</span>, <span class="tex-span">2 ≤ <i>p</i> ≤ 10 000</span>) – the number of elements in <span class="tex-span"><i>A</i></span>, and the modulo for computing scores, respectively.</p><p>The second line contains <span class="tex-span"><i>N</i></span> space-separated integers which are the elements of <span class="tex-span"><i>A</i></span>. Each integer is from the interval <span class="tex-span">[1, 1 000 000]</span>.</p></div><div class="output-specification"><p>Output the number <span class="tex-span"><i>S</i></span> as described in the problem statement.</p></div>

## Input

<p>The first line of the input contains two space-separated integer <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">2 ≤ <i>N</i> ≤ 100 000</span>, <span class="tex-span">2 ≤ <i>p</i> ≤ 10 000</span>) – the number of elements in <span class="tex-span"><i>A</i></span>, and the modulo for computing scores, respectively.</p><p>The second line contains <span class="tex-span"><i>N</i></span> space-separated integers which are the elements of <span class="tex-span"><i>A</i></span>. Each integer is from the interval <span class="tex-span">[1, 1 000 000]</span>.</p>

## Output

<p>Output the number <span class="tex-span"><i>S</i></span> as described in the problem statement.</p>





```input1
4 10
3 4 7 2

```




```input2
10 12
16 3 24 13 9 8 7 5 12 12

```




```output1
16

```




```output2
13

```



## Note

<p>In the first example, the score is maximized if the input sequence is split into two parts as <span class="tex-span">(3, 4)</span>, <span class="tex-span">(7, 2)</span>. It gives the total score of <img align="middle" class="tex-formula" src="file://xTGk3KXe.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second example, the score is maximized if the first part consists of the first three elements, and the second part consists of the rest. Then, the score is <img align="middle" class="tex-formula" src="file://Dv17ZuFV.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
