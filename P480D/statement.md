## Description

<div><p>Jaroslav owns a small courier service. He has recently got and introduced a new system of processing parcels. Each parcel is a box, the box has its weight and strength. The system works as follows. It originally has an empty platform where you can put boxes by the following rules: </p><ul> <li> If the platform is empty, then the box is put directly on the platform, otherwise it is put on the topmost box on the platform. </li><li> The total weight of all boxes on the platform cannot exceed the strength of platform <span class="tex-span"><i>S</i></span> at any time. </li><li> The strength of any box of the platform at any time must be no less than the total weight of the boxes that stand above. </li></ul><p>You can take only the topmost box from the platform.</p><p>The system receives <span class="tex-span"><i>n</i></span> parcels, the <span class="tex-span"><i>i</i></span>-th parcel arrives exactly at time <span class="tex-span"><i>in</i><sub class="lower-index"><i>i</i></sub></span>, its weight and strength are equal to <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, respectively. Each parcel has a value of <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> bourles. However, to obtain this value, the system needs to give the parcel exactly at time <span class="tex-span"><i>out</i><sub class="lower-index"><i>i</i></sub></span>, otherwise Jaroslav will get 0 bourles for it. Thus, Jaroslav can skip any parcel and not put on the platform, formally deliver it at time <span class="tex-span"><i>in</i><sub class="lower-index"><i>i</i></sub></span> and not get anything for it. </p><p>Any operation in the problem is performed instantly. This means that it is possible to make several operations of receiving and delivering parcels at the same time and in any order. </p><p>Please note that the parcel that is delivered at time <span class="tex-span"><i>out</i><sub class="lower-index"><i>i</i></sub></span>, immediately gets outside of the system, and the following activities taking place at the same time are made ​​without taking it into consideration. </p><p>Since the system is very complex, and there are a lot of received parcels, Jaroslav asks you to say what maximum amount of money he can get using his system.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>S</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>S</i> ≤ 1000</span>). Then <span class="tex-span"><i>n</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th line contains five space-separated integers: <span class="tex-span"><i>in</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>out</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>in</i><sub class="lower-index"><i>i</i></sub> &lt; <i>out</i><sub class="lower-index"><i>i</i></sub> &lt; 2<i>n</i></span>, <span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). It is guaranteed that for any <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span"><i>i</i> ≠ <i>j</i></span>) either <span class="tex-span"><i>in</i><sub class="lower-index"><i>i</i></sub> ≠ <i>in</i><sub class="lower-index"><i>j</i></sub></span>, or <span class="tex-span"><i>out</i><sub class="lower-index"><i>i</i></sub> ≠ <i>out</i><sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="output-specification"><p>Print a single number — the maximum sum in bourles that Jaroslav can get.</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>S</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>S</i> ≤ 1000</span>). Then <span class="tex-span"><i>n</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th line contains five space-separated integers: <span class="tex-span"><i>in</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>out</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>in</i><sub class="lower-index"><i>i</i></sub> &lt; <i>out</i><sub class="lower-index"><i>i</i></sub> &lt; 2<i>n</i></span>, <span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). It is guaranteed that for any <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span"><i>i</i> ≠ <i>j</i></span>) either <span class="tex-span"><i>in</i><sub class="lower-index"><i>i</i></sub> ≠ <i>in</i><sub class="lower-index"><i>j</i></sub></span>, or <span class="tex-span"><i>out</i><sub class="lower-index"><i>i</i></sub> ≠ <i>out</i><sub class="lower-index"><i>j</i></sub></span>.</p>

## Output

<p>Print a single number — the maximum sum in bourles that Jaroslav can get.</p>





```input1
3 2
0 1 1 1 1
1 2 1 1 1
0 2 1 1 1

```




```input2
5 5
0 6 1 2 1
1 2 1 1 1
1 3 1 1 1
3 6 2 1 2
4 5 1 1 1

```




```output1
3

```




```output2
5

```



## Note

<p><span class="tex-font-style-bf">Note to the second sample</span> (<span class="tex-span"><i>T</i></span> is the moment in time): </p><ul> <li> <span class="tex-span"><i>T</i> = 0</span>: The first parcel arrives, we put in on the first platform. </li><li> <span class="tex-span"><i>T</i> = 1</span>: The second and third parcels arrive, we put the third one on the current top (i.e. first) parcel on the platform, then we put the secod one on the third one. Now the first parcel holds weight <span class="tex-span"><i>w</i><sub class="lower-index">2</sub> + <i>w</i><sub class="lower-index">3</sub> = 2</span> and the third parcel holds <span class="tex-span"><i>w</i><sub class="lower-index">2</sub> = 1</span>. </li><li> <span class="tex-span"><i>T</i> = 2</span>: We deliver the second parcel and get <span class="tex-span"><i>v</i><sub class="lower-index">2</sub> = 1</span> bourle. Now the first parcel holds weight <span class="tex-span"><i>w</i><sub class="lower-index">3</sub> = 1</span>, the third one holds 0. </li><li> <span class="tex-span"><i>T</i> = 3</span>: The fourth parcel comes. First we give the third parcel and get <span class="tex-span"><i>v</i><sub class="lower-index">3</sub> = 1</span> bourle. Now the first parcel holds weight 0. We put the fourth parcel on it — the first one holds <span class="tex-span"><i>w</i><sub class="lower-index">4</sub> = 2</span>. </li><li> <span class="tex-span"><i>T</i> = 4</span>: The fifth parcel comes. We cannot put it on the top parcel of the platform as in that case the first parcel will carry weight <span class="tex-span"><i>w</i><sub class="lower-index">4</sub> + <i>w</i><sub class="lower-index">5</sub> = 3</span>, that exceed its strength <span class="tex-span"><i>s</i><sub class="lower-index">1</sub> = 2</span>, that's unacceptable. We skip the fifth parcel and get nothing for it. </li><li> <span class="tex-span"><i>T</i> = 5</span>: Nothing happens. </li><li> <span class="tex-span"><i>T</i> = 6</span>: We deliver the fourth, then the first parcel and get <span class="tex-span"><i>v</i><sub class="lower-index">1</sub> + <i>v</i><sub class="lower-index">4</sub> = 3</span> bourles for them. </li></ul><p>Note that you could have skipped the fourth parcel and got the fifth one instead, but in this case the final sum would be 4 bourles.</p>
