## Description

<div><p>It was recycling day in Kekoland. To celebrate it Adil and Bera went to Central Perk where they can take bottles from the ground and put them into a recycling bin.</p><p>We can think Central Perk as coordinate plane. There are <span class="tex-span"><i>n</i></span> bottles on the ground, the <span class="tex-span"><i>i</i></span>-th bottle is located at position <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. Both Adil and Bera can carry only one bottle at once each. </p><p>For both Adil and Bera the process looks as follows: </p><ol> <li> Choose to stop or to continue to collect bottles. </li><li> If the choice was to continue then choose some bottle and walk towards it. </li><li> Pick this bottle and walk to the recycling bin. </li><li> Go to step <span class="tex-span">1</span>. </li></ol><p>Adil and Bera may move independently. They are allowed to pick bottles simultaneously, all bottles may be picked by any of the two, it's allowed that one of them stays still while the other one continues to pick bottles.</p><p>They want to organize the process such that the total distance they walk (the sum of distance walked by Adil and distance walked by Bera) is minimum possible. Of course, at the end all bottles should lie in the recycling bin.</p></div><div class="input-specification"><p>First line of the input contains six integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>y</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>y</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>x</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>y</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>x</i></sub>, <i>a</i><sub class="lower-index"><i>y</i></sub>, <i>b</i><sub class="lower-index"><i>x</i></sub>, <i>b</i><sub class="lower-index"><i>y</i></sub>, <i>t</i><sub class="lower-index"><i>x</i></sub>, <i>t</i><sub class="lower-index"><i>y</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— initial positions of Adil, Bera and recycling bin respectively.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of bottles on the ground.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each of them contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— position of the <span class="tex-span"><i>i</i></span>-th bottle.</p><p>It's guaranteed that positions of Adil, Bera, recycling bin and all bottles are distinct.</p></div><div class="output-specification"><p>Print one real number&nbsp;— the minimum possible total distance Adil and Bera need to walk in order to put all bottles into recycling bin. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://rYeuCFf2.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>First line of the input contains six integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>y</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>y</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>x</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>y</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>x</i></sub>, <i>a</i><sub class="lower-index"><i>y</i></sub>, <i>b</i><sub class="lower-index"><i>x</i></sub>, <i>b</i><sub class="lower-index"><i>y</i></sub>, <i>t</i><sub class="lower-index"><i>x</i></sub>, <i>t</i><sub class="lower-index"><i>y</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— initial positions of Adil, Bera and recycling bin respectively.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of bottles on the ground.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each of them contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— position of the <span class="tex-span"><i>i</i></span>-th bottle.</p><p>It's guaranteed that positions of Adil, Bera, recycling bin and all bottles are distinct.</p>

## Output

<p>Print one real number&nbsp;— the minimum possible total distance Adil and Bera need to walk in order to put all bottles into recycling bin. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://rYeuCFf2.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 1 1 2 0 0
3
1 1
2 1
2 3

```




```input2
5 0 4 2 2 0
5
5 2
3 0
5 5
3 5
3 3

```




```output1
11.084259940083

```




```output2
33.121375178000

```



## Note

<p>Consider the first sample.</p><p>Adil will use the following path: <img align="middle" class="tex-formula" src="file://gUSt8hjA.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Bera will use the following path: <img align="middle" class="tex-formula" src="file://g4eKuUMZ.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Adil's path will be <img align="middle" class="tex-formula" src="file://M4uBKGQc.png" style="max-width: 100.0%;max-height: 100.0%;"> units long, while Bera's path will be <img align="middle" class="tex-formula" src="file://PpQQv4mm.png" style="max-width: 100.0%;max-height: 100.0%;"> units long.</p>
