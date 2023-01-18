## Description

<div><p>The story was not finished as PMP thought. God offered him one more chance to reincarnate and come back to life. But before he can come back, God told him that PMP should ask <span class="tex-span"><i>n</i></span> great men including prominent programmers about their life experiences.</p><p>The men are standing on a straight line. They are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span> from left to right. The coordinate of the <span class="tex-span"><i>i</i></span>-th man is <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i><sub class="lower-index"><i>i</i> + 1</sub>, <i>i</i> &lt; <i>n</i>)</span>. PMP should visit all these people one by one in arbitrary order. Each men should be visited <span class="tex-font-style-bf">exactly once</span>. At the beginning of his tour, he starts at location of <span class="tex-span"><i>s</i></span>-th man and asks him about his experiences.</p><p>Each time PMP wants to change his location, he should give a ticket to an angel and the angel carries him to his destination. Angels take PMP from one location, fly to his destination and put him down there. Nobody else is visited in this movement. Moving from <span class="tex-span"><i>i</i></span>-th man to <span class="tex-span"><i>j</i></span>-th man, takes <span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>j</i></sub>|</span> time. PMP can get back to life as soon as he visits all men.</p><p>There are two types of angels: Some angels are going to the right and they only accept right tickets. Others are going the left and they only accept left tickets. There are an unlimited number of angels of each type. PMP has <span class="tex-span"><i>l</i></span> left tickets and <span class="tex-span"><i>n</i> - 1 - <i>l</i></span> right tickets.</p><p>PMP wants to get back to life as soon as possible to be able to compete in this year's final instead of the final he missed last year. He wants to know the quickest way to visit all the men exactly once. He also needs to know the exact sequence moves he should make.</p></div><div class="input-specification"><p>The first line of input contains three space-separated integers <span class="tex-span"><i>n</i>, <i>l</i>, <i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>l</i> &lt; <i>n</i>, 1 ≤ <i>s</i> ≤ <i>n</i></span>) — the number of people to visit, the number left tickets PMP got, and initial location of PMP. Next line contains <span class="tex-span"><i>n</i></span> space-separated integers. The <span class="tex-span"><i>i</i></span>-th integer in this line is <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 = <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>x</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the location of <span class="tex-span"><i>i</i></span>-th man.</p></div><div class="output-specification"><p>If PMP cannot visit all men with the tickets he got print -1 in the only line of output. Otherwise, in the first line you should print the minimum time PMP can visit all men. In the second line you should print <span class="tex-span"><i>n</i> - 1</span> integers that are the numbers of the men that PMP should visit in order in one optimal solution. If there are multiple answers, output any of them.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line of input contains three space-separated integers <span class="tex-span"><i>n</i>, <i>l</i>, <i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>l</i> &lt; <i>n</i>, 1 ≤ <i>s</i> ≤ <i>n</i></span>) — the number of people to visit, the number left tickets PMP got, and initial location of PMP. Next line contains <span class="tex-span"><i>n</i></span> space-separated integers. The <span class="tex-span"><i>i</i></span>-th integer in this line is <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 = <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>x</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the location of <span class="tex-span"><i>i</i></span>-th man.</p>

## Output

<p>If PMP cannot visit all men with the tickets he got print -1 in the only line of output. Otherwise, in the first line you should print the minimum time PMP can visit all men. In the second line you should print <span class="tex-span"><i>n</i> - 1</span> integers that are the numbers of the men that PMP should visit in order in one optimal solution. If there are multiple answers, output any of them.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
5 2 2
0 10 11 21 22

```




```input2
4 3 1
0 1 2 3

```




```input3
7 3 2
0 100 200 201 301 303 305

```




```output1
33
1 3 5 4

```




```output2
-1

```




```output3
409
1 3 4 7 6 5

```



## Note

<p>Let us remind here, a great contestant of all times, who left us about a year ago. May Renat Mullakhanov rest in peace.</p>
