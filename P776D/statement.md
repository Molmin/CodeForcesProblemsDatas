## Description

<div><p>Moriarty has trapped <span class="tex-span"><i>n</i></span> people in <span class="tex-span"><i>n</i></span> distinct rooms in a hotel. Some rooms are locked, others are unlocked. But, there is a condition that the people in the hotel can only escape when all the doors are unlocked at the same time. There are <span class="tex-span"><i>m</i></span> switches. Each switch control doors of some rooms, but each door is controlled by <span class="tex-font-style-bf">exactly two</span> switches.</p><p>You are given the initial configuration of the doors. Toggling any switch, that is, turning it ON when it is OFF, or turning it OFF when it is ON, toggles the condition of the doors that this switch controls. Say, we toggled switch <span class="tex-span">1</span>, which was connected to room <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span> which were respectively locked, unlocked and unlocked. Then, after toggling the switch, they become unlocked, locked and locked.</p><p>You need to tell Sherlock, if there exists a way to unlock all doors at the same time.</p></div><div class="input-specification"><p>First line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of rooms and the number of switches.</p><p>Next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>) which tell the status of room doors. The <span class="tex-span"><i>i</i></span>-th room is locked if <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 0</span>, otherwise it is unlocked.</p><p>The <span class="tex-span"><i>i</i></span>-th of next <span class="tex-span"><i>m</i></span> lines contains an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) followed by <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> distinct integers separated by space, denoting the number of rooms controlled by the <span class="tex-span"><i>i</i></span>-th switch followed by the room numbers that this switch controls. It is guaranteed that the room numbers are in the range from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. It is guaranteed that each door is controlled by exactly two switches.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">YES</span>" without quotes, if it is possible to open all doors at the same time, otherwise output "<span class="tex-font-style-tt">NO</span>" without quotes.</p></div>

## Input

<p>First line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of rooms and the number of switches.</p><p>Next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>) which tell the status of room doors. The <span class="tex-span"><i>i</i></span>-th room is locked if <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 0</span>, otherwise it is unlocked.</p><p>The <span class="tex-span"><i>i</i></span>-th of next <span class="tex-span"><i>m</i></span> lines contains an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) followed by <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> distinct integers separated by space, denoting the number of rooms controlled by the <span class="tex-span"><i>i</i></span>-th switch followed by the room numbers that this switch controls. It is guaranteed that the room numbers are in the range from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. It is guaranteed that each door is controlled by exactly two switches.</p>

## Output

<p>Output "<span class="tex-font-style-tt">YES</span>" without quotes, if it is possible to open all doors at the same time, otherwise output "<span class="tex-font-style-tt">NO</span>" without quotes.</p>





```input1
3 3
1 0 1
2 1 3
2 1 2
2 2 3

```




```input2
3 3
1 0 1
3 1 2 3
1 2
2 1 3

```




```input3
3 3
1 0 1
3 1 2 3
2 1 2
1 3

```




```output1
NO
```




```output2
YES
```




```output3
NO
```



## Note

<p>In the second example input, the initial statuses of the doors are <span class="tex-span">[1, 0, 1]</span> (<span class="tex-span">0</span> means locked, <span class="tex-span">1</span>&nbsp;— unlocked).</p><p>After toggling switch <span class="tex-span">3</span>, we get <span class="tex-span">[0, 0, 0]</span> that means all doors are locked.</p><p>Then, after toggling switch <span class="tex-span">1</span>, we get <span class="tex-span">[1, 1, 1]</span> that means all doors are unlocked.</p><p>It can be seen that for the first and for the third example inputs it is not possible to make all doors unlocked.</p>
