## Description

<div><p>You've got a list of program warning logs. Each record of a log stream is a string in this format: </p><center> "<span class="tex-font-style-tt">2012-MM-DD HH:MM:SS:MESSAGE</span>" (without the quotes). </center><p>String "<span class="tex-font-style-tt">MESSAGE</span>" consists of spaces, uppercase and lowercase English letters and characters "<span class="tex-font-style-tt">!</span>", "<span class="tex-font-style-tt">.</span>", "<span class="tex-font-style-tt">,</span>", "<span class="tex-font-style-tt">?</span>". String "<span class="tex-font-style-tt">2012-MM-DD</span>" determines a correct date in the year of 2012. String "<span class="tex-font-style-tt">HH:MM:SS</span>" determines a correct time in the 24 hour format.</p><p>The described record of a log stream means that at a certain time the record has got some program warning (string "<span class="tex-font-style-tt">MESSAGE</span>" contains the warning's description).</p><p>Your task is to print the first moment of time, when the number of warnings for the last <span class="tex-span"><i>n</i></span> seconds was not less than <span class="tex-span"><i>m</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10000)</span>.</p><p>The second and the remaining lines of the input represent the log stream. The second line of the input contains the first record of the log stream, the third line contains the second record and so on. Each record of the log stream has the above described format. All records are given in the chronological order, that is, the warning records are given in the order, in which the warnings appeared in the program. </p><p>It is guaranteed that the log has at least one record. It is guaranteed that the total length of all lines of the log stream doesn't exceed <span class="tex-span">5·10<sup class="upper-index">6</sup></span> (in particular, this means that the length of some line does not exceed <span class="tex-span">5·10<sup class="upper-index">6</sup></span> characters). It is guaranteed that all given dates and times are correct, and the string '<span class="tex-font-style-tt">MESSAGE</span>" in all records is non-empty.</p></div><div class="output-specification"><p>If there is no sought moment of time, print -1. Otherwise print a string in the format "<span class="tex-font-style-tt">2012-MM-DD HH:MM:SS</span>" (without the quotes) — the first moment of time when the number of warnings for the last <span class="tex-span"><i>n</i></span> seconds got no less than <span class="tex-span"><i>m</i></span>.</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10000)</span>.</p><p>The second and the remaining lines of the input represent the log stream. The second line of the input contains the first record of the log stream, the third line contains the second record and so on. Each record of the log stream has the above described format. All records are given in the chronological order, that is, the warning records are given in the order, in which the warnings appeared in the program. </p><p>It is guaranteed that the log has at least one record. It is guaranteed that the total length of all lines of the log stream doesn't exceed <span class="tex-span">5·10<sup class="upper-index">6</sup></span> (in particular, this means that the length of some line does not exceed <span class="tex-span">5·10<sup class="upper-index">6</sup></span> characters). It is guaranteed that all given dates and times are correct, and the string '<span class="tex-font-style-tt">MESSAGE</span>" in all records is non-empty.</p>

## Output

<p>If there is no sought moment of time, print -1. Otherwise print a string in the format "<span class="tex-font-style-tt">2012-MM-DD HH:MM:SS</span>" (without the quotes) — the first moment of time when the number of warnings for the last <span class="tex-span"><i>n</i></span> seconds got no less than <span class="tex-span"><i>m</i></span>.</p>





```input1
60 3
2012-03-16 16:15:25: Disk size is
2012-03-16 16:15:25: Network failute
2012-03-16 16:16:29: Cant write varlog
2012-03-16 16:16:42: Unable to start process
2012-03-16 16:16:43: Disk size is too small
2012-03-16 16:16:53: Timeout detected

```




```input2
1 2
2012-03-16 23:59:59:Disk size
2012-03-17 00:00:00: Network
2012-03-17 00:00:01:Cant write varlog

```




```input3
2 2
2012-03-16 23:59:59:Disk size is too sm
2012-03-17 00:00:00:Network failute dete
2012-03-17 00:00:01:Cant write varlogmysq

```




```output1
2012-03-16 16:16:43

```




```output2
-1

```




```output3
2012-03-17 00:00:00

```


