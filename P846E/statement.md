## Description

<div><p>Igor is a post-graduate student of chemistry faculty in Berland State University (BerSU). He needs to conduct a complicated experiment to write his thesis, but laboratory of BerSU doesn't contain all the materials required for this experiment.</p><p>Fortunately, chemical laws allow material transformations (yes, chemistry in Berland differs from ours). But the rules of transformation are a bit strange.</p><p>Berland chemists are aware of <span class="tex-span"><i>n</i></span> materials, numbered in the order they were discovered. Each material can be transformed into some other material (or vice versa). Formally, for each <span class="tex-span"><i>i</i></span> <span class="tex-span">(2 ≤ <i>i</i> ≤ <i>n</i>)</span> there exist two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> that denote a possible transformation: <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> kilograms of material <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> can be transformed into <span class="tex-span">1</span> kilogram of material <span class="tex-span"><i>i</i></span>, and <span class="tex-span">1</span> kilogram of material <span class="tex-span"><i>i</i></span> can be transformed into <span class="tex-span">1</span> kilogram of material <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Chemical processing equipment in BerSU allows only such transformation that the amount of resulting material is <span class="tex-font-style-bf">always an integer number of kilograms</span>.</p><p>For each <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) Igor knows that the experiment requires <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> kilograms of material <span class="tex-span"><i>i</i></span>, and the laboratory contains <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> kilograms of this material. Is it possible to conduct an experiment after transforming some materials (or none)?</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of materials discovered by Berland chemists.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>... <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>) — supplies of BerSU laboratory.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>) — the amounts required for the experiment.</p><p>Then <span class="tex-span"><i>n</i> - 1</span> lines follow. <span class="tex-span"><i>j</i></span>-th of them contains two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i> + 1</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>j</i> + 1</sub></span> that denote transformation of <span class="tex-span">(<i>j</i> + 1)</span>-th material (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>j</i> + 1</sub> ≤ <i>j</i>, 1 ≤ <i>k</i><sub class="lower-index"><i>j</i> + 1</sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">YES</span> if it is possible to conduct an experiment. Otherwise print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of materials discovered by Berland chemists.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>... <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>) — supplies of BerSU laboratory.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>) — the amounts required for the experiment.</p><p>Then <span class="tex-span"><i>n</i> - 1</span> lines follow. <span class="tex-span"><i>j</i></span>-th of them contains two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i> + 1</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>j</i> + 1</sub></span> that denote transformation of <span class="tex-span">(<i>j</i> + 1)</span>-th material (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>j</i> + 1</sub> ≤ <i>j</i>, 1 ≤ <i>k</i><sub class="lower-index"><i>j</i> + 1</sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print <span class="tex-font-style-tt">YES</span> if it is possible to conduct an experiment. Otherwise print <span class="tex-font-style-tt">NO</span>.</p>





```input1
3
1 2 3
3 2 1
1 1
1 1

```




```input2
3
3 2 1
1 2 3
1 1
1 2

```




```output1
YES

```




```output2
NO

```


