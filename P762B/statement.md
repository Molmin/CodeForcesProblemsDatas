## Description

<div><p>Due to the increase in the number of students of Berland State University it was decided to equip a new computer room. You were given the task of buying mouses, and you have to spend as little as possible. After all, the country is in crisis!</p><p>The computers bought for the room were different. Some of them had only USB ports, some&nbsp;— only PS/2 ports, and some had both options.</p><p>You have found a price list of a certain computer shop. In it, for <span class="tex-span"><i>m</i></span> mouses it is specified the cost and the type of the port that is required to plug the mouse in (USB or PS/2). Each mouse from the list can be bought at most once.</p><p>You want to buy some set of mouses from the given price list in such a way so that you maximize the number of computers equipped with mouses (it is not guaranteed that you will be able to equip all of the computers), and in case of equality of this value you want to minimize the total cost of mouses you will buy.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">5</sup></span>) &nbsp;— the number of computers that only have USB ports, the number of computers, that only have PS/2 ports, and the number of computers, that have both options, respectively.</p><p>The next line contains one integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) &nbsp;— the number of mouses in the price list.</p><p>The next <span class="tex-span"><i>m</i></span> lines each describe another mouse. The <span class="tex-span"><i>i</i></span>-th line contains first integer <span class="tex-span"><i>val</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>val</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) &nbsp;— the cost of the <span class="tex-span"><i>i</i></span>-th mouse, then the type of port (USB or PS/2) that is required to plug the mouse in.</p></div><div class="output-specification"><p>Output two integers separated by space&nbsp;— the number of equipped computers and the total cost of the mouses you will buy.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">5</sup></span>) &nbsp;— the number of computers that only have USB ports, the number of computers, that only have PS/2 ports, and the number of computers, that have both options, respectively.</p><p>The next line contains one integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) &nbsp;— the number of mouses in the price list.</p><p>The next <span class="tex-span"><i>m</i></span> lines each describe another mouse. The <span class="tex-span"><i>i</i></span>-th line contains first integer <span class="tex-span"><i>val</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>val</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) &nbsp;— the cost of the <span class="tex-span"><i>i</i></span>-th mouse, then the type of port (USB or PS/2) that is required to plug the mouse in.</p>

## Output

<p>Output two integers separated by space&nbsp;— the number of equipped computers and the total cost of the mouses you will buy.</p>





```input1
2 1 1
4
5 USB
6 PS/2
3 PS/2
7 PS/2

```




```output1
3 14

```



## Note

<p>In the first example you can buy the first three mouses. This way you will equip one of the computers that has only a USB port with a USB mouse, and the two PS/2 mouses you will plug into the computer with PS/2 port and the computer with both ports.</p>
