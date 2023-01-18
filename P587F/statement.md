## Description

<div><p>Duff is mad at her friends. That's why she sometimes makes Malek to take candy from one of her friends for no reason!</p><center> <img class="tex-graphics" src="file://rO545BbA.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>She has <span class="tex-span"><i>n</i></span> friends. Her <span class="tex-span"><i>i</i></span>-th friend's name is <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (their names are not necessarily unique). <span class="tex-span"><i>q</i></span> times, she asks Malek to take candy from her friends. She's angry, but also she acts with rules. When she wants to ask Malek to take candy from one of her friends, like <span class="tex-span"><i>k</i></span>, she chooses two numbers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> and tells Malek to take exactly <img align="middle" class="tex-formula" src="file://ouEQT993.png" style="max-width: 100.0%;max-height: 100.0%;"> candies from him/her, where <span class="tex-span"><i>occur</i>(<i>t</i>, <i>s</i>)</span> is the number of occurrences of string <span class="tex-span"><i>t</i></span> in <span class="tex-span"><i>s</i></span>.</p><p>Malek is not able to calculate how many candies to take in each request from Duff. That's why she asked for your help. Please tell him how many candies to take in each request.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the names. <span class="tex-span"><i>i</i></span>-th of them contains an string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, consisting of lowercase English letters   (<img align="middle" class="tex-formula" src="file://0go7NKPB.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the requests. Each of them contains three integers, <span class="tex-span"><i>l</i>, <i>r</i></span> and <span class="tex-span"><i>k</i></span> (says that Malek should take <img align="middle" class="tex-formula" src="file://WLdxCqGS.png" style="max-width: 100.0%;max-height: 100.0%;"> candies from Duff's <span class="tex-span"><i>k</i></span>-th friend).</p></div><div class="output-specification"><p>Print the answer to each request in one line.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the names. <span class="tex-span"><i>i</i></span>-th of them contains an string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, consisting of lowercase English letters   (<img align="middle" class="tex-formula" src="file://0go7NKPB.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the requests. Each of them contains three integers, <span class="tex-span"><i>l</i>, <i>r</i></span> and <span class="tex-span"><i>k</i></span> (says that Malek should take <img align="middle" class="tex-formula" src="file://WLdxCqGS.png" style="max-width: 100.0%;max-height: 100.0%;"> candies from Duff's <span class="tex-span"><i>k</i></span>-th friend).</p>

## Output

<p>Print the answer to each request in one line.</p>





```input1
5 5
a
ab
abab
ababab
b
1 5 4
3 5 4
1 5 2
1 5 3
1 4 1

```




```output1
12
6
3
7
1

```


