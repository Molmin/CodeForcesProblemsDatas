## Description

<div><p>Piegirl has found a monster and a book about monsters and pies. When she is reading the book, she found out that there are <span class="tex-span"><i>n</i></span> types of monsters, each with an ID between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>. If you feed a pie to a monster, the monster will split into some number of monsters (possibly zero), and at least one colorful diamond. Monsters may be able to split in multiple ways.</p><p>At the begining Piegirl has exactly one monster. She begins by feeding the monster a pie. She continues feeding pies to monsters until no more monsters are left. Then she collects all the diamonds that were created.</p><p>You will be given a list of split rules describing the way in which the various monsters can split. Every monster can split in at least one way, and if a monster can split in multiple ways then each time when it splits Piegirl can choose the way it splits.</p><p>For each monster, determine the smallest and the largest number of diamonds Piegirl can possibly collect, if initially she has a single instance of that monster. Piegirl has an unlimited supply of pies.</p></div><div class="input-specification"><p>The first line contains two integers: <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of possible splits and the number of different monster types. Each of the following <span class="tex-span"><i>m</i></span> lines contains a split rule. Each split rule starts with an integer (a monster ID) <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), and a positive integer <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> indicating the number of monsters and diamonds the current monster can split into. This is followed by <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> integers, with positive integers representing a monster ID and <span class="tex-font-style-tt">-1</span> representing a diamond.</p><p>Each monster will have at least one split rule. Each split rule will have at least one diamond. The sum of <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> across all split rules will be at most <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>For each monster, in order of their IDs, print a line with two integers: the smallest and the largest number of diamonds that can possibly be collected by starting with that monster. If Piegirl cannot possibly end up in a state without monsters, print <span class="tex-font-style-tt">-1</span> for both smallest and the largest value. If she can collect an arbitrarily large number of diamonds, print <span class="tex-font-style-tt">-2</span> as the largest number of diamonds. </p><p>If any number in output exceeds <span class="tex-span">314000000</span> (but is finite), print <span class="tex-span">314000000</span> instead of that number.</p></div>

## Input

<p>The first line contains two integers: <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of possible splits and the number of different monster types. Each of the following <span class="tex-span"><i>m</i></span> lines contains a split rule. Each split rule starts with an integer (a monster ID) <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), and a positive integer <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> indicating the number of monsters and diamonds the current monster can split into. This is followed by <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> integers, with positive integers representing a monster ID and <span class="tex-font-style-tt">-1</span> representing a diamond.</p><p>Each monster will have at least one split rule. Each split rule will have at least one diamond. The sum of <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> across all split rules will be at most <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>For each monster, in order of their IDs, print a line with two integers: the smallest and the largest number of diamonds that can possibly be collected by starting with that monster. If Piegirl cannot possibly end up in a state without monsters, print <span class="tex-font-style-tt">-1</span> for both smallest and the largest value. If she can collect an arbitrarily large number of diamonds, print <span class="tex-font-style-tt">-2</span> as the largest number of diamonds. </p><p>If any number in output exceeds <span class="tex-span">314000000</span> (but is finite), print <span class="tex-span">314000000</span> instead of that number.</p>





```input1
6 4
1 3 -1 1 -1
1 2 -1 -1
2 3 -1 3 -1
2 3 -1 -1 -1
3 2 -1 -1
4 2 4 -1

```




```input2
3 2
1 2 1 -1
2 2 -1 -1
2 3 2 1 -1

```




```output1
2 -2
3 4
2 2
-1 -1

```




```output2
-1 -1
2 2

```


