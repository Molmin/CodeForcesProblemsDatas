## Description

<div><p>Anya loves to watch horror movies. In the best traditions of horror, she will be visited by <span class="tex-span"><i>m</i></span> ghosts tonight. Anya has lots of candles prepared for the visits, each candle can produce light for exactly <span class="tex-span"><i>t</i></span> seconds. It takes the girl one second to light one candle. More formally, Anya can spend one second to light one candle, then this candle burns for exactly <span class="tex-span"><i>t</i></span> seconds and then goes out and can no longer be used.</p><p>For each of the <span class="tex-span"><i>m</i></span> ghosts Anya knows the time at which it comes: the <span class="tex-span"><i>i</i></span>-th visit will happen <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> seconds after midnight, all <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>'s are distinct. Each visit lasts exactly one second.</p><p>What is the minimum number of candles Anya should use so that during each visit, at least <span class="tex-span"><i>r</i></span> candles are burning? Anya can start to light a candle at any time that is integer number of seconds from midnight, possibly, at the time before midnight. <span class="tex-font-style-bf">That means, she can start to light a candle integer number of seconds before midnight or integer number of seconds after a midnight, or in other words in any integer moment of time.</span></p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>t</i>, <i>r</i> ≤ 300</span>), representing the number of ghosts to visit Anya, the duration of a candle's burning and the minimum number of candles that should burn during each visit. </p><p>The next line contains <span class="tex-span"><i>m</i></span> space-separated numbers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 300</span>), the <span class="tex-span"><i>i</i></span>-th of them repesents at what second after the midnight the <span class="tex-span"><i>i</i></span>-th ghost will come. All <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>'s are distinct, they follow in the strictly increasing order.</p></div><div class="output-specification"><p>If it is possible to make at least <span class="tex-span"><i>r</i></span> candles burn during each visit, then print the minimum number of candles that Anya needs to light for that.</p><p>If that is impossible, print <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>t</i>, <i>r</i> ≤ 300</span>), representing the number of ghosts to visit Anya, the duration of a candle's burning and the minimum number of candles that should burn during each visit. </p><p>The next line contains <span class="tex-span"><i>m</i></span> space-separated numbers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 300</span>), the <span class="tex-span"><i>i</i></span>-th of them repesents at what second after the midnight the <span class="tex-span"><i>i</i></span>-th ghost will come. All <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>'s are distinct, they follow in the strictly increasing order.</p>

## Output

<p>If it is possible to make at least <span class="tex-span"><i>r</i></span> candles burn during each visit, then print the minimum number of candles that Anya needs to light for that.</p><p>If that is impossible, print <span class="tex-span"> - 1</span>.</p>





```input1
1 8 3
10

```




```input2
2 10 1
5 8

```




```input3
1 1 3
10

```




```output1
3

```




```output2
1

```




```output3
-1

```



## Note

<p><span class="tex-font-style-bf">Anya can start lighting a candle in the same second with ghost visit. But this candle isn't counted as burning at this visit.</span></p><p>It takes exactly one second to light up a candle and only after that second this candle is considered burning; it means that if Anya starts lighting candle at moment x, candle is buring from second x + 1 to second x + t inclusively.</p><p>In the first sample test three candles are enough. For example, Anya can start lighting them at the <span class="tex-span">3</span>-rd, <span class="tex-span">5</span>-th and <span class="tex-span">7</span>-th seconds after the midnight.</p><p>In the second sample test one candle is enough. For example, Anya can start lighting it one second before the midnight.</p><p>In the third sample test the answer is <span class="tex-span"> - 1</span>, since during each second at most one candle can burn but Anya needs three candles to light up the room at the moment when the ghost comes.</p>
