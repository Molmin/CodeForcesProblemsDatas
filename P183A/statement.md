## Description

<div><p>Sensation, sensation in the two-dimensional kingdom! The police have caught a highly dangerous outlaw, member of the notorious "Pihters" gang. The law department states that the outlaw was driving from the gang's headquarters in his car when he crashed into an ice cream stall. The stall, the car, and the headquarters each occupies exactly one point on the two-dimensional kingdom.</p><p>The outlaw's car was equipped with a GPS transmitter. The transmitter showed that the car made <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>n</i></span> movements on its way from the headquarters to the stall. A movement can move the car from point <span class="tex-span">(<i>x</i>, <i>y</i>)</span> to one of these four points: to point <span class="tex-span">(<i>x</i> - 1, <i>y</i>)</span> which we will mark by letter "<span class="tex-font-style-tt">L</span>", to point <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span> — "<span class="tex-font-style-tt">R</span>", to point <span class="tex-span">(<i>x</i>, <i>y</i> - 1)</span> — "<span class="tex-font-style-tt">D</span>", to point <span class="tex-span">(<i>x</i>, <i>y</i> + 1)</span> — "<span class="tex-font-style-tt">U</span>".</p><p>The GPS transmitter is very inaccurate and it doesn't preserve the exact sequence of the car's movements. Instead, it keeps records of the car's possible movements. Each record is a string of one of these types: "<span class="tex-font-style-tt">UL</span>", "<span class="tex-font-style-tt">UR</span>", "<span class="tex-font-style-tt">DL</span>", "<span class="tex-font-style-tt">DR</span>" or "<span class="tex-font-style-tt">ULDR</span>". Each such string means that the car made a single movement corresponding to one of the characters of the string. For example, string "<span class="tex-font-style-tt">UL</span>" means that the car moved either "<span class="tex-font-style-tt">U</span>", or "<span class="tex-font-style-tt">L</span>".</p><p>You've received the journal with the outlaw's possible movements from the headquarters to the stall. The journal records are given in a chronological order. Given that the ice-cream stall is located at point <span class="tex-span">(0, 0)</span>, your task is to print the number of different points that can contain the gang headquarters (that is, the number of different possible locations of the car's origin).</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> — the number of the car's movements from the headquarters to the stall.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines describes the car's possible movements. It is guaranteed that each possible movement is one of the following strings: "<span class="tex-font-style-tt">UL</span>", "<span class="tex-font-style-tt">UR</span>", "<span class="tex-font-style-tt">DL</span>", "<span class="tex-font-style-tt">DR</span>" or "<span class="tex-font-style-tt">ULDR</span>". </p><p>All movements are given in chronological order. </p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span> and <span class="tex-font-style-tt">cout</span> stream or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print a single integer — the number of different possible locations of the gang's headquarters.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> — the number of the car's movements from the headquarters to the stall.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines describes the car's possible movements. It is guaranteed that each possible movement is one of the following strings: "<span class="tex-font-style-tt">UL</span>", "<span class="tex-font-style-tt">UR</span>", "<span class="tex-font-style-tt">DL</span>", "<span class="tex-font-style-tt">DR</span>" or "<span class="tex-font-style-tt">ULDR</span>". </p><p>All movements are given in chronological order. </p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span> and <span class="tex-font-style-tt">cout</span> stream or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print a single integer — the number of different possible locations of the gang's headquarters.</p>





```input1
3
UR
UL
ULDR

```




```input2
2
DR
DL

```




```output1
9

```




```output2
4

```



## Note

<p>The figure below shows the nine possible positions of the gang headquarters from the first sample: </p><center> <img class="tex-graphics" src="file://qOPnx5Nj.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For example, the following movements can get the car from point <span class="tex-span">(1, 0)</span> to point <span class="tex-span">(0, 0)</span>: </p><center> <img class="tex-graphics" src="file://SEC4SdpC.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
