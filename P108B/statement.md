## Description

<div><p>Tattah's youngest brother, Tuftuf, is new to programming.</p><p>Since his older brother is such a good programmer, his biggest dream is to outshine him. Tuftuf is a student at the German University in Cairo (GUC) where he learns to write programs in Gava.</p><p>Today, Tuftuf was introduced to Gava's unsigned integer datatypes. Gava has <span class="tex-span"><i>n</i></span> unsigned integer datatypes of sizes (in bits) <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span>. The <span class="tex-span"><i>i</i></span>-th datatype have size <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> bits, so it can represent every integer between <span class="tex-span">0</span> and <span class="tex-span">2<sup class="upper-index"><i>a</i><sub class="lower-index"><i>i</i></sub></sup> - 1</span> inclusive. </p><p>Tuftuf is thinking of learning a better programming language. If there exists an integer <span class="tex-span"><i>x</i></span>, such that <span class="tex-span"><i>x</i></span> fits in some type <span class="tex-span"><i>i</i></span> (in <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> bits) and <span class="tex-span"><i>x</i>·<i>x</i></span> does not fit in some other type <span class="tex-span"><i>j</i></span> (in <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> bits) where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>j</i></sub></span>, then Tuftuf will stop using Gava.</p><p>Your task is to determine Tuftuf's destiny.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of Gava's unsigned integer datatypes' sizes. The second line contains a single-space-separated list of <span class="tex-span"><i>n</i></span> integers (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — sizes of datatypes in bits. Some datatypes may have equal sizes.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if Tuftuf will stop using Gava, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of Gava's unsigned integer datatypes' sizes. The second line contains a single-space-separated list of <span class="tex-span"><i>n</i></span> integers (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — sizes of datatypes in bits. Some datatypes may have equal sizes.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if Tuftuf will stop using Gava, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
3
64 16 32

```




```input2
4
4 2 1 3

```




```output1
NO

```




```output2
YES

```



## Note

<p>In the second example, <span class="tex-span"><i>x</i> = 7</span> <span class="tex-span">(111<sub class="lower-index">2</sub>)</span> fits in <span class="tex-span">3</span> bits, but <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> = 49</span> <span class="tex-span">(110001<sub class="lower-index">2</sub>)</span> does not fit in <span class="tex-span">4</span> bits.</p>
