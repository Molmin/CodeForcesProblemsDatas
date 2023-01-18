## Description

<div><p>Mad scientist Mike has just finished constructing a new device to search for extraterrestrial intelligence! He was in such a hurry to launch it for the first time that he plugged in the power wires without giving it a proper glance and started experimenting right away. After a while Mike observed that the wires ended up entangled and now have to be untangled again.</p><p>The device is powered by two wires "plus" and "minus". The wires run along the floor from the wall (on the left) to the device (on the right). Both the wall and the device have two contacts in them on the same level, into which the wires are plugged in some order. The wires are considered entangled if there are one or more places where one wire runs above the other one. For example, the picture below has four such places (top view):</p><center> <img class="tex-graphics" src="file://fzba9cSA.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Mike knows the sequence in which the wires run above each other. Mike also noticed that on the left side, the "plus" wire is always plugged into the top contact (as seen on the picture). He would like to untangle the wires without unplugging them and <span class="tex-font-style-bf">without moving</span> the device. Determine if it is possible to do that. A wire can be freely moved and stretched on the floor, but cannot be cut.</p><p>To understand the problem better please read the notes to the test samples.</p></div><div class="input-specification"><p>The single line of the input contains a sequence of characters "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">-</span>" of length <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>). The <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) position of the sequence contains the character "<span class="tex-font-style-tt">+</span>", if on the <span class="tex-span"><i>i</i></span>-th step from the wall the "plus" wire runs above the "minus" wire, and the character "<span class="tex-font-style-tt">-</span>" otherwise.</p></div><div class="output-specification"><p>Print either "<span class="tex-font-style-tt">Yes</span>" (without the quotes) if the wires can be untangled or "<span class="tex-font-style-tt">No</span>" (without the quotes) if the wires cannot be untangled.</p></div>

## Input

<p>The single line of the input contains a sequence of characters "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">-</span>" of length <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>). The <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) position of the sequence contains the character "<span class="tex-font-style-tt">+</span>", if on the <span class="tex-span"><i>i</i></span>-th step from the wall the "plus" wire runs above the "minus" wire, and the character "<span class="tex-font-style-tt">-</span>" otherwise.</p>

## Output

<p>Print either "<span class="tex-font-style-tt">Yes</span>" (without the quotes) if the wires can be untangled or "<span class="tex-font-style-tt">No</span>" (without the quotes) if the wires cannot be untangled.</p>





```input1
-++-

```




```input2
+-

```




```input3
++

```




```input4
-

```




```output1
Yes

```




```output2
No

```




```output3
Yes

```




```output4
No

```



## Note

<p>The first testcase corresponds to the picture in the statement. To untangle the wires, one can first move the "plus" wire lower, thus eliminating the two crosses in the middle, and then draw it under the "minus" wire, eliminating also the remaining two crosses.</p><p>In the second testcase the "plus" wire makes one full revolution around the "minus" wire. Thus the wires cannot be untangled: </p><center> <img class="tex-graphics" src="file://aIGVa3Fa.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third testcase the "plus" wire simply runs above the "minus" wire twice in sequence. The wires can be untangled by lifting "plus" and moving it higher: </p><center> <img class="tex-graphics" src="file://b9gezIPt.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the fourth testcase the "minus" wire runs above the "plus" wire once. The wires cannot be untangled without moving the device itself: </p><center> <img class="tex-graphics" src="file://BbGAFu0G.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
