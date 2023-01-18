## Description

<div><p><span class="tex-font-style-it">This is simplified version of the problem used on the original contest. The original problem seems to have too difiicult solution. The constraints for input data have been reduced.</span></p><p>Polycarp likes to play computer role-playing game «Lizards and Basements». At the moment he is playing it as a magician. At one of the last levels he has to fight the line of archers. The only spell with which he can damage them is a fire ball. If Polycarp hits the <span class="tex-span"><i>i</i></span>-th archer with his fire ball (they are numbered from left to right), the archer loses <span class="tex-span"><i>a</i></span> health points. At the same time the spell damages the archers adjacent to the <span class="tex-span"><i>i</i></span>-th (if any) — they lose <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> &lt; <i>a</i> ≤ 10</span>) health points each.</p><p>As the extreme archers (i.e. archers numbered 1 and <span class="tex-span"><i>n</i></span>) are very far, the fire ball cannot reach them. Polycarp can hit any other archer with his fire ball.</p><p>The amount of health points for each archer is known. An archer will be killed when this amount is less than 0. What is the minimum amount of spells Polycarp can use to kill all the enemies?</p><p>Polycarp can throw his fire ball into an archer if the latter is already killed.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i>, <i>a</i>, <i>b</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10</span>; <span class="tex-span">1 ≤ <i>b</i> &lt; <i>a</i> ≤ 10</span>). The second line contains a sequence of <span class="tex-span"><i>n</i></span> integers — <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 15</span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the amount of health points the <span class="tex-span"><i>i</i></span>-th archer has.</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>t</i></span> — the required minimum amount of fire balls.</p><p>In the second line print <span class="tex-span"><i>t</i></span> numbers — indexes of the archers that Polycarp should hit to kill all the archers in <span class="tex-span"><i>t</i></span> shots. All these numbers should be between 2 and <span class="tex-span"><i>n</i> - 1</span>. Separate numbers with spaces. If there are several solutions, output any of them. Print numbers in any order.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i>, <i>a</i>, <i>b</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10</span>; <span class="tex-span">1 ≤ <i>b</i> &lt; <i>a</i> ≤ 10</span>). The second line contains a sequence of <span class="tex-span"><i>n</i></span> integers — <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 15</span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the amount of health points the <span class="tex-span"><i>i</i></span>-th archer has.</p>

## Output

<p>In the first line print <span class="tex-span"><i>t</i></span> — the required minimum amount of fire balls.</p><p>In the second line print <span class="tex-span"><i>t</i></span> numbers — indexes of the archers that Polycarp should hit to kill all the archers in <span class="tex-span"><i>t</i></span> shots. All these numbers should be between 2 and <span class="tex-span"><i>n</i> - 1</span>. Separate numbers with spaces. If there are several solutions, output any of them. Print numbers in any order.</p>





```input1
3 2 1
2 2 2

```




```input2
4 3 1
1 4 1 1

```




```output1
3
2 2 2
```




```output2
4
2 2 3 3
```


