## Description

<div><p>School holidays come in Berland. The holidays are going to continue for <span class="tex-span"><i>n</i></span> days. The students of school №<span class="tex-span"><i>N</i></span> are having the time of their lives and the IT teacher Marina Sergeyevna, who has spent all the summer busy checking the BSE (Berland State Examination) results, has finally taken a vacation break! Some people are in charge of the daily watering of flowers in shifts according to the schedule. However when Marina Sergeyevna was making the schedule, she was so tired from work and so lost in dreams of the oncoming vacation that she perhaps made several mistakes. In fact, it is possible that according to the schedule, on some days during the holidays the flowers will not be watered or will be watered multiple times. Help Marina Sergeyevna to find a mistake.</p></div><div class="input-specification"><p>The first input line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of days in Berland holidays and the number of people in charge of the watering respectively. The next <span class="tex-span"><i>m</i></span> lines contain the description of the duty schedule. Each line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), meaning that the <span class="tex-span"><i>i</i></span>-th person in charge should water the flowers from the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th to the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-th day inclusively, once a day. The duty shifts are described sequentially, i.e. <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span> inclusively. </p></div><div class="output-specification"><p>Print "OK" (without quotes), if the schedule does not contain mistakes. Otherwise you have to find the minimal number of a day when the flowers will not be watered or will be watered multiple times, and output two integers — the day number and the number of times the flowers will be watered that day.</p></div>

## Input

<p>The first input line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of days in Berland holidays and the number of people in charge of the watering respectively. The next <span class="tex-span"><i>m</i></span> lines contain the description of the duty schedule. Each line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), meaning that the <span class="tex-span"><i>i</i></span>-th person in charge should water the flowers from the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th to the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-th day inclusively, once a day. The duty shifts are described sequentially, i.e. <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span> inclusively. </p>

## Output

<p>Print "OK" (without quotes), if the schedule does not contain mistakes. Otherwise you have to find the minimal number of a day when the flowers will not be watered or will be watered multiple times, and output two integers — the day number and the number of times the flowers will be watered that day.</p>





```input1
10 5
1 2
3 3
4 6
7 7
8 10

```




```input2
10 5
1 2
2 3
4 5
7 8
9 10

```




```input3
10 5
1 2
3 3
5 7
7 7
7 10

```




```output1
OK

```




```output2
2 2

```




```output3
4 0

```



## Note

<p>Keep in mind that in the second sample the mistake occurs not only on the second day, but also on the sixth day, when nobody waters the flowers. However, you have to print the second day, i.e. the day with the minimal number.</p>
