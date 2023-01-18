## Description

<div><p>Innokentiy likes tea very much and today he wants to drink exactly <span class="tex-span"><i>n</i></span> cups of tea. He would be happy to drink more but he had exactly <span class="tex-span"><i>n</i></span> tea bags, <span class="tex-span"><i>a</i></span> of them are green and <span class="tex-span"><i>b</i></span> are black.</p><p>Innokentiy doesn't like to drink the same tea (green or black) more than <span class="tex-span"><i>k</i></span> times in a row. Your task is to determine the order of brewing tea bags so that Innokentiy will be able to drink <span class="tex-span"><i>n</i></span> cups of tea, without drinking the same tea more than <span class="tex-span"><i>k</i></span> times in a row, or to inform that it is impossible. Each tea bag has to be used exactly once.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>)&nbsp;— the number of cups of tea Innokentiy wants to drink, the maximum number of cups of same tea he can drink in a row, the number of tea bags of green and black tea. It is guaranteed that <span class="tex-span"><i>a</i> + <i>b</i> = <i>n</i></span>.</p></div><div class="output-specification"><p>If it is impossible to drink <span class="tex-span"><i>n</i></span> cups of tea, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, print the string of the length <span class="tex-span"><i>n</i></span>, which consists of characters '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">B</span>'. If some character equals '<span class="tex-font-style-tt">G</span>', then the corresponding cup of tea should be green. If some character equals '<span class="tex-font-style-tt">B</span>', then the corresponding cup of tea should be black.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>)&nbsp;— the number of cups of tea Innokentiy wants to drink, the maximum number of cups of same tea he can drink in a row, the number of tea bags of green and black tea. It is guaranteed that <span class="tex-span"><i>a</i> + <i>b</i> = <i>n</i></span>.</p>

## Output

<p>If it is impossible to drink <span class="tex-span"><i>n</i></span> cups of tea, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, print the string of the length <span class="tex-span"><i>n</i></span>, which consists of characters '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">B</span>'. If some character equals '<span class="tex-font-style-tt">G</span>', then the corresponding cup of tea should be green. If some character equals '<span class="tex-font-style-tt">B</span>', then the corresponding cup of tea should be black.</p><p>If there are multiple answers, print any of them.</p>





```input1
5 1 3 2

```




```input2
7 2 2 5

```




```input3
4 3 4 0

```




```output1
GBGBG

```




```output2
BBGBGBB
```




```output3
NO

```


