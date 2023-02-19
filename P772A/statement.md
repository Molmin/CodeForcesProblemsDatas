## Description

<div><p>You have <span class="tex-span"><i>n</i></span> devices that you want to use simultaneously.</p><p>The <span class="tex-span"><i>i</i></span>-th device uses <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> units of power per second. This usage is continuous. That is, in <span class="tex-span">λ</span> seconds, the device will use <span class="tex-span">λ·<i>a</i><sub class="lower-index"><i>i</i></sub></span> units of power. The <span class="tex-span"><i>i</i></span>-th device currently has <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> units of power stored. All devices can store an arbitrary amount of power.</p><p>You have a single charger that can plug to any single device. The charger will add <span class="tex-span"><i>p</i></span> units of power per second to a device. This charging is continuous. That is, if you plug in a device for <span class="tex-span">λ</span> seconds, it will gain <span class="tex-span">λ·<i>p</i></span> units of power. You can switch which device is charging at any arbitrary unit of time (including real numbers), and the time it takes to switch is negligible.</p><p>You are wondering, what is the maximum amount of time you can use the devices until one of them hits <span class="tex-span">0</span> units of power.</p><p>If you can use the devices indefinitely, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the maximum amount of time before any one device hits <span class="tex-span">0</span> power.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of devices and the power of the charger.</p><p>This is followed by <span class="tex-span"><i>n</i></span> lines which contain two integers each. Line <span class="tex-span"><i>i</i></span> contains the integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— the power of the device and the amount of power stored in the device in the beginning.</p></div><div class="output-specification"><p>If you can use the devices indefinitely, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the maximum amount of time before any one device hits <span class="tex-span">0</span> power.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Namely, let's assume that your answer is <span class="tex-span"><i>a</i></span> and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://qyQBhbEi.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of devices and the power of the charger.</p><p>This is followed by <span class="tex-span"><i>n</i></span> lines which contain two integers each. Line <span class="tex-span"><i>i</i></span> contains the integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— the power of the device and the amount of power stored in the device in the beginning.</p>

## Output

<p>If you can use the devices indefinitely, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the maximum amount of time before any one device hits <span class="tex-span">0</span> power.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Namely, let's assume that your answer is <span class="tex-span"><i>a</i></span> and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://qyQBhbEi.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2 1
2 2
2 1000

```




```input2
1 100
1 1

```




```input3
3 5
4 3
5 2
6 1

```




```output1
2.0000000000
```




```output2
-1

```




```output3
0.5000000000
```



## Note

<p>In sample test 1, you can charge the first device for the entire time until it hits zero power. The second device has enough power to last this time without being charged.</p><p>In sample test 2, you can use the device indefinitely.</p><p>In sample test 3, we can charge the third device for <span class="tex-span">2 / 5</span> of a second, then switch to charge the second device for a <span class="tex-span">1 / 10</span> of a second.</p>
