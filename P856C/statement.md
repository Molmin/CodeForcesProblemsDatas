## Description

<div><p>It is Borya's eleventh birthday, and he has got a great present: <span class="tex-span"><i>n</i></span> cards with numbers. The <span class="tex-span"><i>i</i></span>-th card has the number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> written on it. Borya wants to put his cards in a row to get one greater number. For example, if Borya has cards with numbers <span class="tex-span">1</span>, <span class="tex-span">31</span>, and <span class="tex-span">12</span>, and he puts them in a row in this order, he would get a number <span class="tex-span">13112</span>.</p><p>He is only 11, but he already knows that there are <span class="tex-span"><i>n</i>!</span> ways to put his cards in a row. But today is a special day, so he is only interested in such ways that the resulting big number is divisible by eleven. So, the way from the previous paragraph is good, because <span class="tex-span">13112 = 1192 × 11</span>, but if he puts the cards in the following order: <span class="tex-span">31</span>, <span class="tex-span">1</span>, <span class="tex-span">12</span>, he would get a number <span class="tex-span">31112</span>, it is not divisible by <span class="tex-span">11</span>, so this way is not good for Borya. Help Borya to find out how many good ways to put the cards are there.</p><p>Borya considers all cards different, even if some of them contain the same number. For example, if Borya has two cards with 1 on it, there are two good ways.</p><p>Help Borya, find the number of good ways to put the cards. This number can be large, so output it modulo <span class="tex-span">998244353</span>.</p></div><div class="input-specification"><p>Input data contains multiple test cases. The first line of the input data contains an integer <span class="tex-span"><i>t</i></span>&nbsp;— the number of test cases (<span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>). The descriptions of test cases follow.</p><p>Each test is described by two lines.</p><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>)&nbsp;— the number of cards in Borya's present.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— numbers written on the cards.</p><p>It is guaranteed that the total number of cards in all tests of one input data doesn't exceed <span class="tex-span">2000</span>.</p></div><div class="output-specification"><p>For each test case output one line: the number of ways to put the cards to the table so that the resulting big number was divisible by 11, print the number modulo <span class="tex-span">998244353</span>.</p></div>

## Input

<p>Input data contains multiple test cases. The first line of the input data contains an integer <span class="tex-span"><i>t</i></span>&nbsp;— the number of test cases (<span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>). The descriptions of test cases follow.</p><p>Each test is described by two lines.</p><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>)&nbsp;— the number of cards in Borya's present.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— numbers written on the cards.</p><p>It is guaranteed that the total number of cards in all tests of one input data doesn't exceed <span class="tex-span">2000</span>.</p>

## Output

<p>For each test case output one line: the number of ways to put the cards to the table so that the resulting big number was divisible by 11, print the number modulo <span class="tex-span">998244353</span>.</p>





```input1
4
2
1 1
3
1 31 12
3
12345 67 84
9
1 2 3 4 5 6 7 8 9

```




```output1
2
2
2
31680

```


