## Description

<div><p>Jon Snow now has to fight with White Walkers. He has <span class="tex-span"><i>n</i></span> rangers, each of which has his own strength. Also Jon Snow has his favourite number <span class="tex-span"><i>x</i></span>. Each ranger can fight with a white walker only if the strength of the white walker equals his strength. He however thinks that his rangers are weak and need to improve. Jon now thinks that if he takes the bitwise XOR of strengths of some of rangers with his favourite number <span class="tex-span"><i>x</i></span>, he might get soldiers of high strength. So, he decided to do the following operation <span class="tex-span"><i>k</i></span> times: </p><ol><li> Arrange all the rangers in a straight line in the order of increasing strengths.</li><li> Take the bitwise XOR (is written as <img align="middle" class="tex-formula" src="file://GrRP9faX.png" style="max-width: 100.0%;max-height: 100.0%;">) of the strength of each alternate ranger with <span class="tex-span"><i>x</i></span> and update it's strength.</li></ol> Suppose, Jon has <span class="tex-span">5</span> rangers with strengths <span class="tex-span">[9, 7, 11, 15, 5]</span> and he performs the operation <span class="tex-span">1</span> time with <span class="tex-span"><i>x</i> = 2</span>. He first arranges them in the order of their strengths, <span class="tex-span">[5, 7, 9, 11, 15]</span>. Then he does the following: <ol><li> The strength of first ranger is updated to <img align="middle" class="tex-formula" src="file://xdGlflBe.png" style="max-width: 100.0%;max-height: 100.0%;">, i.e. <span class="tex-span">7</span>.</li><li> The strength of second ranger remains the same, i.e. <span class="tex-span">7</span>.</li><li> The strength of third ranger is updated to <img align="middle" class="tex-formula" src="file://Nb9oPIgC.png" style="max-width: 100.0%;max-height: 100.0%;">, i.e. <span class="tex-span">11</span>.</li><li> The strength of fourth ranger remains the same, i.e. <span class="tex-span">11</span>.</li><li> The strength of fifth ranger is updated to <img align="middle" class="tex-formula" src="file://nXXAywQI.png" style="max-width: 100.0%;max-height: 100.0%;">, i.e. <span class="tex-span">13</span>.</li></ol> The new strengths of the <span class="tex-span">5</span> rangers are <span class="tex-span">[7, 7, 11, 11, 13]</span><p>Now, Jon wants to know the maximum and minimum strength of the rangers after performing the above operations <span class="tex-span"><i>k</i></span> times. He wants your help for this task. Can you help him?</p></div><div class="input-specification"><p>First line consists of three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">3</sup></span>) — number of rangers Jon has, the number of times Jon will carry out the operation and Jon's favourite number respectively.</p><p>Second line consists of <span class="tex-span"><i>n</i></span> integers representing the strengths of the rangers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup></span>).</p></div><div class="output-specification"><p>Output two integers, the maximum and the minimum strength of the rangers after performing the operation <span class="tex-span"><i>k</i></span> times.</p></div>

## Input

<p>First line consists of three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">3</sup></span>) — number of rangers Jon has, the number of times Jon will carry out the operation and Jon's favourite number respectively.</p><p>Second line consists of <span class="tex-span"><i>n</i></span> integers representing the strengths of the rangers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup></span>).</p>

## Output

<p>Output two integers, the maximum and the minimum strength of the rangers after performing the operation <span class="tex-span"><i>k</i></span> times.</p>





```input1
5 1 2
9 7 11 15 5

```




```input2
2 100000 569
605 986

```




```output1
13 7
```




```output2
986 605
```


