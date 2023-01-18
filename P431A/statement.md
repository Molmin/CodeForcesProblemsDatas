## Description

<div><p>Quite recently, a very smart student named Jury decided that lectures are boring, so he downloaded a game called "<span class="tex-font-style-tt">Black Square</span>" on his super cool touchscreen phone.</p><p>In this game, the phone's screen is divided into four vertical strips. Each second, a black square appears on some of the strips. According to the rules of the game, Jury must use this second to touch the corresponding strip to make the square go away. As Jury is both smart and lazy, he counted that he wastes exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> calories on touching the <span class="tex-span"><i>i</i></span>-th strip.</p><p>You've got a string <span class="tex-span"><i>s</i></span>, describing the process of the game and numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub></span>. Calculate how many calories Jury needs to destroy all the squares?</p></div><div class="input-specification"><p>The first line contains four space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>The second line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>), where the <span class="tex-span"><i>і</i></span>-th character of the string equals "<span class="tex-font-style-tt">1</span>", if on the <span class="tex-span"><i>i</i></span>-th second of the game the square appears on the first strip, "<span class="tex-font-style-tt">2</span>", if it appears on the second strip, "<span class="tex-font-style-tt">3</span>", if it appears on the third strip, "<span class="tex-font-style-tt">4</span>", if it appears on the fourth strip.</p></div><div class="output-specification"><p>Print a single integer — the total number of calories that Jury wastes.</p></div>

## Input

<p>The first line contains four space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>The second line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>), where the <span class="tex-span"><i>і</i></span>-th character of the string equals "<span class="tex-font-style-tt">1</span>", if on the <span class="tex-span"><i>i</i></span>-th second of the game the square appears on the first strip, "<span class="tex-font-style-tt">2</span>", if it appears on the second strip, "<span class="tex-font-style-tt">3</span>", if it appears on the third strip, "<span class="tex-font-style-tt">4</span>", if it appears on the fourth strip.</p>

## Output

<p>Print a single integer — the total number of calories that Jury wastes.</p>





```input1
1 2 3 4
123214

```




```input2
1 5 3 2
11221

```




```output1
13

```




```output2
13

```


