## Description

<div><p>The main server of Gomble company received a log of one top-secret process, the name of which can't be revealed. The log was written in the following format: «<span class="tex-font-style-tt">[date:time]: message</span>», where for each «<span class="tex-font-style-tt">[date:time]</span>» value existed not more than 10 lines. All the files were encoded in a very complicated manner, and only one programmer — Alex — managed to decode them. The code was so complicated that Alex needed four weeks to decode it. Right after the decoding process was finished, all the files were deleted. But after the files deletion, Alex noticed that he saved the recordings in format «<span class="tex-font-style-tt">[time]: message</span>». So, information about the dates was lost. However, as the lines were added into the log in chronological order, it's not difficult to say if the recordings could appear during one day or not. It is possible also to find the minimum amount of days during which the log was written.</p><p>So, to make up for his mistake Alex has to find the minimum amount of days covered by the log. Note that Alex doesn't have to find the minimum amount of days between the beginning and the end of the logging, he has to find the minimum amount of dates in which records could be done. (See Sample test 2 for further clarifications).</p><p>We should remind you that the process made not more than 10 recordings in a minute. Consider that a midnight belongs to coming day.</p></div><div class="input-specification"><p>The first input line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). The following <span class="tex-span"><i>n</i></span> lines contain recordings in format «<span class="tex-font-style-tt">[time]: message</span>», where time is given in format «<span class="tex-font-style-tt">hh:mm x.m.</span>». For <span class="tex-font-style-tt">hh</span> two-digit numbers from <span class="tex-font-style-tt">01</span> to <span class="tex-font-style-tt">12</span> are used, for <span class="tex-font-style-tt">mm</span> two-digit numbers from <span class="tex-font-style-tt">00</span> to <span class="tex-font-style-tt">59</span> are used, and <span class="tex-font-style-tt">x</span> is either character «<span class="tex-font-style-tt">a</span>» or character «<span class="tex-font-style-tt">p</span>». A message is a non-empty sequence of Latin letters and/or spaces, it doesn't start or end with a space. The length of each message doesn't exceed 20.</p></div><div class="output-specification"><p>Output one number — the minimum amount of days covered by the log.</p></div>

## Input

<p>The first input line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). The following <span class="tex-span"><i>n</i></span> lines contain recordings in format «<span class="tex-font-style-tt">[time]: message</span>», where time is given in format «<span class="tex-font-style-tt">hh:mm x.m.</span>». For <span class="tex-font-style-tt">hh</span> two-digit numbers from <span class="tex-font-style-tt">01</span> to <span class="tex-font-style-tt">12</span> are used, for <span class="tex-font-style-tt">mm</span> two-digit numbers from <span class="tex-font-style-tt">00</span> to <span class="tex-font-style-tt">59</span> are used, and <span class="tex-font-style-tt">x</span> is either character «<span class="tex-font-style-tt">a</span>» or character «<span class="tex-font-style-tt">p</span>». A message is a non-empty sequence of Latin letters and/or spaces, it doesn't start or end with a space. The length of each message doesn't exceed 20.</p>

## Output

<p>Output one number — the minimum amount of days covered by the log.</p>





```input1
5
[05:00 a.m.]: Server is started
[05:00 a.m.]: Rescan initialized
[01:13 p.m.]: Request processed
[01:10 p.m.]: Request processed
[11:40 p.m.]: Rescan completed

```




```input2
3
[09:00 a.m.]: User logged in
[08:00 a.m.]: User logged in
[07:00 a.m.]: User logged in

```




```output1
2

```




```output2
3

```



## Note

<p>Formally the 12-hour time format is described at: </p><ul> <li> <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/12-hour_clock</span>. </li></ul> The problem authors recommend you to look through these descriptions before you start with the problem.
