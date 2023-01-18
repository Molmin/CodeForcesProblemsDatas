## Description

<div><p>As Sherlock Holmes was investigating a crime, he identified <span class="tex-span"><i>n</i></span> suspects. He knows for sure that exactly one of them committed the crime. To find out which one did it, the detective lines up the suspects and numbered them from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. After that, he asked each one: "Which one committed the crime?". Suspect number <span class="tex-span"><i>i</i></span> answered either "The crime was committed by suspect number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>", or "Suspect number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> didn't commit the crime". Also, the suspect could say so about himself (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>i</i></span>).</p><p>Sherlock Holmes understood for sure that exactly <span class="tex-span"><i>m</i></span> answers were the truth and all other answers were a lie. Now help him understand this: which suspect lied and which one told the truth?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ <i>n</i></span>) — the total number of suspects and the number of suspects who told the truth. Next <span class="tex-span"><i>n</i></span> lines contain the suspects' answers. The <span class="tex-span"><i>i</i></span>-th line contains either "+<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes), if the suspect number <span class="tex-span"><i>i</i></span> says that the crime was committed by suspect number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, or "-<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes), if the suspect number <span class="tex-span"><i>i</i></span> says that the suspect number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> didn't commit the crime (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is an integer, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p><p>It is guaranteed that at least one suspect exists, such that if he committed the crime, then exactly <span class="tex-span"><i>m</i></span> people told the truth.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines. Line number <span class="tex-span"><i>i</i></span> should contain "<span class="tex-font-style-tt">Truth</span>" if suspect number <span class="tex-span"><i>i</i></span> has told the truth for sure. Print "<span class="tex-font-style-tt">Lie</span>" if the suspect number <span class="tex-span"><i>i</i></span> lied for sure and print "<span class="tex-font-style-tt">Not defined</span>" if he could lie and could tell the truth, too, depending on who committed the crime.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ <i>n</i></span>) — the total number of suspects and the number of suspects who told the truth. Next <span class="tex-span"><i>n</i></span> lines contain the suspects' answers. The <span class="tex-span"><i>i</i></span>-th line contains either "+<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes), if the suspect number <span class="tex-span"><i>i</i></span> says that the crime was committed by suspect number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, or "-<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes), if the suspect number <span class="tex-span"><i>i</i></span> says that the suspect number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> didn't commit the crime (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is an integer, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p><p>It is guaranteed that at least one suspect exists, such that if he committed the crime, then exactly <span class="tex-span"><i>m</i></span> people told the truth.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines. Line number <span class="tex-span"><i>i</i></span> should contain "<span class="tex-font-style-tt">Truth</span>" if suspect number <span class="tex-span"><i>i</i></span> has told the truth for sure. Print "<span class="tex-font-style-tt">Lie</span>" if the suspect number <span class="tex-span"><i>i</i></span> lied for sure and print "<span class="tex-font-style-tt">Not defined</span>" if he could lie and could tell the truth, too, depending on who committed the crime.</p>





```input1
1 1
+1

```




```input2
3 2
-1
-2
-3

```




```input3
4 1
+2
-3
+4
-1

```




```output1
Truth

```




```output2
Not defined
Not defined
Not defined

```




```output3
Lie
Not defined
Lie
Not defined

```



## Note

<p>The first sample has the single person and he confesses to the crime, and Sherlock Holmes knows that one person is telling the truth. That means that this person is telling the truth.</p><p>In the second sample there are three suspects and each one denies his guilt. Sherlock Holmes knows that only two of them are telling the truth. Any one of them can be the criminal, so we don't know for any of them, whether this person is telling the truth or not.</p><p>In the third sample the second and the fourth suspect defend the first and the third one. But only one is telling the truth, thus, the first or the third one is the criminal. Both of them can be criminals, so the second and the fourth one can either be lying or telling the truth. The first and the third one are lying for sure as they are blaming the second and the fourth one.</p>
