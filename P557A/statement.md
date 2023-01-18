## Description

<div><p>Soon a school Olympiad in Informatics will be held in Berland, <span class="tex-span"><i>n</i></span> schoolchildren will participate there.</p><p>At a meeting of the jury of the Olympiad it was decided that <span class="tex-font-style-it">each</span> of the <span class="tex-span"><i>n</i></span> participants, depending on the results, will get a diploma of the first, second or third degree. Thus, each student will receive exactly one diploma.</p><p>They also decided that there must be given at least <span class="tex-span"><i>min</i><sub class="lower-index">1</sub></span> and at most <span class="tex-span"><i>max</i><sub class="lower-index">1</sub></span> diplomas of the first degree, at least <span class="tex-span"><i>min</i><sub class="lower-index">2</sub></span> and at most <span class="tex-span"><i>max</i><sub class="lower-index">2</sub></span> diplomas of the second degree, and at least <span class="tex-span"><i>min</i><sub class="lower-index">3</sub></span> and at most <span class="tex-span"><i>max</i><sub class="lower-index">3</sub></span> diplomas of the third degree.</p><p>After some discussion it was decided to choose from all the options of distributing diplomas satisfying these limitations the one that maximizes the number of participants who receive diplomas of the first degree. Of all these options they select the one which maximizes the number of the participants who receive diplomas of the second degree. If there are multiple of these options, they select the option that maximizes the number of diplomas of the third degree.</p><p>Choosing the best option of distributing certificates was entrusted to Ilya, one of the best programmers of Berland. However, he found more important things to do, so it is your task now to choose the best option of distributing of diplomas, based on the described limitations.</p><p>It is guaranteed that the described limitations are such that there is a way to choose such an option of distributing diplomas that all <span class="tex-span"><i>n</i></span> participants of the Olympiad will receive a diploma of some degree.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">6</sup></span>)&nbsp;—&nbsp;the number of schoolchildren who will participate in the Olympiad.</p><p>The next line of the input contains two integers <span class="tex-span"><i>min</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>max</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>min</i><sub class="lower-index">1</sub> ≤ <i>max</i><sub class="lower-index">1</sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;—&nbsp;the minimum and maximum limits on the number of diplomas of the first degree that can be distributed.</p><p>The third line of the input contains two integers <span class="tex-span"><i>min</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>max</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>min</i><sub class="lower-index">2</sub> ≤ <i>max</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;—&nbsp;the minimum and maximum limits on the number of diplomas of the second degree that can be distributed. </p><p>The next line of the input contains two integers <span class="tex-span"><i>min</i><sub class="lower-index">3</sub></span> and <span class="tex-span"><i>max</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>min</i><sub class="lower-index">3</sub> ≤ <i>max</i><sub class="lower-index">3</sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;—&nbsp;the minimum and maximum limits on the number of diplomas of the third degree that can be distributed. </p><p>It is guaranteed that <span class="tex-span"><i>min</i><sub class="lower-index">1</sub> + <i>min</i><sub class="lower-index">2</sub> + <i>min</i><sub class="lower-index">3</sub> ≤ <i>n</i> ≤ <i>max</i><sub class="lower-index">1</sub> + <i>max</i><sub class="lower-index">2</sub> + <i>max</i><sub class="lower-index">3</sub></span>.</p></div><div class="output-specification"><p>In the first line of the output print three numbers, showing how many diplomas of the first, second and third degree will be given to students in the optimal variant of distributing diplomas.</p><p>The optimal variant of distributing diplomas is the one that maximizes the number of students who receive diplomas of the first degree. Of all the suitable options, the best one is the one which maximizes the number of participants who receive diplomas of the second degree. If there are several of these options, the best one is the one that maximizes the number of diplomas of the third degree.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">6</sup></span>)&nbsp;—&nbsp;the number of schoolchildren who will participate in the Olympiad.</p><p>The next line of the input contains two integers <span class="tex-span"><i>min</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>max</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>min</i><sub class="lower-index">1</sub> ≤ <i>max</i><sub class="lower-index">1</sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;—&nbsp;the minimum and maximum limits on the number of diplomas of the first degree that can be distributed.</p><p>The third line of the input contains two integers <span class="tex-span"><i>min</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>max</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>min</i><sub class="lower-index">2</sub> ≤ <i>max</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;—&nbsp;the minimum and maximum limits on the number of diplomas of the second degree that can be distributed. </p><p>The next line of the input contains two integers <span class="tex-span"><i>min</i><sub class="lower-index">3</sub></span> and <span class="tex-span"><i>max</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>min</i><sub class="lower-index">3</sub> ≤ <i>max</i><sub class="lower-index">3</sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;—&nbsp;the minimum and maximum limits on the number of diplomas of the third degree that can be distributed. </p><p>It is guaranteed that <span class="tex-span"><i>min</i><sub class="lower-index">1</sub> + <i>min</i><sub class="lower-index">2</sub> + <i>min</i><sub class="lower-index">3</sub> ≤ <i>n</i> ≤ <i>max</i><sub class="lower-index">1</sub> + <i>max</i><sub class="lower-index">2</sub> + <i>max</i><sub class="lower-index">3</sub></span>.</p>

## Output

<p>In the first line of the output print three numbers, showing how many diplomas of the first, second and third degree will be given to students in the optimal variant of distributing diplomas.</p><p>The optimal variant of distributing diplomas is the one that maximizes the number of students who receive diplomas of the first degree. Of all the suitable options, the best one is the one which maximizes the number of participants who receive diplomas of the second degree. If there are several of these options, the best one is the one that maximizes the number of diplomas of the third degree.</p>





```input1
6
1 5
2 6
3 7

```




```input2
10
1 2
1 3
1 5

```




```input3
6
1 3
2 2
2 2

```




```output1
1 2 3 

```




```output2
2 3 5 

```




```output3
2 2 2 

```


