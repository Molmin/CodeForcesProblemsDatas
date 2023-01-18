## Description

<div><p>One particularly well-known fact about zombies is that they move and think terribly slowly. While we still don't know why their movements are so sluggish, the problem of laggy thinking has been recently resolved. It turns out that the reason is not (as previously suspected) any kind of brain defect – it's the opposite! Independent researchers confirmed that the nervous system of a zombie is highly complicated – it consists of <span class="tex-span"><i>n</i></span> brains (much like a cow has several stomachs). They are interconnected by <span class="tex-font-style-it">brain connectors</span>, which are veins capable of transmitting thoughts between brains. There are two important properties such a brain network should have to function properly: </p><ol> <li> It should be possible to exchange thoughts between any two pairs of brains (perhaps indirectly, through other brains). </li><li> There should be no redundant brain connectors, that is, removing any brain connector would make property 1 false. </li></ol><p>If both properties are satisfied, we say that the nervous system is <span class="tex-font-style-it">valid</span>. Unfortunately (?), if the system is not valid, the zombie stops thinking and becomes (even more) dead. Your task is to analyze a given nervous system of a zombie and find out whether it is valid.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) denoting the number of brains (which are conveniently numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>) and the number of brain connectors in the nervous system, respectively. In the next <span class="tex-span"><i>m</i></span> lines, descriptions of brain connectors follow. Every connector is given as a pair of brains <span class="tex-span"><i>a</i> <i>b</i></span> it connects (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>).</p></div><div class="output-specification"><p>The output consists of one line, containing either <span class="tex-font-style-tt">yes</span> or <span class="tex-font-style-tt">no</span> depending on whether the nervous system is valid.</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) denoting the number of brains (which are conveniently numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>) and the number of brain connectors in the nervous system, respectively. In the next <span class="tex-span"><i>m</i></span> lines, descriptions of brain connectors follow. Every connector is given as a pair of brains <span class="tex-span"><i>a</i> <i>b</i></span> it connects (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>).</p>

## Output

<p>The output consists of one line, containing either <span class="tex-font-style-tt">yes</span> or <span class="tex-font-style-tt">no</span> depending on whether the nervous system is valid.</p>





```input1
4 4
1 2
2 3
3 1
4 1

```




```input2
6 5
1 2
2 3
3 4
4 5
3 6

```




```output1
no

```




```output2
yes

```


