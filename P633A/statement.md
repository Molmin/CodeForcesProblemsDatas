## Description

<div><p>Dante is engaged in a fight with "The Savior". Before he can fight it with his sword, he needs to break its shields. He has two guns, Ebony and Ivory, each of them is able to perform any non-negative number of shots.</p><p>For every bullet that hits the shield, Ebony deals <span class="tex-span"><i>a</i></span> units of damage while Ivory deals <span class="tex-span"><i>b</i></span> units of damage. In order to break the shield Dante has to deal <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>c</i></span> units of damage. Find out if this is possible.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 100, 1 ≤ <i>c</i> ≤ 10 000</span>)&nbsp;— the number of units of damage dealt by Ebony gun and Ivory gun, and the total number of damage required to break the shield, respectively.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if Dante can deal exactly <span class="tex-span"><i>c</i></span> damage to the shield and "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 100, 1 ≤ <i>c</i> ≤ 10 000</span>)&nbsp;— the number of units of damage dealt by Ebony gun and Ivory gun, and the total number of damage required to break the shield, respectively.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if Dante can deal exactly <span class="tex-span"><i>c</i></span> damage to the shield and "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p>





```input1
4 6 15

```




```input2
3 2 7

```




```input3
6 11 6

```




```output1
No

```




```output2
Yes

```




```output3
Yes

```



## Note

<p>In the second sample, Dante can fire <span class="tex-span">1</span> bullet from Ebony and <span class="tex-span">2</span> from Ivory to deal exactly <span class="tex-span">1·3 + 2·2 = 7</span> damage. In the third sample, Dante can fire <span class="tex-span">1</span> bullet from ebony and no bullets from ivory to do <span class="tex-span">1·6 + 0·11 = 6</span> damage. </p>
