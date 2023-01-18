## Description

<div><p>Mad scientist Mike is busy carrying out experiments in chemistry. Today he will attempt to join three atoms into one molecule.</p><p>A molecule consists of atoms, with some pairs of atoms connected by atomic bonds. Each atom has a valence number — the number of bonds the atom must form with other atoms. An atom can form <span class="tex-font-style-bf">one or multiple</span> bonds with any other atom, but it cannot form a bond with itself. The number of bonds of an atom in the molecule must be equal to its valence number.</p><center> <img class="tex-graphics" src="file://WA4t367a.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Mike knows valence numbers of the three atoms. Find a molecule that can be built from these atoms according to the stated rules, or determine that it is impossible.</p></div><div class="input-specification"><p>The single line of the input contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">6</sup></span>) — the valence numbers of the given atoms.</p></div><div class="output-specification"><p>If such a molecule can be built, print three space-separated integers — the number of bonds between the 1-st and the 2-nd, the 2-nd and the 3-rd, the 3-rd and the 1-st atoms, correspondingly. If there are multiple solutions, output any of them. If there is no solution, print "<span class="tex-font-style-tt">Impossible</span>" (without the quotes).</p></div>

## Input

<p>The single line of the input contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">6</sup></span>) — the valence numbers of the given atoms.</p>

## Output

<p>If such a molecule can be built, print three space-separated integers — the number of bonds between the 1-st and the 2-nd, the 2-nd and the 3-rd, the 3-rd and the 1-st atoms, correspondingly. If there are multiple solutions, output any of them. If there is no solution, print "<span class="tex-font-style-tt">Impossible</span>" (without the quotes).</p>





```input1
1 1 2

```




```input2
3 4 5

```




```input3
4 1 1

```




```output1
0 1 1

```




```output2
1 3 2

```




```output3
Impossible

```



## Note

<p>The first sample corresponds to the first figure. There are no bonds between atoms 1 and 2 in this case.</p><p>The second sample corresponds to the second figure. There is one or more bonds between each pair of atoms.</p><p>The third sample corresponds to the third figure. There is no solution, because an atom cannot form bonds with itself.</p><p>The configuration in the fourth figure is impossible as each atom must have at least one atomic bond.</p>
