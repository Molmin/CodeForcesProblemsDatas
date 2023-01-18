## Description

<div><p>Gleb is a famous competitive programming teacher from Innopolis. He is planning a trip to <span class="tex-span"><i>N</i></span> programming camps in the nearest future. Each camp will be held in a different country. For each of them, Gleb needs to apply for a visa. </p><p>For each of these trips Gleb knows three integers: the number of the first day of the trip <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, the length of the trip in days <span class="tex-span"><i>len</i><sub class="lower-index"><i>i</i></sub></span>, and the number of days <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> this country's consulate will take to process a visa application and stick a visa in a passport. Gleb has <span class="tex-span"><i>P</i></span> (<span class="tex-span">1 ≤ <i>P</i> ≤ 2</span>) valid passports and is able to decide which visa he wants to put in which passport.</p><p>For each trip, Gleb will have a flight to that country early in the morning of the day <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and will return back late in the evening of the day <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> + <i>len</i><sub class="lower-index"><i>i</i></sub> - 1</span>.</p><p>To apply for a visa on the day <span class="tex-span"><i>d</i></span>, Gleb needs to be in Innopolis in the middle of this day. So he can't apply for a visa while he is on a trip, including the first and the last days. If a trip starts the next day after the end of the other one, Gleb can't apply for a visa between them as well. The earliest Gleb can apply for a visa is day 1.</p><p>After applying for a visa of country <span class="tex-span"><i>i</i></span> on day <span class="tex-span"><i>d</i></span>, Gleb will get his passport back in the middle of the day <span class="tex-span"><i>d</i> + <i>t</i><sub class="lower-index"><i>i</i></sub></span>. Consulates use delivery services, so Gleb can get his passport back even if he is not in Innopolis on this day. Gleb can apply for another visa on the same day he received his passport back, if he is in Innopolis this day. </p><p>Gleb will not be able to start his trip on day <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> if he doesn't has a passport with a visa for the corresponding country in the morning of day <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. In particular, the passport should not be in another country's consulate for visa processing.</p><p>Help Gleb to decide which visas he needs to receive in which passport, and when he should apply for each visa. </p></div><div class="input-specification"><p>In the first line of the input there are two integers <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 22</span>) and <span class="tex-span"><i>P</i></span> (<span class="tex-span">1 ≤ <i>P</i> ≤ 2</span>)—the number of trips and the number of passports Gleb has, respectively.</p><p>The next <span class="tex-span"><i>N</i></span> lines describe Gleb's trips. Each line contains three positive integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>len</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>len</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)—the first day of the trip, the length of the trip and number of days the consulate of this country needs to process a visa application. It is guaranteed that no two trips intersect.</p></div><div class="output-specification"><p>If it is impossible to get all visas on time, just print "NO" (quotes for clarity). Otherwise, print "YES" and <span class="tex-span"><i>N</i></span> lines describing trips. For each trip, first print number of the passport Gleb should put this country's visa in, and then print number of the day he should apply for it. Print trips in the same order as they appear in the input. Days are numbered from 1, starting with tomorrow—the first day you can apply for a visa. Passports are numbered from 1 to <span class="tex-span"><i>P</i></span>.</p><p>If there are several possible answers, print any of them.</p></div>

## Input

<p>In the first line of the input there are two integers <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 22</span>) and <span class="tex-span"><i>P</i></span> (<span class="tex-span">1 ≤ <i>P</i> ≤ 2</span>)—the number of trips and the number of passports Gleb has, respectively.</p><p>The next <span class="tex-span"><i>N</i></span> lines describe Gleb's trips. Each line contains three positive integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>len</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>len</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)—the first day of the trip, the length of the trip and number of days the consulate of this country needs to process a visa application. It is guaranteed that no two trips intersect.</p>

## Output

<p>If it is impossible to get all visas on time, just print "NO" (quotes for clarity). Otherwise, print "YES" and <span class="tex-span"><i>N</i></span> lines describing trips. For each trip, first print number of the passport Gleb should put this country's visa in, and then print number of the day he should apply for it. Print trips in the same order as they appear in the input. Days are numbered from 1, starting with tomorrow—the first day you can apply for a visa. Passports are numbered from 1 to <span class="tex-span"><i>P</i></span>.</p><p>If there are several possible answers, print any of them.</p>





```input1
2 1
3 1 1
6 1 1

```




```input2
3 1
13 2 2
7 3 1
19 3 4

```




```input3
7 2
15 1 1
14 1 1
18 1 1
21 1 1
9 4 6
22 2 5
5 4 3

```




```input4
3 1
7 3 1
13 2 3
19 3 4

```




```output1
YES
1 1
1 4

```




```output2
YES
1 10
1 1
1 2

```




```output3
YES
2 13
1 1
1 16
1 19
1 2
2 16
2 1

```




```output4
NO

```



## Note

<p>Examples with answer "YES" are depicted below.</p><p>Each cell of the stripe represents a single day. Rectangles represent trips, each trip starts in the morning and ends in the evening. Rectangles with angled corners represent visa applications. Each application starts in the middle of a day and ends <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> days after. The trip and the visa application for the same country have the same color.</p><p>In examples with two passports, visa applications and trips depicted above the time stripe are made using the first passport, visa applications and trips depicted below the time stripe are made using the second passport.</p><p><span class="tex-font-style-bf">Example 1</span>: </p><center> <img class="tex-graphics" src="file://C4jc2fLg.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p><span class="tex-font-style-bf">Example 2</span>: </p><center> <img class="tex-graphics" src="file://uGuadsan.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p><span class="tex-font-style-bf">Example 3</span>: </p><center> <img class="tex-graphics" src="file://NZNNj6HP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
