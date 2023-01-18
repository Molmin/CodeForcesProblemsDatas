## Description

<div><p>According to Berland laws it is only allowed to sell alcohol to people <span class="tex-font-style-bf">not younger than</span> 18 years. Vasya's job is to monitor the law's enforcement. Tonight he entered a bar and saw <span class="tex-span"><i>n</i></span> people sitting there. For every one of them Vasya happened to determine either the age or the drink the person is having. Vasya can check any person, i.e. learn his age and the drink he is having at the same time. What minimal number of people should Vasya check additionally to make sure that there are no clients under 18 having alcohol drinks?</p><p>The list of all alcohol drinks in Berland is: <span class="tex-font-style-tt">ABSINTH</span>, <span class="tex-font-style-tt">BEER</span>, <span class="tex-font-style-tt">BRANDY</span>, <span class="tex-font-style-tt">CHAMPAGNE</span>, <span class="tex-font-style-tt">GIN</span>, <span class="tex-font-style-tt">RUM</span>, <span class="tex-font-style-tt">SAKE</span>, <span class="tex-font-style-tt">TEQUILA</span>, <span class="tex-font-style-tt">VODKA</span>, <span class="tex-font-style-tt">WHISKEY</span>, <span class="tex-font-style-tt">WINE</span></p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) which is the number of the bar's clients. Then follow <span class="tex-span"><i>n</i></span> lines, each describing one visitor. A line either contains his age (an integer from 0 to 1000) or his drink (a string of capital Latin letters from 1 to 100 in length). It is guaranteed that the input data does not contain spaces and other unnecessary separators.</p><p>Only the drinks from the list given above should be considered alcohol.</p></div><div class="output-specification"><p>Print a single number which is the number of people Vasya should check to guarantee the law enforcement.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) which is the number of the bar's clients. Then follow <span class="tex-span"><i>n</i></span> lines, each describing one visitor. A line either contains his age (an integer from 0 to 1000) or his drink (a string of capital Latin letters from 1 to 100 in length). It is guaranteed that the input data does not contain spaces and other unnecessary separators.</p><p>Only the drinks from the list given above should be considered alcohol.</p>

## Output

<p>Print a single number which is the number of people Vasya should check to guarantee the law enforcement.</p>





```input1
5
18
VODKA
COKE
19
17

```




```output1
2

```



## Note

<p>In the sample test the second and fifth clients should be checked.</p>
