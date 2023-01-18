## Description

<div><p>Petya loves lucky numbers. Everybody knows that positive integers are <span class="tex-font-style-underline">lucky</span> if their decimal representation doesn't contain digits other than <span class="tex-span">4</span> and <span class="tex-span">7</span>. For example, numbers <span class="tex-span">47</span>, <span class="tex-span">744</span>, <span class="tex-span">4</span> are lucky and <span class="tex-span">5</span>, <span class="tex-span">17</span>, <span class="tex-span">467</span> are not.</p><p>One night Petya was sleeping. He was dreaming of being the president of some island country. The country is represented by islands connected by two-way roads. Between some islands there is no road way, even through other islands, that's why the country is divided into several regions. More formally, each island belongs to exactly one region, there is a path between any two islands located in the same region; there is no path between any two islands from different regions. A region is lucky if the amount of islands in it is a lucky number.</p><p>As a real president, Petya first decided to build a presidential palace. Being a lucky numbers' fan, Petya wants to position his palace in one of the lucky regions. However, it is possible that initially the country has no such regions. In this case Petya can build additional roads between different regions, thus joining them. Find the minimum number of roads needed to build to create a lucky region.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). They are the number of islands and the number of roads correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain road descriptions. Each road is defined by the numbers of islands that it connects: that is, by two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>). Some roads can connect an island with itself; there can be more than one road between a pair of islands. Numbers in each line are separated by exactly one space character.</p></div><div class="output-specification"><p>If there's no solution, output the only number "-1" (without the quotes). Otherwise, output the minimum number of roads <span class="tex-span"><i>r</i></span> that need to be built to get a lucky region.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). They are the number of islands and the number of roads correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain road descriptions. Each road is defined by the numbers of islands that it connects: that is, by two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>). Some roads can connect an island with itself; there can be more than one road between a pair of islands. Numbers in each line are separated by exactly one space character.</p>

## Output

<p>If there's no solution, output the only number "-1" (without the quotes). Otherwise, output the minimum number of roads <span class="tex-span"><i>r</i></span> that need to be built to get a lucky region.</p>





```input1
4 3
1 2
2 3
1 3

```




```input2
5 4
1 2
3 4
4 5
3 5

```




```output1
1

```




```output2
-1

```


