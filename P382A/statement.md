## Description

<div><p>Ksenia has ordinary pan scales and several weights of an equal mass. Ksenia has already put some weights on the scales, while other weights are untouched. Ksenia is now wondering whether it is possible to put all the remaining weights on the scales so that the scales were in equilibrium. </p><p>The scales is in equilibrium if the total sum of weights on the left pan is equal to the total sum of weights on the right pan.</p></div><div class="input-specification"><p>The first line has a non-empty sequence of characters describing the scales. In this sequence, an uppercase English letter indicates a weight, and the symbol "<span class="tex-font-style-tt">|</span>" indicates the delimiter (the character occurs in the sequence exactly once). All weights that are recorded in the sequence before the delimiter are initially on the left pan of the scale. All weights that are recorded in the sequence after the delimiter are initially on the right pan of the scale. </p><p>The second line contains a non-empty sequence containing uppercase English letters. Each letter indicates a weight which is not used yet. </p><p>It is guaranteed that all the English letters in the input data are different. It is guaranteed that the input does not contain any extra characters.</p></div><div class="output-specification"><p>If you cannot put all the weights on the scales so that the scales were in equilibrium, print string "<span class="tex-font-style-tt">Impossible</span>". Otherwise, print the description of the resulting scales, copy the format of the input.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line has a non-empty sequence of characters describing the scales. In this sequence, an uppercase English letter indicates a weight, and the symbol "<span class="tex-font-style-tt">|</span>" indicates the delimiter (the character occurs in the sequence exactly once). All weights that are recorded in the sequence before the delimiter are initially on the left pan of the scale. All weights that are recorded in the sequence after the delimiter are initially on the right pan of the scale. </p><p>The second line contains a non-empty sequence containing uppercase English letters. Each letter indicates a weight which is not used yet. </p><p>It is guaranteed that all the English letters in the input data are different. It is guaranteed that the input does not contain any extra characters.</p>

## Output

<p>If you cannot put all the weights on the scales so that the scales were in equilibrium, print string "<span class="tex-font-style-tt">Impossible</span>". Otherwise, print the description of the resulting scales, copy the format of the input.</p><p>If there are multiple answers, print any of them.</p>





```input1
AC|T
L

```




```input2
|ABC
XYZ

```




```input3
W|T
F

```




```input4
ABC|
D

```




```output1
AC|TL

```




```output2
XYZ|ABC

```




```output3
Impossible

```




```output4
Impossible

```


