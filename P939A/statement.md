## Description

<div><p>As you could know there are no male planes nor female planes. However, each plane on Earth likes some other plane. There are <span class="tex-span"><i>n</i></span> planes on Earth, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and the plane with number <span class="tex-span"><i>i</i></span> likes the plane with number <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span> and <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span>.</p><p>We call a love triangle a situation in which plane <span class="tex-span"><i>A</i></span> likes plane <span class="tex-span"><i>B</i></span>, plane <span class="tex-span"><i>B</i></span> likes plane <span class="tex-span"><i>C</i></span> and plane <span class="tex-span"><i>C</i></span> likes plane <span class="tex-span"><i>A</i></span>. Find out if there is any love triangle on Earth.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the number of planes.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span>), meaning that the <span class="tex-span"><i>i</i></span>-th plane likes the <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>-th.</p></div><div class="output-specification"><p>Output «<span class="tex-font-style-tt">YES</span>» if there is a love triangle consisting of planes on Earth. Otherwise, output «<span class="tex-font-style-tt">NO</span>».</p><p>You can output any letter in lower case or in upper case.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the number of planes.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span>), meaning that the <span class="tex-span"><i>i</i></span>-th plane likes the <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>-th.</p>

## Output

<p>Output «<span class="tex-font-style-tt">YES</span>» if there is a love triangle consisting of planes on Earth. Otherwise, output «<span class="tex-font-style-tt">NO</span>».</p><p>You can output any letter in lower case or in upper case.</p>





```input1
5
2 4 5 1 3

```




```input2
5
5 5 5 5 1

```




```output1
YES

```




```output2
NO

```



## Note

<p>In first example plane <span class="tex-span">2</span> likes plane <span class="tex-span">4</span>, plane <span class="tex-span">4</span> likes plane <span class="tex-span">1</span>, plane <span class="tex-span">1</span> likes plane <span class="tex-span">2</span> and that is a love triangle.</p><p>In second example there are no love triangles.</p>
