## Description

<div><p>Harry, Ron and Hermione have figured out that Helga Hufflepuff's cup is a horcrux. Through her encounter with Bellatrix Lestrange, Hermione came to know that the cup is present in Bellatrix's family vault in Gringott's Wizarding Bank. </p><p>The Wizarding bank is in the form of a tree with total <span class="tex-span"><i>n</i></span> vaults where each vault has some type, denoted by a number between <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. A tree is an undirected connected graph with no cycles.</p><p>The vaults with the highest security are of type <span class="tex-span"><i>k</i></span>, and all vaults of type <span class="tex-span"><i>k</i></span> have the highest security.</p><p><span class="tex-font-style-bf">There can be at most <span class="tex-span"><i>x</i></span> vaults of highest security</span>. </p><p>Also, <span class="tex-font-style-bf">if a vault is of the highest security, its adjacent vaults are guaranteed to not be of the highest security and their type is guaranteed to be less than <span class="tex-span"><i>k</i></span></span>.</p><p>Harry wants to consider every possibility so that he can easily find the best path to reach Bellatrix's vault. So, you have to tell him, given the tree structure of Gringotts, the number of possible ways of giving each vault a type such that the above conditions hold.</p></div><div class="input-specification"><p>The first line of input contains two space separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>&nbsp;— the number of vaults and the number of different vault types possible. (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contain two space separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) representing the <span class="tex-span"><i>i</i></span>-th edge, which shows there is a path between the two vaults <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that the given graph is a tree.</p><p>The last line of input contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>m</i>, 1 ≤ <i>x</i> ≤ 10</span>), the type of the highest security vault and the maximum possible number of vaults of highest security.</p></div><div class="output-specification"><p>Output a single integer, the number of ways of giving each vault a type following the conditions modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of input contains two space separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>&nbsp;— the number of vaults and the number of different vault types possible. (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contain two space separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) representing the <span class="tex-span"><i>i</i></span>-th edge, which shows there is a path between the two vaults <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that the given graph is a tree.</p><p>The last line of input contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>m</i>, 1 ≤ <i>x</i> ≤ 10</span>), the type of the highest security vault and the maximum possible number of vaults of highest security.</p>

## Output

<p>Output a single integer, the number of ways of giving each vault a type following the conditions modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
4 2
1 2
2 3
1 4
1 2

```




```input2
3 3
1 2
1 3
2 1

```




```input3
3 1
1 2
1 3
1 1

```




```output1
1

```




```output2
13

```




```output3
0

```



## Note

<p>In test case <span class="tex-span">1</span>, we cannot have any vault of the highest security as its type is <span class="tex-span">1</span> implying that its adjacent vaults would have to have a vault type less than <span class="tex-span">1</span>, which is not allowed. Thus, there is only one possible combination, in which all the vaults have type <span class="tex-span">2</span>.</p>
