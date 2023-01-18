## Description

<div><p>Do you remember a kind cartoon "Beauty and the Beast"? No, no, there was no firing from machine guns or radiation mutants time-travels!</p><p>There was a beauty named Belle. Once she had violated the Beast's order and visited the West Wing. After that she was banished from the castle... </p><p>Everybody was upset. The beautiful Belle was upset, so was the Beast, so was Lumiere the candlestick. But the worst thing was that Cogsworth was upset. Cogsworth is not a human, but is the mantel clock, which was often used as an alarm clock.</p><p>Due to Cogsworth's frustration all the inhabitants of the castle were in trouble: now they could not determine when it was time to drink morning tea, and when it was time for an evening stroll. </p><p>Fortunately, deep in the basement are lying digital clock showing the time in the format <span class="tex-font-style-tt">HH:MM</span>. Now the residents of the castle face a difficult task. They should turn Cogsworth's hour and minute mustache hands in such a way, that Cogsworth began to show the correct time. Moreover they need to find turn angles in degrees for each mustache hands. The initial time showed by Cogsworth is <span class="tex-font-style-tt">12:00</span>.</p><p>You can only rotate the hands forward, that is, as is shown in the picture: </p><center> <img class="tex-graphics" src="file://20j9mzgH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>As since there are many ways too select such angles because of full rotations, choose the smallest angles in the right (non-negative) direction.</p><p>Note that Cogsworth's hour and minute mustache hands move evenly and continuously. Hands are moving independently, so when turning one hand the other hand remains standing still.</p></div><div class="input-specification"><p>The only line of input contains current time according to the digital clock, formatted as <span class="tex-font-style-tt">HH:MM</span> (<span class="tex-span">00 ≤ </span><span class="tex-font-style-tt">HH</span><span class="tex-span"> ≤ 23</span>, <span class="tex-span">00 ≤ </span><span class="tex-font-style-tt">MM</span><span class="tex-span"> ≤ 59</span>). The mantel clock initially shows <span class="tex-font-style-tt">12:00</span>.</p><p>Pretests contain times of the beginning of some morning TV programs of the Channel One Russia.</p></div><div class="output-specification"><p>Print two numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> — the angles of turning the hour and minute hands, respectively (<span class="tex-span">0 ≤ <i>x</i>, <i>y</i> &lt; 360</span>). The absolute or relative error in the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The only line of input contains current time according to the digital clock, formatted as <span class="tex-font-style-tt">HH:MM</span> (<span class="tex-span">00 ≤ </span><span class="tex-font-style-tt">HH</span><span class="tex-span"> ≤ 23</span>, <span class="tex-span">00 ≤ </span><span class="tex-font-style-tt">MM</span><span class="tex-span"> ≤ 59</span>). The mantel clock initially shows <span class="tex-font-style-tt">12:00</span>.</p><p>Pretests contain times of the beginning of some morning TV programs of the Channel One Russia.</p>

## Output

<p>Print two numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> — the angles of turning the hour and minute hands, respectively (<span class="tex-span">0 ≤ <i>x</i>, <i>y</i> &lt; 360</span>). The absolute or relative error in the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
12:00

```




```input2
04:30

```




```input3
08:17

```




```output1
0 0
```




```output2
135 180
```




```output3
248.5 102
```



## Note

<p><span class="tex-font-style-bf">A note to the second example:</span> the hour hand will be positioned exactly in the middle, between 4 and 5.</p>
