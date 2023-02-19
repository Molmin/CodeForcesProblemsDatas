## Description

<div><p>Finally! Vasya have come of age and that means he can finally get a passport! To do it, he needs to visit the passport office, but it's not that simple. There's only one receptionist at the passport office and people can queue up long before it actually opens. Vasya wants to visit the passport office tomorrow.</p><p>He knows that the receptionist starts working after <span class="tex-span"><i>t</i><sub class="lower-index"><i>s</i></sub></span> minutes have passed after midnight and closes after <span class="tex-span"><i>t</i><sub class="lower-index"><i>f</i></sub></span> minutes have passed after midnight (so that <span class="tex-span">(<i>t</i><sub class="lower-index"><i>f</i></sub> - 1)</span> is the last minute when the receptionist is still working). The receptionist spends exactly <span class="tex-span"><i>t</i></span> minutes on each person in the queue. If the receptionist would stop working within <span class="tex-span"><i>t</i></span> minutes, he stops serving visitors (other than the one he already serves). </p><p>Vasya also knows that exactly <span class="tex-span"><i>n</i></span> visitors would come tomorrow. For each visitor Vasya knows the point of time when he would come to the passport office. Each visitor queues up and doesn't leave until he was served. If the receptionist is free when a visitor comes (in particular, if the previous visitor was just served and the queue is empty), the receptionist begins to serve the newcomer immediately.</p><center> <img class="tex-graphics" height="302px" src="file://zBvkDGmY.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px">   <span class="tex-font-size-small">"Reception 1"</span> </center><p>For each visitor, the point of time when he would come to the passport office is positive. Vasya can come to the office at the time zero (that is, at midnight) if he needs so, but he can come to the office only at integer points of time. If Vasya arrives at the passport office at the same time with several other visitors, he yields to them and stand in the queue after the last of them.</p><p>Vasya wants to come at such point of time that he will be served by the receptionist, and he would spend the minimum possible time in the queue. Help him!</p></div><div class="input-specification"><p>The first line contains three integers: the point of time when the receptionist begins to work <span class="tex-span"><i>t</i><sub class="lower-index"><i>s</i></sub></span>, the point of time when the receptionist stops working <span class="tex-span"><i>t</i><sub class="lower-index"><i>f</i></sub></span> and the time the receptionist spends on each visitor <span class="tex-span"><i>t</i></span>. The second line contains one integer <span class="tex-span"><i>n</i></span>&nbsp;— the amount of visitors (<span class="tex-span">0 ≤ <i>n</i> ≤ 100 000</span>). The third line contains positive integers in non-decreasing order&nbsp;— the points of time when the visitors arrive to the passport office.</p><p>All times are set in minutes and do not exceed <span class="tex-span">10<sup class="upper-index">12</sup></span>; it is guaranteed that <span class="tex-span"><i>t</i><sub class="lower-index"><i>s</i></sub> &lt; <i>t</i><sub class="lower-index"><i>f</i></sub></span>. It is also guaranteed that Vasya can arrive at the passport office at such a point of time that he would be served by the receptionist.</p></div><div class="output-specification"><p>Print single non-negative integer&nbsp;— the point of time when Vasya should arrive at the passport office. If Vasya arrives at the passport office at the same time with several other visitors, he yields to them and queues up the last. If there are many answers, you can print any of them.</p></div>

## Input

<p>The first line contains three integers: the point of time when the receptionist begins to work <span class="tex-span"><i>t</i><sub class="lower-index"><i>s</i></sub></span>, the point of time when the receptionist stops working <span class="tex-span"><i>t</i><sub class="lower-index"><i>f</i></sub></span> and the time the receptionist spends on each visitor <span class="tex-span"><i>t</i></span>. The second line contains one integer <span class="tex-span"><i>n</i></span>&nbsp;— the amount of visitors (<span class="tex-span">0 ≤ <i>n</i> ≤ 100 000</span>). The third line contains positive integers in non-decreasing order&nbsp;— the points of time when the visitors arrive to the passport office.</p><p>All times are set in minutes and do not exceed <span class="tex-span">10<sup class="upper-index">12</sup></span>; it is guaranteed that <span class="tex-span"><i>t</i><sub class="lower-index"><i>s</i></sub> &lt; <i>t</i><sub class="lower-index"><i>f</i></sub></span>. It is also guaranteed that Vasya can arrive at the passport office at such a point of time that he would be served by the receptionist.</p>

## Output

<p>Print single non-negative integer&nbsp;— the point of time when Vasya should arrive at the passport office. If Vasya arrives at the passport office at the same time with several other visitors, he yields to them and queues up the last. If there are many answers, you can print any of them.</p>





```input1
10 15 2
2
10 13

```




```input2
8 17 3
4
3 4 5 8

```




```output1
12
```




```output2
2
```



## Note

<p>In the first example the first visitor comes exactly at the point of time when the receptionist begins to work, and he is served for two minutes. At 12 minutes after the midnight the receptionist stops serving the first visitor, and if Vasya arrives at this moment, he will be served immediately, because the next visitor would only come at 13 minutes after midnight.</p><p>In the second example, Vasya has to come before anyone else to be served. </p>
