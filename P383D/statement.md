## Description

<div><p>Iahub accidentally discovered a secret lab. He found there <span class="tex-span"><i>n</i></span> devices ordered in a line, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. Each device <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> can create either <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> units of matter or <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> units of antimatter. </p><p>Iahub wants to choose some contiguous subarray of devices in the lab, specify the production mode for each of them (produce matter or antimatter) and finally take a photo of it. However he will be successful only if the amounts of matter and antimatter produced in the selected subarray will be the same (otherwise there would be overflowing matter or antimatter in the photo). </p><p>You are requested to compute the number of different ways Iahub can successful take a photo. A photo is different than another if it represents another subarray, or if at least one device of the subarray is set to produce matter in one of the photos and antimatter in the other one.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>.</p><p>The sum <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub></span> will be less than or equal to <span class="tex-span">10000</span>.</p></div><div class="output-specification"><p>Output a single integer, the number of ways Iahub can take a photo, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>.</p><p>The sum <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub></span> will be less than or equal to <span class="tex-span">10000</span>.</p>

## Output

<p>Output a single integer, the number of ways Iahub can take a photo, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
4
1 1 1 1

```




```output1
12

```



## Note

<p>The possible photos are [1+, 2-], [1-, 2+], [2+, 3-], [2-, 3+], [3+, 4-], [3-, 4+], [1+, 2+, 3-, 4-], [1+, 2-, 3+, 4-], [1+, 2-, 3-, 4+], [1-, 2+, 3+, 4-], [1-, 2+, 3-, 4+] and [1-, 2-, 3+, 4+], where "<span class="tex-span"><i>i</i></span>+" means that the <span class="tex-span"><i>i</i></span>-th element produces matter, and "<span class="tex-span"><i>i</i></span>-" means that the <span class="tex-span"><i>i</i></span>-th element produces antimatter.</p>
