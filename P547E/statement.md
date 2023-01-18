## Description

<div><p>What-The-Fatherland is a strange country! All phone numbers there are strings consisting of lowercase English letters. What is double strange that a phone number can be associated with several bears!</p><p>In that country there is a rock band called CF consisting of <span class="tex-span"><i>n</i></span> bears (including Mike) numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. </p><center> <img class="tex-graphics" src="file://EkE0fGyd.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Phone number of <span class="tex-span"><i>i</i></span>-th member of CF is <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. May 17th is a holiday named Phone Calls day. In the last Phone Calls day, everyone called all the numbers that are substrings of his/her number (one may call some number several times). In particular, everyone called himself (that was really strange country).</p><p>Denote as <span class="tex-span"><i>call</i>(<i>i</i>, <i>j</i>)</span> the number of times that <span class="tex-span"><i>i</i></span>-th member of CF called the <span class="tex-span"><i>j</i></span>-th member of CF. </p><p>The geek Mike has <span class="tex-span"><i>q</i></span> questions that he wants to ask you. In each question he gives you numbers <span class="tex-span"><i>l</i>, <i>r</i></span> and <span class="tex-span"><i>k</i></span> and you should tell him the number </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://CLP6yreo.png" style="max-width: 100.0%;max-height: 100.0%;"></center></div><div class="input-specification"><p>The first line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 × 10<sup class="upper-index">5</sup></span> and <span class="tex-span">1 ≤ <i>q</i> ≤ 5 × 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the phone numbers, <span class="tex-span"><i>i</i></span>-th line contains a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> consisting of lowercase English letters (<img align="middle" class="tex-formula" src="file://NRUyb6tb.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the information about the questions, each of them contains integers <span class="tex-span"><i>l</i>, <i>r</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print the answer for each question in a separate line.</p></div>

## Input

<p>The first line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 × 10<sup class="upper-index">5</sup></span> and <span class="tex-span">1 ≤ <i>q</i> ≤ 5 × 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the phone numbers, <span class="tex-span"><i>i</i></span>-th line contains a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> consisting of lowercase English letters (<img align="middle" class="tex-formula" src="file://NRUyb6tb.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the information about the questions, each of them contains integers <span class="tex-span"><i>l</i>, <i>r</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>).</p>

## Output

<p>Print the answer for each question in a separate line.</p>





```input1
5 5
a
ab
abab
ababab
b
1 5 1
3 5 1
1 5 2
1 5 3
1 4 5

```




```output1
7
5
6
3
6

```


