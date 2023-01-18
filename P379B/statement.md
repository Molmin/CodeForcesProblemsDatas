## Description

<div><p>The New Year is coming! That's why many people today are busy preparing New Year presents. Vasily the Programmer is no exception.</p><p>Vasily knows that the best present is (no, it's not a contest) money. He's put <span class="tex-span"><i>n</i></span> empty wallets from left to right in a row and decided how much money to put in what wallet. Vasily decided to put <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> coins to the <span class="tex-span"><i>i</i></span>-th wallet from the left.</p><p>Vasily is a very busy man, so the money are sorted into the bags by his robot. Initially, the robot stands by the leftmost wallet in the row. The robot can follow instructions of three types: go to the wallet that is to the left of the current one (if such wallet exists), go to the wallet that is to the right of the current one (if such wallet exists), put a coin to the current wallet. Due to some technical malfunctions the robot cannot follow two "put a coin" instructions in a row.</p><p>Vasily doesn't want to wait for long, so he wants to write a program for the robot that contains at most <span class="tex-span">10<sup class="upper-index">6</sup></span> operations (not necessarily minimum in length) the robot can use to put coins into the wallets. Help him.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 300)</span> — the number of wallets. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 300)</span>.</p><p>It is guaranteed that at least one <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is positive.</p></div><div class="output-specification"><p>Print the sequence that consists of <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup>)</span> characters, each of them equals: "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>" or "<span class="tex-font-style-tt">P</span>". Each character of the sequence is an instruction to the robot. Character "<span class="tex-font-style-tt">L</span>" orders to move to the left, character "<span class="tex-font-style-tt">R</span>" orders to move to the right, character "<span class="tex-font-style-tt">P</span>" orders the robot to put a coin in the wallet. The robot is not allowed to go beyond the wallet line. In other words, you cannot give instructions "<span class="tex-font-style-tt">L</span>" if the robot is at wallet 1, or "<span class="tex-font-style-tt">R</span>" at wallet <span class="tex-span"><i>n</i></span>.</p><p>As a result of the performed operations, the <span class="tex-span"><i>i</i></span>-th wallet from the left must contain exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> coins. If there are multiple answers, you can print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 300)</span> — the number of wallets. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 300)</span>.</p><p>It is guaranteed that at least one <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is positive.</p>

## Output

<p>Print the sequence that consists of <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup>)</span> characters, each of them equals: "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>" or "<span class="tex-font-style-tt">P</span>". Each character of the sequence is an instruction to the robot. Character "<span class="tex-font-style-tt">L</span>" orders to move to the left, character "<span class="tex-font-style-tt">R</span>" orders to move to the right, character "<span class="tex-font-style-tt">P</span>" orders the robot to put a coin in the wallet. The robot is not allowed to go beyond the wallet line. In other words, you cannot give instructions "<span class="tex-font-style-tt">L</span>" if the robot is at wallet 1, or "<span class="tex-font-style-tt">R</span>" at wallet <span class="tex-span"><i>n</i></span>.</p><p>As a result of the performed operations, the <span class="tex-span"><i>i</i></span>-th wallet from the left must contain exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> coins. If there are multiple answers, you can print any of them.</p>





```input1
2
1 2

```




```input2
4
0 2 0 2

```




```output1
PRPLRP
```




```output2
RPRRPLLPLRRRP
```


