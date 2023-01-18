## Description

<div><p>Vasya has got many devices that work on electricity. He's got <span class="tex-span"><i>n</i></span> supply-line filters to plug the devices, the <span class="tex-span"><i>i</i></span>-th supply-line filter has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> sockets.</p><p>Overall Vasya has got <span class="tex-span"><i>m</i></span> devices and <span class="tex-span"><i>k</i></span> electrical sockets in his flat, he can plug the devices or supply-line filters directly. Of course, he can plug the supply-line filter to any other supply-line filter. The device (or the supply-line filter) is considered plugged to electricity if it is either plugged to one of <span class="tex-span"><i>k</i></span> electrical sockets, or if it is plugged to some supply-line filter that is in turn plugged to electricity. </p><p>What minimum number of supply-line filters from the given set will Vasya need to plug all the devices he has to electricity? Note that all devices and supply-line filters take one socket for plugging and that he can use one socket to plug either one device or one supply-line filter.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 50</span>) — the number of supply-line filters, the number of devices and the number of sockets that he can plug to directly, correspondingly. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 50</span>) — number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> stands for the number of sockets on the <span class="tex-span"><i>i</i></span>-th supply-line filter.</p></div><div class="output-specification"><p>Print a single number — the minimum number of supply-line filters that is needed to plug all the devices to electricity. If it is impossible to plug all the devices even using all the supply-line filters, print -1.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 50</span>) — the number of supply-line filters, the number of devices and the number of sockets that he can plug to directly, correspondingly. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 50</span>) — number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> stands for the number of sockets on the <span class="tex-span"><i>i</i></span>-th supply-line filter.</p>

## Output

<p>Print a single number — the minimum number of supply-line filters that is needed to plug all the devices to electricity. If it is impossible to plug all the devices even using all the supply-line filters, print -1.</p>





```input1
3 5 3
3 1 2

```




```input2
4 7 2
3 3 2 4

```




```input3
5 5 1
1 3 1 2 1

```




```output1
1

```




```output2
2

```




```output3
-1

```



## Note

<p>In the first test case he can plug the first supply-line filter directly to electricity. After he plug it, he get 5 (3 on the supply-line filter and 2 remaining sockets for direct plugging) available sockets to plug. Thus, one filter is enough to plug 5 devices.</p><p>One of the optimal ways in the second test sample is to plug the second supply-line filter directly and plug the fourth supply-line filter to one of the sockets in the second supply-line filter. Thus, he gets exactly 7 sockets, available to plug: one to plug to the electricity directly, 2 on the second supply-line filter, 4 on the fourth supply-line filter. There's no way he can plug 7 devices if he use one supply-line filter.</p>
