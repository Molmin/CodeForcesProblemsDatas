## Description

<div><p>After Santa Claus and his assistant Elf delivered all the presents and made all the wishes come true, they returned to the North Pole and found out that it is all covered with snow. Both of them were quite tired and they decided only to remove the snow from the roads connecting huts. The North Pole has <span class="tex-span"><i>n</i></span> huts connected with <span class="tex-span"><i>m</i></span> roads. One can go along the roads in both directions. </p><p>The Elf offered to split: Santa Claus will clear up the wide roads and the Elf will tread out the narrow roads. For each road they decided who will clear it: Santa Claus or the Elf. To minimize the efforts they decided to clear the road so as to fulfill both those conditions: </p><ul> <li> between any two huts should exist <span class="tex-font-style-bf">exactly one simple path</span> along the cleared roads; </li><li> Santa Claus and the Elf should clear the same number of roads. </li></ul><p>At this point Santa Claus and his assistant Elf wondered which roads should they clear up?</p></div><div class="input-specification"><p>The first input line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of huts and the number of roads. Then follow <span class="tex-span"><i>m</i></span> lines, each of them contains a road description: the numbers of huts it connects — <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>) and the person responsible for clearing out this road ("<span class="tex-font-style-tt">S</span>" — for the Elf or "<span class="tex-font-style-tt">M</span>" for Santa Claus). It is possible to go on each road in both directions. Note that there can be more than one road between two huts and a road can begin and end in the same hut.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">-1</span>" without the quotes if it is impossible to choose the roads that will be cleared by the given rule. Otherwise print in the first line how many roads should be cleared and in the second line print the numbers of those roads (the roads are numbered from <span class="tex-span">1</span> in the order of occurrence in the input). It is allowed to print the numbers of the roads in any order. Each number should be printed exactly once. As you print the numbers, separate them with spaces.</p></div>

## Input

<p>The first input line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of huts and the number of roads. Then follow <span class="tex-span"><i>m</i></span> lines, each of them contains a road description: the numbers of huts it connects — <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>) and the person responsible for clearing out this road ("<span class="tex-font-style-tt">S</span>" — for the Elf or "<span class="tex-font-style-tt">M</span>" for Santa Claus). It is possible to go on each road in both directions. Note that there can be more than one road between two huts and a road can begin and end in the same hut.</p>

## Output

<p>Print "<span class="tex-font-style-tt">-1</span>" without the quotes if it is impossible to choose the roads that will be cleared by the given rule. Otherwise print in the first line how many roads should be cleared and in the second line print the numbers of those roads (the roads are numbered from <span class="tex-span">1</span> in the order of occurrence in the input). It is allowed to print the numbers of the roads in any order. Each number should be printed exactly once. As you print the numbers, separate them with spaces.</p>





```input1
1 2
1 1 S
1 1 M

```




```input2
3 3
1 2 S
1 3 M
2 3 S

```




```input3
5 6
1 1 S
1 2 M
1 3 S
1 4 M
1 5 M
2 2 S

```




```output1
0


```




```output2
2
2 1 

```




```output3
-1

```



## Note

<p>A path is called simple if all huts on it are pairwise different.</p>
