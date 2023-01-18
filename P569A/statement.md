## Description

<div><p>Little Lesha loves listening to music via his smartphone. But the smartphone doesn't have much memory, so Lesha listens to his favorite songs in a well-known social network InTalk.</p><p>Unfortunately, internet is not that fast in the city of Ekaterinozavodsk and the song takes a lot of time to download. But Lesha is quite impatient. The song's duration is <span class="tex-span"><i>T</i></span> seconds. Lesha downloads the first <span class="tex-span"><i>S</i></span> seconds of the song and plays it. When the playback reaches the point that has not yet been downloaded, Lesha immediately plays the song from the start (the loaded part of the song stays in his phone, and the download is continued from the same place), and it happens until the song is downloaded completely and Lesha listens to it to the end. For <span class="tex-span"><i>q</i></span> seconds of real time the Internet allows you to download <span class="tex-span"><i>q</i> - 1</span> seconds of the track.</p><p>Tell Lesha, for how many times he will start the song, including the very first start.</p></div><div class="input-specification"><p>The single line contains three integers <span class="tex-span"><i>T</i>, <i>S</i>, <i>q</i></span> (<span class="tex-span">2 ≤ <i>q</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>S</i> &lt; <i>T</i> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of times the song will be restarted.</p></div>

## Input

<p>The single line contains three integers <span class="tex-span"><i>T</i>, <i>S</i>, <i>q</i></span> (<span class="tex-span">2 ≤ <i>q</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>S</i> &lt; <i>T</i> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print a single integer&nbsp;— the number of times the song will be restarted.</p>





```input1
5 2 2

```




```input2
5 4 7

```




```input3
6 2 3

```




```output1
2

```




```output2
1

```




```output3
1

```



## Note

<p>In the first test, the song is played twice faster than it is downloaded, which means that during four first seconds Lesha reaches the moment that has not been downloaded, and starts the song again. After another two seconds, the song is downloaded completely, and thus, Lesha starts the song twice.</p><p>In the second test, the song is almost downloaded, and Lesha will start it only once.</p><p>In the third sample test the download finishes and Lesha finishes listening at the same moment. Note that song isn't restarted in this case.</p>
