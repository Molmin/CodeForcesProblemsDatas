## Description

<div><p>Limak is a little polar bear. In the snow he found a scroll with the ancient prophecy. Limak doesn't know any ancient languages and thus is unable to understand the prophecy. But he knows digits!</p><p>One fragment of the prophecy is a sequence of <span class="tex-span"><i>n</i></span> digits. The first digit isn't zero. Limak thinks that it's a list of some special years. It's hard to see any commas or spaces, so maybe ancient people didn't use them. Now Limak wonders what years are listed there.</p><p>Limak assumes three things:</p><ul> <li> Years are listed in the <span class="tex-font-style-bf">strictly</span> increasing order; </li><li> Every year is a positive integer number; </li><li> There are no leading zeros. </li></ul><p>Limak is going to consider all possible ways to split a sequence into numbers (years), satisfying the conditions above. He will do it without any help. However, he asked you to tell him the number of ways to do so. Since this number may be very large, you are only asked to calculate it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the number of digits.</p><p>The second line contains a string of digits and has length equal to <span class="tex-span"><i>n</i></span>. It's guaranteed that the first digit is not '<span class="tex-font-style-tt">0</span>'.</p></div><div class="output-specification"><p>Print the number of ways to correctly split the given sequence modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the number of digits.</p><p>The second line contains a string of digits and has length equal to <span class="tex-span"><i>n</i></span>. It's guaranteed that the first digit is not '<span class="tex-font-style-tt">0</span>'.</p>

## Output

<p>Print the number of ways to correctly split the given sequence modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
6
123434

```




```input2
8
20152016

```




```output1
8

```




```output2
4

```



## Note

<p>In the first sample there are <span class="tex-span">8</span> ways to split the sequence:</p><ul> <li> "<span class="tex-font-style-tt">123434</span>" = "<span class="tex-font-style-tt">123434</span>" (maybe the given sequence is just one big number) </li><li> "<span class="tex-font-style-tt">123434</span>" = "<span class="tex-font-style-tt">1</span>" + "<span class="tex-font-style-tt">23434</span>" </li><li> "<span class="tex-font-style-tt">123434</span>" = "<span class="tex-font-style-tt">12</span>" + "<span class="tex-font-style-tt">3434</span>" </li><li> "<span class="tex-font-style-tt">123434</span>" = "<span class="tex-font-style-tt">123</span>" + "<span class="tex-font-style-tt">434</span>" </li><li> "<span class="tex-font-style-tt">123434</span>" = "<span class="tex-font-style-tt">1</span>" + "<span class="tex-font-style-tt">23</span>" + "<span class="tex-font-style-tt">434</span>" </li><li> "<span class="tex-font-style-tt">123434</span>" = "<span class="tex-font-style-tt">1</span>" + "<span class="tex-font-style-tt">2</span>" + "<span class="tex-font-style-tt">3434</span>" </li><li> "<span class="tex-font-style-tt">123434</span>" = "<span class="tex-font-style-tt">1</span>" + "<span class="tex-font-style-tt">2</span>" + "<span class="tex-font-style-tt">3</span>" + "<span class="tex-font-style-tt">434</span>" </li><li> "<span class="tex-font-style-tt">123434</span>" = "<span class="tex-font-style-tt">1</span>" + "<span class="tex-font-style-tt">2</span>" + "<span class="tex-font-style-tt">3</span>" + "<span class="tex-font-style-tt">4</span>" + "<span class="tex-font-style-tt">34</span>" </li></ul><p>Note that we don't count a split "<span class="tex-font-style-tt">123434</span>" = "<span class="tex-font-style-tt">12</span>" + "<span class="tex-font-style-tt">34</span>" + "<span class="tex-font-style-tt">34</span>" because numbers have to be strictly increasing.</p><p>In the second sample there are <span class="tex-span">4</span> ways:</p><ul> <li> "<span class="tex-font-style-tt">20152016</span>" = "<span class="tex-font-style-tt">20152016</span>" </li><li> "<span class="tex-font-style-tt">20152016</span>" = "<span class="tex-font-style-tt">20</span>" + "<span class="tex-font-style-tt">152016</span>" </li><li> "<span class="tex-font-style-tt">20152016</span>" = "<span class="tex-font-style-tt">201</span>" + "<span class="tex-font-style-tt">52016</span>" </li><li> "<span class="tex-font-style-tt">20152016</span>" = "<span class="tex-font-style-tt">2015</span>" + "<span class="tex-font-style-tt">2016</span>" </li></ul>
