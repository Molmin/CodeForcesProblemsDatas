## Description

<div><p>Little Vasya loves orange juice very much. That's why any food and drink in his kitchen necessarily contains orange juice. There are <span class="tex-span"><i>n</i></span> drinks in his fridge, the volume fraction of orange juice in the <span class="tex-span"><i>i</i></span>-th drink equals <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> percent.</p><p>One day Vasya decided to make himself an orange cocktail. He took equal proportions of each of the <span class="tex-span"><i>n</i></span> drinks and mixed them. Then he wondered, how much orange juice the cocktail has.</p><p>Find the volume fraction of orange juice in the final drink.</p></div><div class="input-specification"><p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of orange-containing drinks in Vasya's fridge. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the volume fraction of orange juice in the <span class="tex-span"><i>i</i></span>-th drink, in percent. The numbers are separated by a space.</p></div><div class="output-specification"><p>Print the volume fraction in percent of orange juice in Vasya's cocktail. The answer will be considered correct if the absolute or relative error does not exceed <span class="tex-span">10 <sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of orange-containing drinks in Vasya's fridge. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the volume fraction of orange juice in the <span class="tex-span"><i>i</i></span>-th drink, in percent. The numbers are separated by a space.</p>

## Output

<p>Print the volume fraction in percent of orange juice in Vasya's cocktail. The answer will be considered correct if the absolute or relative error does not exceed <span class="tex-span">10 <sup class="upper-index"> - 4</sup></span>.</p>





```input1
3
50 50 100

```




```input2
4
0 25 50 75

```




```output1
66.666666666667

```




```output2
37.500000000000

```



## Note

<p>Note to the first sample: let's assume that Vasya takes <span class="tex-span"><i>x</i></span> milliliters of each drink from the fridge. Then the volume of pure juice in the cocktail will equal <img align="middle" class="tex-formula" src="file://yL9U2Kqo.png" style="max-width: 100.0%;max-height: 100.0%;"> milliliters. The total cocktail's volume equals <span class="tex-span">3·<i>x</i></span> milliliters, so the volume fraction of the juice in the cocktail equals <img align="middle" class="tex-formula" src="file://vwft6ZwH.png" style="max-width: 100.0%;max-height: 100.0%;">, that is, <span class="tex-span">66.(6)</span> percent.</p>
