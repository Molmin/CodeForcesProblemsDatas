## Description

<div><p>Valeric and Valerko missed the last Euro football game, so they decided to watch the game's key moments on the Net. They want to start watching as soon as possible but the connection speed is too low. If they turn on the video right now, it will "hang up" as the size of data to watch per second will be more than the size of downloaded data per second.</p><p>The guys want to watch the whole video without any pauses, so they have to wait some <span class="tex-font-style-bf">integer</span> number of seconds for a part of the video to download. After this number of seconds passes, they can start watching. Waiting for the whole video to download isn't necessary as the video can download after the guys started to watch.</p><p>Let's suppose that video's length is <span class="tex-span"><i>c</i></span> seconds and Valeric and Valerko wait <span class="tex-span"><i>t</i></span> seconds before the watching. Then for any moment of time <span class="tex-span"><i>t</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>t</i> ≤ <i>t</i><sub class="lower-index">0</sub> ≤ <i>c</i> + <i>t</i></span>, the following condition must fulfill: the size of data received in <span class="tex-span"><i>t</i><sub class="lower-index">0</sub></span> seconds is not less than the size of data needed to watch <span class="tex-span"><i>t</i><sub class="lower-index">0</sub> - <i>t</i></span> seconds of the video.</p><p>Of course, the guys want to wait as little as possible, so your task is to find the minimum integer number of seconds to wait before turning the video on. The guys must watch the video without pauses.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 1000, <i>a</i> &gt; <i>b</i>)</span>. The first number (<span class="tex-span"><i>a</i></span>) denotes the size of data needed to watch one second of the video. The second number (<span class="tex-span"><i>b</i></span>) denotes the size of data Valeric and Valerko can download from the Net per second. The third number (<span class="tex-span"><i>c</i></span>) denotes the video's length in seconds.</p></div><div class="output-specification"><p>Print a single number — the minimum integer number of seconds that Valeric and Valerko must wait to watch football without pauses.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 1000, <i>a</i> &gt; <i>b</i>)</span>. The first number (<span class="tex-span"><i>a</i></span>) denotes the size of data needed to watch one second of the video. The second number (<span class="tex-span"><i>b</i></span>) denotes the size of data Valeric and Valerko can download from the Net per second. The third number (<span class="tex-span"><i>c</i></span>) denotes the video's length in seconds.</p>

## Output

<p>Print a single number — the minimum integer number of seconds that Valeric and Valerko must wait to watch football without pauses.</p>





```input1
4 1 1

```




```input2
10 3 2

```




```input3
13 12 1

```




```output1
3

```




```output2
5

```




```output3
1

```



## Note

<p>In the first sample video's length is 1 second and it is necessary 4 units of data for watching 1 second of video, so guys should download 4 <span class="tex-span">·</span> 1 = 4 units of data to watch the whole video. The most optimal way is to wait 3 seconds till 3 units of data will be downloaded and then start watching. While guys will be watching video 1 second, one unit of data will be downloaded and Valerik and Valerko will have 4 units of data by the end of watching. Also every moment till the end of video guys will have more data then necessary for watching.</p><p>In the second sample guys need 2 <span class="tex-span">·</span> 10 = 20 units of data, so they have to wait 5 seconds and after that they will have 20 units before the second second ends. However, if guys wait 4 seconds, they will be able to watch first second of video without pauses, but they will download 18 units of data by the end of second second and it is less then necessary.</p>
