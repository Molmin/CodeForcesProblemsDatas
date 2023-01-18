## Description

<div><p>During a New Year special offer the "Sudislavl Bars" offered <span class="tex-span"><i>n</i></span> promo codes. Each promo code consists of exactly six digits and gives right to one free cocktail at the bar "Mosquito Shelter". Of course, all the promocodes differ.</p><p>As the "Mosquito Shelter" opens only at 9, and partying in Sudislavl usually begins at as early as 6, many problems may arise as to how to type a promotional code without errors. It is necessary to calculate such maximum <span class="tex-span"><i>k</i></span>, that the promotional code could be uniquely identified if it was typed with no more than <span class="tex-span"><i>k</i></span> errors. At that, <span class="tex-span"><i>k</i> = 0</span> means that the promotional codes must be entered exactly.</p><p>A mistake in this problem should be considered as entering the wrong numbers. For example, value "<span class="tex-font-style-tt">123465</span>" contains two errors relative to promocode "<span class="tex-font-style-tt">123456</span>". Regardless of the number of errors the entered value consists of exactly six digits.</p></div><div class="input-specification"><p>The first line of the output contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of promocodes.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a single promocode, consisting of exactly 6 digits. It is guaranteed that all the promocodes are distinct. Promocodes can start from digit "<span class="tex-font-style-tt">0</span>".</p></div><div class="output-specification"><p>Print the maximum <span class="tex-span"><i>k</i></span> (naturally, not exceeding the length of the promocode), such that any promocode can be uniquely identified if it is typed with at most <span class="tex-span"><i>k</i></span> mistakes.</p></div>

## Input

<p>The first line of the output contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of promocodes.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a single promocode, consisting of exactly 6 digits. It is guaranteed that all the promocodes are distinct. Promocodes can start from digit "<span class="tex-font-style-tt">0</span>".</p>

## Output

<p>Print the maximum <span class="tex-span"><i>k</i></span> (naturally, not exceeding the length of the promocode), such that any promocode can be uniquely identified if it is typed with at most <span class="tex-span"><i>k</i></span> mistakes.</p>





```input1
2
000000
999999

```




```input2
6
211111
212111
222111
111111
112111
121111

```




```output1
2

```




```output2
0

```



## Note

<p>In the first sample <span class="tex-span"><i>k</i> &lt; 3</span>, so if a bar customer types in value "<span class="tex-font-style-tt">090909</span>", then it will be impossible to define which promocode exactly corresponds to it.</p>
