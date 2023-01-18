## Description

<div><p>Petya sometimes has to water his field. To water the field, Petya needs a tank with exactly <span class="tex-span"><i>V</i></span> ml of water.</p><p>Petya has got <span class="tex-span"><i>N</i></span> tanks, <span class="tex-span"><i>i</i></span>-th of them initially containing <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> ml of water. The tanks are really large, any of them can contain any amount of water (no matter how large this amount is).</p><p>Also Petya has got a scoop that can contain up to <span class="tex-span"><i>K</i></span> ml of water (initially the scoop is empty). This scoop can be used to get some water from some tank, and after that pour it all into some tank (it is impossible to get water from multiple tanks without pouring it, or leave some water in the scoop when pouring it). When Petya tries to get some water from a tank, he gets <span class="tex-span"><i>min</i>(<i>v</i>, <i>K</i>)</span> water, where <span class="tex-span"><i>v</i></span> is the current volume of water in the tank.</p><p>Is it possible to obtain a tank with exactly <span class="tex-span"><i>V</i></span> ml of water using these operations? If it is possible, print a sequence of operations that allows to do it. If there are multiple ways to obtain needed amount of water in some tank, print any of them.</p></div><div class="input-specification"><p>The first line contains <span class="tex-span">3</span> integers: <span class="tex-span"><i>N</i></span> <span class="tex-span">(2 ≤ <i>N</i> ≤ 5000)</span>, <span class="tex-span"><i>K</i></span> <span class="tex-span">(1 ≤ <i>K</i> ≤ 5000)</span>, and <span class="tex-span"><i>V</i></span> <span class="tex-span">(0 ≤ <i>V</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the number of tanks, the maximum volume of water the scoop can contain, and the required amount of water in some tank, respectively.</p><p>The second line contains <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is initial volume of water in <span class="tex-span"><i>i</i></span>-th tank.</p></div><div class="output-specification"><p>If it is impossible to obtain a tank with exactly <span class="tex-span"><i>V</i></span> ml of water, print <span class="tex-font-style-tt">NO</span>. </p><p>Otherwise print <span class="tex-font-style-tt">YES</span> in the first line, and beginning from the second line, print the sequence of operations in the following format: </p><p>Each line has to contain <span class="tex-span">3</span> numbers denoting a compressed operation: "<span class="tex-span"><i>cnt</i></span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>" <span class="tex-span">(1 ≤ <i>cnt</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>x</i>, <i>y</i> ≤ <i>N</i>)</span>, where <span class="tex-span"><i>x</i></span> is the index of the tank where we get water, <span class="tex-span"><i>y</i></span> is the index of the tank where we pour water, and <span class="tex-span"><i>cnt</i></span> is the number of times we transfer water from tank <span class="tex-span"><i>x</i></span> to tank <span class="tex-span"><i>y</i></span>. </p><p>The number of these lines <span class="tex-font-style-bf">must not exceed <span class="tex-span"><i>N</i> + 5</span></span>.</p></div>

## Input

<p>The first line contains <span class="tex-span">3</span> integers: <span class="tex-span"><i>N</i></span> <span class="tex-span">(2 ≤ <i>N</i> ≤ 5000)</span>, <span class="tex-span"><i>K</i></span> <span class="tex-span">(1 ≤ <i>K</i> ≤ 5000)</span>, and <span class="tex-span"><i>V</i></span> <span class="tex-span">(0 ≤ <i>V</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the number of tanks, the maximum volume of water the scoop can contain, and the required amount of water in some tank, respectively.</p><p>The second line contains <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is initial volume of water in <span class="tex-span"><i>i</i></span>-th tank.</p>

## Output

<p>If it is impossible to obtain a tank with exactly <span class="tex-span"><i>V</i></span> ml of water, print <span class="tex-font-style-tt">NO</span>. </p><p>Otherwise print <span class="tex-font-style-tt">YES</span> in the first line, and beginning from the second line, print the sequence of operations in the following format: </p><p>Each line has to contain <span class="tex-span">3</span> numbers denoting a compressed operation: "<span class="tex-span"><i>cnt</i></span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>" <span class="tex-span">(1 ≤ <i>cnt</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>x</i>, <i>y</i> ≤ <i>N</i>)</span>, where <span class="tex-span"><i>x</i></span> is the index of the tank where we get water, <span class="tex-span"><i>y</i></span> is the index of the tank where we pour water, and <span class="tex-span"><i>cnt</i></span> is the number of times we transfer water from tank <span class="tex-span"><i>x</i></span> to tank <span class="tex-span"><i>y</i></span>. </p><p>The number of these lines <span class="tex-font-style-bf">must not exceed <span class="tex-span"><i>N</i> + 5</span></span>.</p>





```input1
2 3 5
2 3

```




```input2
2 3 4
2 3

```




```input3
5 2 0
1 3 5 7 9

```




```output1
YES
1 2 1

```




```output2
NO

```




```output3
YES
2 2 1
3 3 1
4 4 1
5 5 1

```


