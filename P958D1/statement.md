## Description

<div><p>The Rebel fleet is on the run. It consists of <span class="tex-span"><i>m</i></span> ships currently gathered around a single planet. Just a few seconds ago, the vastly more powerful Empire fleet has appeared in the same solar system, and the Rebels will need to escape into hyperspace. In order to spread the fleet, the captain of each ship has independently come up with the coordinate to which that ship will jump. In the obsolete navigation system used by the Rebels, this coordinate is given as the value of an arithmetic expression of the form <img align="middle" class="tex-formula" src="file://3HLA2I7i.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>To plan the future of the resistance movement, Princess Heidi needs to know, for each ship, how many ships are going to end up at the same coordinate after the jump. You are her only hope!</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>) – the number of ships. The next <span class="tex-span"><i>m</i></span> lines describe one jump coordinate each, given as an arithmetic expression. An expression has the form <span class="tex-font-style-tt">(a+b)/c</span>. Namely, it consists of: an opening parenthesis <span class="tex-font-style-tt">(</span>, a positive integer <span class="tex-span"><i>a</i></span> of up to two decimal digits, a plus sign <span class="tex-font-style-tt">+</span>, a positive integer <span class="tex-span"><i>b</i></span> of up to two decimal digits, a closing parenthesis <span class="tex-font-style-tt">)</span>, a slash <span class="tex-font-style-tt">/</span>, and a positive integer <span class="tex-span"><i>c</i></span> of up to two decimal digits.</p></div><div class="output-specification"><p>Print a single line consisting of <span class="tex-span"><i>m</i></span> space-separated integers. The <span class="tex-span"><i>i</i></span>-th integer should be equal to the number of ships whose coordinate is equal to that of the <span class="tex-span"><i>i</i></span>-th ship (including the <span class="tex-span"><i>i</i></span>-th ship itself).</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>) – the number of ships. The next <span class="tex-span"><i>m</i></span> lines describe one jump coordinate each, given as an arithmetic expression. An expression has the form <span class="tex-font-style-tt">(a+b)/c</span>. Namely, it consists of: an opening parenthesis <span class="tex-font-style-tt">(</span>, a positive integer <span class="tex-span"><i>a</i></span> of up to two decimal digits, a plus sign <span class="tex-font-style-tt">+</span>, a positive integer <span class="tex-span"><i>b</i></span> of up to two decimal digits, a closing parenthesis <span class="tex-font-style-tt">)</span>, a slash <span class="tex-font-style-tt">/</span>, and a positive integer <span class="tex-span"><i>c</i></span> of up to two decimal digits.</p>

## Output

<p>Print a single line consisting of <span class="tex-span"><i>m</i></span> space-separated integers. The <span class="tex-span"><i>i</i></span>-th integer should be equal to the number of ships whose coordinate is equal to that of the <span class="tex-span"><i>i</i></span>-th ship (including the <span class="tex-span"><i>i</i></span>-th ship itself).</p>





```input1
4
(99+98)/97
(26+4)/10
(12+33)/15
(5+1)/7

```




```output1
1 2 2 1
```



## Note

<p>In the sample testcase, the second and the third ship will both end up at the coordinate <span class="tex-span">3</span>.</p><p>Note that this problem has only two versions – easy and hard.</p>
