## Description

<div><p>A team of students from the city S is sent to the All-Berland Olympiad in Informatics. Traditionally, they go on the train. All students have bought tickets in one carriage, consisting of <span class="tex-span"><i>n</i></span> compartments (each compartment has exactly four people). We know that if one compartment contain one or two students, then they get bored, and if one compartment contain three or four students, then the compartment has fun throughout the entire trip.</p><p>The students want to swap with other people, so that no compartment with students had bored students. To swap places with another person, you need to convince him that it is really necessary. The students can not independently find the necessary arguments, so they asked a sympathetic conductor for help. The conductor can use her life experience to persuade any passenger to switch places with some student.</p><p>However, the conductor does not want to waste time persuading the wrong people, so she wants to know what is the minimum number of people necessary to persuade her to change places with the students. Your task is to find the number. </p><p>After all the swaps each compartment should either have no student left, or have a company of three or four students. </p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of compartments in the carriage. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> showing how many students ride in each compartment (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 4</span>). It is guaranteed that at least one student is riding in the train.</p></div><div class="output-specification"><p>If no sequence of swapping seats with other people leads to the desired result, print number "<span class="tex-font-style-tt">-1</span>" (without the quotes). In another case, print the smallest number of people you need to persuade to swap places.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of compartments in the carriage. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> showing how many students ride in each compartment (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 4</span>). It is guaranteed that at least one student is riding in the train.</p>

## Output

<p>If no sequence of swapping seats with other people leads to the desired result, print number "<span class="tex-font-style-tt">-1</span>" (without the quotes). In another case, print the smallest number of people you need to persuade to swap places.</p>





```input1
5
1 2 2 4 3

```




```input2
3
4 1 1

```




```input3
4
0 3 0 4

```




```output1
2

```




```output2
2

```




```output3
0

```


