## Description

<div><p>Think of New York as a rectangular grid consisting of <span class="tex-span"><i>N</i></span> vertical avenues numerated from <span class="tex-span">1</span> to <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span> horizontal streets numerated <span class="tex-span">1</span> to <span class="tex-span"><i>M</i></span>. <span class="tex-span"><i>C</i></span> friends are staying at <span class="tex-span"><i>C</i></span> hotels located at some street-avenue crossings. They are going to celebrate birthday of one of them in the one of <span class="tex-span"><i>H</i></span> restaurants also located at some street-avenue crossings. They also want that the maximum distance covered by one of them while traveling to the restaurant to be minimum possible. Help friends choose optimal restaurant for a celebration.</p><p>Suppose that the distance between neighboring crossings are all the same equal to one kilometer.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>N</i></span> и <span class="tex-span"><i>M</i></span>&nbsp;— size of the city (<span class="tex-span">1 ≤ <i>N</i>, <i>M</i> ≤ 10<sup class="upper-index">9</sup></span>). In the next line there is a single integer <span class="tex-span"><i>C</i></span> (<span class="tex-span">1 ≤ <i>C</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of hotels friends stayed at. Following <span class="tex-span"><i>C</i></span> lines contain descriptions of hotels, each consisting of two coordinates <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>N</i></span>, <span class="tex-span">1 ≤ <i>y</i> ≤ <i>M</i></span>). The next line contains an integer <span class="tex-span"><i>H</i></span>&nbsp;— the number of restaurants (<span class="tex-span">1 ≤ <i>H</i> ≤ 10<sup class="upper-index">5</sup></span>). Following <span class="tex-span"><i>H</i></span> lines contain descriptions of restaurants in the same format.</p><p>Several restaurants and hotels may be located near the same crossing.</p></div><div class="output-specification"><p>In the first line output the optimal distance. In the next line output index of a restaurant that produces this optimal distance. If there are several possibilities, you are allowed to output any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>N</i></span> и <span class="tex-span"><i>M</i></span>&nbsp;— size of the city (<span class="tex-span">1 ≤ <i>N</i>, <i>M</i> ≤ 10<sup class="upper-index">9</sup></span>). In the next line there is a single integer <span class="tex-span"><i>C</i></span> (<span class="tex-span">1 ≤ <i>C</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of hotels friends stayed at. Following <span class="tex-span"><i>C</i></span> lines contain descriptions of hotels, each consisting of two coordinates <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>N</i></span>, <span class="tex-span">1 ≤ <i>y</i> ≤ <i>M</i></span>). The next line contains an integer <span class="tex-span"><i>H</i></span>&nbsp;— the number of restaurants (<span class="tex-span">1 ≤ <i>H</i> ≤ 10<sup class="upper-index">5</sup></span>). Following <span class="tex-span"><i>H</i></span> lines contain descriptions of restaurants in the same format.</p><p>Several restaurants and hotels may be located near the same crossing.</p>

## Output

<p>In the first line output the optimal distance. In the next line output index of a restaurant that produces this optimal distance. If there are several possibilities, you are allowed to output any of them.</p>





```input1
10 10
2
1 1
3 3
2
1 10
4 4

```




```output1
6
2

```


