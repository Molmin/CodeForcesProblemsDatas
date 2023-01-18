## Description

<div><p>As Famil Door’s birthday is coming, some of his friends (like Gabi) decided to buy a present for him. His friends are going to buy a string consisted of round brackets since Famil Door loves string of brackets of length <span class="tex-span"><i>n</i></span> more than any other strings!</p><p>The sequence of round brackets is called <span class="tex-font-style-it">valid</span> if and only if: </p><ol> <li> the total number of opening brackets is equal to the total number of closing brackets; </li><li> for any prefix of the sequence, the number of opening brackets is greater or equal than the number of closing brackets. </li></ol><p>Gabi bought a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>m</i></span> (<span class="tex-span"><i>m</i> ≤ <i>n</i></span>) and want to complete it to obtain a valid sequence of brackets of length <span class="tex-span"><i>n</i></span>. He is going to pick some strings <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> consisting of round brackets and merge them in a string <span class="tex-span"><i>p</i> + <i>s</i> + <i>q</i></span>, that is add the string <span class="tex-span"><i>p</i></span> at the beginning of the string <span class="tex-span"><i>s</i></span> and string <span class="tex-span"><i>q</i></span> at the end of the string <span class="tex-span"><i>s</i></span>.</p><p>Now he wonders, how many <span class="tex-font-style-bf">pairs</span> of strings <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> exists, such that the string <span class="tex-span"><i>p</i> + <i>s</i> + <i>q</i></span> is a valid sequence of round brackets. As this number may be pretty large, he wants to calculate it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>First line contains <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 100 000, <i>n</i> - <i>m</i> ≤ 2000</span>)&nbsp;— the desired length of the string and the length of the string bought by Gabi, respectively.</p><p>The second line contains string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>m</i></span> consisting of characters '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>' only.</p></div><div class="output-specification"><p>Print the number of pairs of string <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> such that <span class="tex-span"><i>p</i> + <i>s</i> + <i>q</i></span> is a valid sequence of round brackets modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>First line contains <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 100 000, <i>n</i> - <i>m</i> ≤ 2000</span>)&nbsp;— the desired length of the string and the length of the string bought by Gabi, respectively.</p><p>The second line contains string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>m</i></span> consisting of characters '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>' only.</p>

## Output

<p>Print the number of pairs of string <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> such that <span class="tex-span"><i>p</i> + <i>s</i> + <i>q</i></span> is a valid sequence of round brackets modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
4 1
(

```




```input2
4 4
(())

```




```input3
4 3
(((

```




```output1
4

```




```output2
1

```




```output3
0

```



## Note

<p>In the first sample there are four different valid pairs: </p><ol> <li> <span class="tex-span"><i>p</i> = </span>"<span class="tex-font-style-tt">(</span>", <span class="tex-span"><i>q</i> = </span>"<span class="tex-font-style-tt">))</span>" </li><li> <span class="tex-span"><i>p</i> = </span>"<span class="tex-font-style-tt">()</span>", <span class="tex-span"><i>q</i> = </span>"<span class="tex-font-style-tt">)</span>" </li><li> <span class="tex-span"><i>p</i> = </span>"", <span class="tex-span"><i>q</i> = </span>"<span class="tex-font-style-tt">())</span>" </li><li> <span class="tex-span"><i>p</i> = </span>"", <span class="tex-span"><i>q</i> = </span>"<span class="tex-font-style-tt">)()</span>" </li></ol><p>In the second sample the only way to obtain a desired string is choose empty <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span>.</p><p>In the third sample there is no way to get a valid sequence of brackets.</p>
