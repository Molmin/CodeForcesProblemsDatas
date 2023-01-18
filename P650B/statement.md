## Description

<div><p>Vasya's telephone contains <span class="tex-span"><i>n</i></span> photos. Photo number 1 is currently opened on the phone. It is allowed to move left and right to the adjacent photo by swiping finger over the screen. If you swipe left from the first photo, you reach photo <span class="tex-span"><i>n</i></span>. Similarly, by swiping right from the last photo you reach photo <span class="tex-span">1</span>. It takes <span class="tex-span"><i>a</i></span> seconds to swipe from photo to adjacent.</p><p>For each photo it is known which orientation is intended for it — horizontal or vertical. Phone is in the vertical orientation and <span class="tex-font-style-bf">can't</span> be rotated. It takes <span class="tex-span"><i>b</i></span> second to change orientation of the photo.</p><p>Vasya has <span class="tex-span"><i>T</i></span> seconds to watch photos. He want to watch as many photos as possible. If Vasya opens the photo for the first time, he spends <span class="tex-span">1</span> second to notice all details in it. If photo is in the wrong orientation, he spends <span class="tex-span"><i>b</i></span> seconds on rotating it before watching it. If Vasya has already opened the photo, he just skips it (so he doesn't spend any time for watching it or for changing its orientation). It is not allowed to skip unseen photos.</p><p>Help Vasya find the maximum number of photos he is able to watch during <span class="tex-span"><i>T</i></span> seconds.</p></div><div class="input-specification"><p>The first line of the input contains 4 integers <span class="tex-span"><i>n</i>, <i>a</i>, <i>b</i>, <i>T</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>T</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of photos, time to move from a photo to adjacent, time to change orientation of a photo and time Vasya can spend for watching photo.</p><p>Second line of the input contains a string of length <span class="tex-span"><i>n</i></span> containing symbols '<span class="tex-font-style-tt">w</span>' and '<span class="tex-font-style-tt">h</span>'. </p><p>If the <span class="tex-span"><i>i</i></span>-th position of a string contains '<span class="tex-font-style-tt">w</span>', then the photo <span class="tex-span"><i>i</i></span> should be seen in the <span class="tex-font-style-bf">horizontal</span> orientation.</p><p>If the <span class="tex-span"><i>i</i></span>-th position of a string contains '<span class="tex-font-style-tt">h</span>', then the photo <span class="tex-span"><i>i</i></span> should be seen in <span class="tex-font-style-bf">vertical</span> orientation.</p></div><div class="output-specification"><p>Output the only integer, the maximum number of photos Vasya is able to watch during those <span class="tex-span"><i>T</i></span> seconds.</p></div>

## Input

<p>The first line of the input contains 4 integers <span class="tex-span"><i>n</i>, <i>a</i>, <i>b</i>, <i>T</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>T</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of photos, time to move from a photo to adjacent, time to change orientation of a photo and time Vasya can spend for watching photo.</p><p>Second line of the input contains a string of length <span class="tex-span"><i>n</i></span> containing symbols '<span class="tex-font-style-tt">w</span>' and '<span class="tex-font-style-tt">h</span>'. </p><p>If the <span class="tex-span"><i>i</i></span>-th position of a string contains '<span class="tex-font-style-tt">w</span>', then the photo <span class="tex-span"><i>i</i></span> should be seen in the <span class="tex-font-style-bf">horizontal</span> orientation.</p><p>If the <span class="tex-span"><i>i</i></span>-th position of a string contains '<span class="tex-font-style-tt">h</span>', then the photo <span class="tex-span"><i>i</i></span> should be seen in <span class="tex-font-style-bf">vertical</span> orientation.</p>

## Output

<p>Output the only integer, the maximum number of photos Vasya is able to watch during those <span class="tex-span"><i>T</i></span> seconds.</p>





```input1
4 2 3 10
wwhw

```




```input2
5 2 4 13
hhwhh

```




```input3
5 2 4 1000
hhwhh

```




```input4
3 1 100 10
whw

```




```output1
2

```




```output2
4

```




```output3
5

```




```output4
0

```



## Note

<p>In the first sample test you can rotate the first photo (3 seconds), watch the first photo (1 seconds), move left (2 second), rotate fourth photo (3 seconds), watch fourth photo (1 second). The whole process takes exactly 10 seconds.</p><p>Note that in the last sample test the time is not enough even to watch the first photo, also you can't skip it.</p>
