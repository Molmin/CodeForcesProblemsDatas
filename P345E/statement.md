## Description

<div><p>Today you go out of your house and immediately notice that something is weird. Around your door there is a swarm of black cats — all tense paws and twitching tails. As you do your first step, they all dart off and start running towards you. It looks like they want to thwart you!</p><p>You are moving in a straight line from point <span class="tex-span">(0, 0)</span> to point <span class="tex-span">(<i>a</i>, 0)</span> with velocity <span class="tex-span"><i>v</i></span>. There are <span class="tex-span"><i>n</i></span> black cats around you who want to cross your paths. A cat can move in any direction with velocity at most <span class="tex-span"><i>u</i></span>. A cat assumes it has crossed your path if it managed to get to at least one point of your path earlier or at the same time as you got there.</p><p>You are given four integers: <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>n</i></span>, as well as cats' coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. What is the greatest number of cats who manage to cross your path?</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ 10000;&nbsp;1 ≤ <i>v</i>, <i>u</i> ≤ 100;&nbsp;1 ≤ <i>n</i> ≤ 1000)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 100 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — location of the <span class="tex-span"><i>i</i></span>-th cat.</p><p>It's guaranteed that all cats are located in distinct points.</p></div><div class="output-specification"><p>Output a single integer — what is the greatest number of cats who manage to cross your path?</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ 10000;&nbsp;1 ≤ <i>v</i>, <i>u</i> ≤ 100;&nbsp;1 ≤ <i>n</i> ≤ 1000)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 100 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — location of the <span class="tex-span"><i>i</i></span>-th cat.</p><p>It's guaranteed that all cats are located in distinct points.</p>

## Output

<p>Output a single integer — what is the greatest number of cats who manage to cross your path?</p>





```input1
1 1 5 4
0 3
4 -4
7 0
-2 -2

```




```input2
10 5 3 4
7 5
5 2
10 -7
15 0

```




```output1
3

```




```output2
3

```


