## Description

<div><p>A long time ago (probably even in the first book), Nicholas Flamel, a great alchemist and the creator of the Philosopher's Stone, taught Harry Potter three useful spells. The first one allows you to convert <span class="tex-span"><i>a</i></span> grams of sand into <span class="tex-span"><i>b</i></span> grams of lead, the second one allows you to convert <span class="tex-span"><i>c</i></span> grams of lead into <span class="tex-span"><i>d</i></span> grams of gold and third one allows you to convert <span class="tex-span"><i>e</i></span> grams of gold into <span class="tex-span"><i>f</i></span> grams of sand. When Harry told his friends about these spells, Ron Weasley was amazed. After all, if they succeed in turning sand into lead, lead into gold, and then turning part of the gold into sand again and so on, then it will be possible to start with a small amount of sand and get huge amounts of gold! Even an infinite amount of gold! Hermione Granger, by contrast, was skeptical about that idea. She argues that according to the law of conservation of matter getting an infinite amount of matter, even using magic, is impossible. On the contrary, the amount of matter may even decrease during transformation, being converted to magical energy. Though Hermione's theory seems convincing, Ron won't believe her. As far as Ron is concerned, Hermione made up her law of conservation of matter to stop Harry and Ron wasting their time with this nonsense, and to make them go and do homework instead. That's why Ron has already collected a certain amount of sand for the experiments. A quarrel between the friends seems unavoidable...</p><p>Help Harry to determine which one of his friends is right, and avoid the quarrel after all. To do this you have to figure out whether it is possible to get the amount of gold greater than any preassigned number from some finite amount of sand.</p></div><div class="input-specification"><p>The first line contains <span class="tex-span">6</span> integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>e</i></span>, <span class="tex-span"><i>f</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i>, <i>e</i>, <i>f</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>Print "Ron", if it is possible to get an infinitely large amount of gold having a certain finite amount of sand (and not having any gold and lead at all), i.e., Ron is right. Otherwise, print "Hermione".</p></div>

## Input

<p>The first line contains <span class="tex-span">6</span> integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>e</i></span>, <span class="tex-span"><i>f</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i>, <i>e</i>, <i>f</i> ≤ 1000</span>).</p>

## Output

<p>Print "Ron", if it is possible to get an infinitely large amount of gold having a certain finite amount of sand (and not having any gold and lead at all), i.e., Ron is right. Otherwise, print "Hermione".</p>





```input1
100 200 250 150 200 250

```




```input2
100 50 50 200 200 100

```




```input3
100 10 200 20 300 30

```




```input4
0 0 0 0 0 0

```




```input5
1 1 0 1 1 1

```




```input6
1 0 1 2 1 2

```




```input7
100 1 100 1 0 1

```




```output1
Ron

```




```output2
Hermione

```




```output3
Hermione

```




```output4
Hermione

```




```output5
Ron

```




```output6
Hermione

```




```output7
Ron

```



## Note

<p>Consider the first sample. Let's start with the <span class="tex-span">500</span> grams of sand. Apply the first spell <span class="tex-span">5</span> times and turn the sand into <span class="tex-span">1000</span> grams of lead. Then apply the second spell <span class="tex-span">4</span> times to get <span class="tex-span">600</span> grams of gold. Let’s take <span class="tex-span">400</span> grams from the resulting amount of gold turn them back into sand. We get <span class="tex-span">500</span> grams of sand and <span class="tex-span">200</span> grams of gold. If we apply the same operations to <span class="tex-span">500</span> grams of sand again, we can get extra <span class="tex-span">200</span> grams of gold every time. Thus, you can get <span class="tex-span">200</span>, <span class="tex-span">400</span>, <span class="tex-span">600</span> etc. grams of gold, i.e., starting with a finite amount of sand (<span class="tex-span">500</span> grams), you can get the amount of gold which is greater than any preassigned number.</p><p>In the forth sample it is impossible to get sand, or lead, or gold, applying the spells.</p><p>In the fifth sample an infinitely large amount of gold can be obtained by using only the second spell, which allows you to receive <span class="tex-span">1</span> gram of gold out of nothing. Note that if such a second spell is available, then the first and the third one do not affect the answer at all.</p><p>The seventh sample is more interesting. We can also start with a zero amount of sand there. With the aid of the third spell you can get sand out of nothing. We get <span class="tex-span">10000</span> grams of sand in this manner. Let's get <span class="tex-span">100</span> grams of lead using the first spell <span class="tex-span">100</span> times. Then make <span class="tex-span">1</span> gram of gold from them. We managed to receive <span class="tex-span">1</span> gram of gold, starting with a zero amount of sand! Clearly, in this manner you can get an infinitely large amount of gold.</p>
