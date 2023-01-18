## Description

<div><p>Two neighboring kingdoms decided to build a wall between them with some gates to enable the citizens to go from one kingdom to another. Each time a citizen passes through a gate, he has to pay one silver coin.</p><p>The world can be represented by the first quadrant of a plane and the wall is built along the identity line (i.e. the line with the equation <span class="tex-span"><i>x</i> = <i>y</i></span>). Any point below the wall belongs to the first kingdom while any point above the wall belongs to the second kingdom. There is a gate at any integer point on the line (i.e. at points <span class="tex-span">(0, 0)</span>, <span class="tex-span">(1, 1)</span>, <span class="tex-span">(2, 2)</span>, ...). The wall and the gates do not belong to any of the kingdoms. </p><p>Fafa is at the gate at position <span class="tex-span">(0, 0)</span> and he wants to walk around in the two kingdoms. He knows the sequence <span class="tex-span"><i>S</i></span> of moves he will do. This sequence is a string where each character represents a move. The two possible moves Fafa will do are '<span class="tex-font-style-tt">U</span>' (move one step up, from <span class="tex-span">(<i>x</i>, <i>y</i>)</span> to <span class="tex-span">(<i>x</i>, <i>y</i> + 1)</span>) and '<span class="tex-font-style-tt">R</span>' (move one step right, from <span class="tex-span">(<i>x</i>, <i>y</i>)</span> to <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span>). </p><p>Fafa wants to know the number of silver coins he needs to pay to walk around the two kingdoms following the sequence <span class="tex-span"><i>S</i></span>. Note that if Fafa visits a gate without moving from one kingdom to another, he pays no silver coins. Also assume that he doesn't pay at the gate at point <span class="tex-span">(0, 0)</span>, i.&nbsp;e. he is initially on the side he needs. </p></div><div class="input-specification"><p>The first line of the input contains single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of moves in the walking sequence.</p><p>The second line contains a string <span class="tex-span"><i>S</i></span> of length <span class="tex-span"><i>n</i></span> consisting of the characters '<span class="tex-font-style-tt">U</span>' and '<span class="tex-font-style-tt">R</span>' describing the required moves. Fafa will follow the sequence <span class="tex-span"><i>S</i></span> in order from left to right.</p></div><div class="output-specification"><p>On a single line, print one integer representing the number of silver coins Fafa needs to pay at the gates to follow the sequence <span class="tex-span"><i>S</i></span>.</p></div>

## Input

<p>The first line of the input contains single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of moves in the walking sequence.</p><p>The second line contains a string <span class="tex-span"><i>S</i></span> of length <span class="tex-span"><i>n</i></span> consisting of the characters '<span class="tex-font-style-tt">U</span>' and '<span class="tex-font-style-tt">R</span>' describing the required moves. Fafa will follow the sequence <span class="tex-span"><i>S</i></span> in order from left to right.</p>

## Output

<p>On a single line, print one integer representing the number of silver coins Fafa needs to pay at the gates to follow the sequence <span class="tex-span"><i>S</i></span>.</p>





```input1
1
U

```




```input2
6
RURUUR

```




```input3
7
URRRUUU

```




```output1
0

```




```output2
1

```




```output3
2

```



## Note

<p>The figure below describes the third sample. The red arrows represent the sequence of moves Fafa will follow. The green gates represent the gates at which Fafa have to pay silver coins.</p><center> <img class="tex-graphics" src="file://I2v2lszu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
