## Description

<div><p>Berland starts to seize the initiative on the war with Flatland. To drive the enemy from their native land, the berlanders need to know exactly how many more flatland soldiers are left in the enemy's reserve. Fortunately, the scouts captured an enemy in the morning, who had a secret encrypted message with the information the berlanders needed so much.</p><p>The captured enemy had an array of positive integers. Berland intelligence have long been aware of the flatland code: to convey the message, which contained a number <span class="tex-span"><i>m</i></span>, the enemies use an array of integers <span class="tex-span"><i>a</i></span>. The number of its subarrays, in which there are at least <span class="tex-span"><i>k</i></span> equal numbers, equals <span class="tex-span"><i>m</i></span>. The number <span class="tex-span"><i>k</i></span> has long been known in the Berland army so General Touristov has once again asked Corporal Vasya to perform a simple task: to decipher the flatlanders' message.</p><p>Help Vasya, given an array of integers <span class="tex-span"><i>a</i></span> and number <span class="tex-span"><i>k</i></span>, find the number of subarrays of the array of numbers <span class="tex-span"><i>a</i></span>, which has at least <span class="tex-span"><i>k</i></span> equal numbers.</p><p><span class="tex-font-style-it">Subarray</span> <span class="tex-span"><i>a</i>[<i>i</i>... <i>j</i>]&nbsp;(1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i>)</span> of array <span class="tex-span"><i>a</i> = (<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>)</span> is an array, made from its consecutive elements, starting from the <span class="tex-span"><i>i</i></span>-th one and ending with the <span class="tex-span"><i>j</i></span>-th one: <span class="tex-span"><i>a</i>[<i>i</i>... <i>j</i>] = (<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>j</i></sub>)</span>.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 4·10<sup class="upper-index">5</sup>)</span>, showing how many numbers an array has and how many equal numbers the subarrays are required to have, correspondingly. </p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — elements of the array.</p></div><div class="output-specification"><p>Print the single number — the number of such subarrays of array <span class="tex-span"><i>a</i></span>, that they have at least <span class="tex-span"><i>k</i></span> equal integers.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. In is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 4·10<sup class="upper-index">5</sup>)</span>, showing how many numbers an array has and how many equal numbers the subarrays are required to have, correspondingly. </p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — elements of the array.</p>

## Output

<p>Print the single number — the number of such subarrays of array <span class="tex-span"><i>a</i></span>, that they have at least <span class="tex-span"><i>k</i></span> equal integers.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. In is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
4 2
1 2 1 2

```




```input2
5 3
1 2 1 1 3

```




```input3
3 1
1 1 1

```




```output1
3
```




```output2
2
```




```output3
6
```



## Note

<p>In the first sample are three subarrays, containing at least two equal numbers: (1,2,1), (2,1,2) and (1,2,1,2).</p><p>In the second sample are two subarrays, containing three equal numbers: (1,2,1,1,3) and (1,2,1,1).</p><p>In the third sample any subarray contains at least one 1 number. Overall they are 6: (1), (1), (1), (1,1), (1,1) and (1,1,1).</p>
