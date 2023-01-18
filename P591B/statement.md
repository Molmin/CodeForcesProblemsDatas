## Description

<div><p>The name of one small but proud corporation consists of <span class="tex-span"><i>n</i></span> lowercase English letters. The Corporation has decided to try rebranding&nbsp;— an active marketing strategy, that includes a set of measures to change either the brand (both for the company and the goods it produces) or its components: the name, the logo, the slogan. They decided to start with the name.</p><p>For this purpose the corporation has consecutively hired <span class="tex-span"><i>m</i></span> designers. Once a company hires the <span class="tex-span"><i>i</i></span>-th designer, he immediately contributes to the creation of a new corporation name as follows: he takes the newest version of the name and replaces all the letters <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> by <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, and all the letters <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> by <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. This results in the new version. It is possible that some of these letters do no occur in the string. It may also happen that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> coincides with <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. The version of the name received after the work of the last designer becomes the new name of the corporation.</p><p>Manager Arkady has recently got a job in this company, but is already soaked in the spirit of teamwork and is very worried about the success of the rebranding. Naturally, he can't wait to find out what is the new name the Corporation will receive.</p><p>Satisfy Arkady's curiosity and tell him the final version of the name.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 200 000</span>)&nbsp;— the length of the initial name and the number of designers hired, respectively.</p><p>The second line consists of <span class="tex-span"><i>n</i></span> lowercase English letters and represents the original name of the corporation.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the designers' actions: the <span class="tex-span"><i>i</i></span>-th of them contains two space-separated lowercase English letters <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print the new name of the corporation.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 200 000</span>)&nbsp;— the length of the initial name and the number of designers hired, respectively.</p><p>The second line consists of <span class="tex-span"><i>n</i></span> lowercase English letters and represents the original name of the corporation.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the designers' actions: the <span class="tex-span"><i>i</i></span>-th of them contains two space-separated lowercase English letters <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print the new name of the corporation.</p>





```input1
6 1
police
p m

```




```input2
11 6
abacabadaba
a b
b c
a d
e g
f a
b b

```




```output1
molice

```




```output2
cdcbcdcfcdc

```



## Note

<p>In the second sample the name of the corporation consecutively changes as follows:</p><center> <img align="middle" class="tex-formula" src="file://X4UlbVPq.png" style="max-width: 100.0%;max-height: 100.0%;"><p><img align="middle" class="tex-formula" src="file://sP5oNGG0.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img align="middle" class="tex-formula" src="file://GeyOAQJG.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img align="middle" class="tex-formula" src="file://QYoxkPFP.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img align="middle" class="tex-formula" src="file://Gaa83gCd.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img align="middle" class="tex-formula" src="file://uThuL6JQ.png" style="max-width: 100.0%;max-height: 100.0%;"></p></center>
