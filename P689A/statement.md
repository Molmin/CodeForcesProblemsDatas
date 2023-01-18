## Description

<div><p>While swimming at the beach, Mike has accidentally dropped his cellphone into the water. There was no worry as he bought a cheap replacement phone with an old-fashioned keyboard. The keyboard has only ten digital equal-sized keys, located in the following way:</p><center> <img align="middle" class="tex-formula" src="file://RdSKPLeo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Together with his old phone, he lost all his contacts and now he can only remember the way his fingers moved when he put some number in. One can formally consider <span class="tex-font-style-it">finger movements</span> as a sequence of vectors connecting centers of keys pressed consecutively to put in a number. For example, the finger movements for number "586" are the same as finger movements for number "253":</p><center> <img class="tex-graphics" src="file://qDftKLmj.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><center> <img class="tex-graphics" src="file://nAqxfLIX.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Mike has already put in a number by his "finger memory" and started calling it, so he is now worrying, can he be sure that he is calling the correct number? In other words, is there any other number, that has the same finger movements?</p></div><div class="input-specification"><p>The first line of the input contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 9</span>)&nbsp;— the number of digits in the phone number that Mike put in.</p><p>The second line contains the string consisting of <span class="tex-span"><i>n</i></span> digits (characters from '<span class="tex-font-style-tt">0</span>' to '<span class="tex-font-style-tt">9</span>') representing the number that Mike put in.</p></div><div class="output-specification"><p>If there is no other phone number with the same finger movements and Mike can be sure he is calling the correct number, print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the only line.</p><p>Otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes) in the first line.</p></div>

## Input

<p>The first line of the input contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 9</span>)&nbsp;— the number of digits in the phone number that Mike put in.</p><p>The second line contains the string consisting of <span class="tex-span"><i>n</i></span> digits (characters from '<span class="tex-font-style-tt">0</span>' to '<span class="tex-font-style-tt">9</span>') representing the number that Mike put in.</p>

## Output

<p>If there is no other phone number with the same finger movements and Mike can be sure he is calling the correct number, print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the only line.</p><p>Otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes) in the first line.</p>





```input1
3
586

```




```input2
2
09

```




```input3
9
123456789

```




```input4
3
911

```




```output1
NO

```




```output2
NO

```




```output3
YES

```




```output4
YES

```



## Note

<p>You can find the picture clarifying the first sample case in the statement above.</p>
