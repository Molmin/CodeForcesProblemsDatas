## Description

<div><p>Once upon a time DravDe, an outstanding person famous for his professional achievements (as you must remember, he works in a warehouse storing Ogudar-Olok, a magical but non-alcoholic drink) came home after a hard day. That day he had to drink 9875 boxes of the drink and, having come home, he went to bed at once.</p><p>DravDe dreamt about managing a successful farm. He dreamt that every day one animal came to him and asked him to let it settle there. However, DravDe, being unimaginably kind, could send the animal away and it went, rejected. There were exactly <span class="tex-span"><i>n</i></span> days in DravDe’s dream and the animal that came on the <span class="tex-span"><i>i</i></span>-th day, ate exactly <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> tons of food daily starting from day <span class="tex-span"><i>i</i></span>. But if one day the animal could not get the food it needed, it got really sad. At the very beginning of the dream there were exactly <span class="tex-span"><i>X</i></span> tons of food on the farm.</p><p>DravDe woke up terrified...</p><p>When he retold the dream to you, he couldn’t remember how many animals were on the farm by the end of the <span class="tex-span"><i>n</i></span>-th day any more, but he did remember that nobody got sad (as it was a happy farm) and that there was the maximum possible amount of the animals. That’s the number he wants you to find out. </p><p>It should be noticed that the animals arrived in the morning and DravDe only started to feed them in the afternoon, so that if an animal willing to join them is rejected, it can’t eat any farm food. But if the animal does join the farm, it eats daily from that day to the <span class="tex-span"><i>n</i></span>-th.</p></div><div class="input-specification"><p>The first input line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>X</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 1 ≤ <i>X</i> ≤ 10<sup class="upper-index">4</sup></span>) — amount of days in DravDe’s dream and the total amount of food (in tons) that was there initially. The second line contains integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 300</span>). Numbers in the second line are divided by a space.</p></div><div class="output-specification"><p>Output the only number — the maximum possible amount of animals on the farm by the end of the <span class="tex-span"><i>n</i></span>-th day given that the food was enough for everybody.</p></div>

## Input

<p>The first input line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>X</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 1 ≤ <i>X</i> ≤ 10<sup class="upper-index">4</sup></span>) — amount of days in DravDe’s dream and the total amount of food (in tons) that was there initially. The second line contains integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 300</span>). Numbers in the second line are divided by a space.</p>

## Output

<p>Output the only number — the maximum possible amount of animals on the farm by the end of the <span class="tex-span"><i>n</i></span>-th day given that the food was enough for everybody.</p>





```input1
3 4
1 1 1

```




```input2
3 6
1 1 1

```




```output1
2

```




```output2
3

```



## Note

<p>Note to the first example: DravDe leaves the second and the third animal on the farm. The second animal will eat one ton of food on the second day and one ton on the third day. The third animal will eat one ton of food on the third day.</p>
