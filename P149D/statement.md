## Description

<div><p>Once Petya read a problem about a bracket sequence. He gave it much thought but didn't find a solution. Today you will face it.</p><p>You are given string <span class="tex-span"><i>s</i></span>. It represents a correct bracket sequence. A correct bracket sequence is the sequence of opening ("<span class="tex-font-style-tt">(</span>") and closing ("<span class="tex-font-style-tt">)</span>") brackets, such that it is possible to obtain a correct mathematical expression from it, inserting numbers and operators between the brackets. For example, such sequences as "<span class="tex-font-style-tt">(())()</span>" and "<span class="tex-font-style-tt">()</span>" are correct bracket sequences and such sequences as "<span class="tex-font-style-tt">)()</span>" and "<span class="tex-font-style-tt">(()</span>" are not.</p><p>In a correct bracket sequence each bracket corresponds to the matching bracket (an opening bracket corresponds to the matching closing bracket and vice versa). For example, in a bracket sequence shown of the figure below, the third bracket corresponds to the matching sixth one and the fifth bracket corresponds to the fourth one.</p><center> <img class="tex-graphics" src="file://ztknBUAp.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> <p>You are allowed to color some brackets in the bracket sequence so as all three conditions are fulfilled: </p><ul> <li> Each bracket is either not colored any color, or is colored red, or is colored blue. </li><li> For any pair of matching brackets exactly one of them is colored. In other words, for any bracket the following is true: either it or the matching bracket that corresponds to it is colored. </li><li> No two neighboring colored brackets have the same color. </li></ul><p>Find the number of different ways to color the bracket sequence. The ways should meet the above-given conditions. Two ways of coloring are considered different if they differ in the color of at least one bracket. As the result can be quite large, print it modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line contains the single string <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ |<i>s</i>| ≤ 700</span>) which represents a correct bracket sequence. </p></div><div class="output-specification"><p>Print the only number — the number of ways to color the bracket sequence that meet the above given conditions modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains the single string <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ |<i>s</i>| ≤ 700</span>) which represents a correct bracket sequence. </p>

## Output

<p>Print the only number — the number of ways to color the bracket sequence that meet the above given conditions modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
(())

```




```input2
(()())

```




```input3
()

```




```output1
12

```




```output2
40

```




```output3
4

```



## Note

<p>Let's consider the first sample test. The bracket sequence from the sample can be colored, for example, as is shown on two figures below. </p><center> <img class="tex-graphics" src="file://LTk23dbv.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://UkzsPF8w.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> <p>The two ways of coloring shown below are incorrect. </p><center> <img class="tex-graphics" src="file://f4F4ysvb.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://JtAf5DnG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
