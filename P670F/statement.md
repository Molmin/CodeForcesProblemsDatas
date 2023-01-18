## Description

<div><p>Vasya decided to pass a very large integer <span class="tex-span"><i>n</i></span> to Kate. First, he wrote that number as a string, then he appended to the right integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of digits in <span class="tex-span"><i>n</i></span>. </p><p>Magically, all the numbers were shuffled in arbitrary order while this note was passed to Kate. The only thing that Vasya remembers, is a non-empty substring of <span class="tex-span"><i>n</i></span> (a substring of <span class="tex-span"><i>n</i></span> is a sequence of consecutive digits of the number <span class="tex-span"><i>n</i></span>).</p><p>Vasya knows that there may be more than one way to restore the number <span class="tex-span"><i>n</i></span>. Your task is to find the smallest possible initial integer <span class="tex-span"><i>n</i></span>. Note that decimal representation of number <span class="tex-span"><i>n</i></span> contained no leading zeroes, except the case the integer <span class="tex-span"><i>n</i></span> was equal to zero itself (in this case a single digit <span class="tex-font-style-tt">0</span> was used).</p></div><div class="input-specification"><p>The first line of the input contains the string received by Kate. The number of digits in this string does not exceed <span class="tex-span">1 000 000</span>.</p><p>The second line contains the substring of <span class="tex-span"><i>n</i></span> which Vasya remembers. This string can contain leading zeroes. </p><p>It is guaranteed that the input data is correct, and the answer always exists.</p></div><div class="output-specification"><p>Print the smalles integer <span class="tex-span"><i>n</i></span> which Vasya could pass to Kate.</p></div>

## Input

<p>The first line of the input contains the string received by Kate. The number of digits in this string does not exceed <span class="tex-span">1 000 000</span>.</p><p>The second line contains the substring of <span class="tex-span"><i>n</i></span> which Vasya remembers. This string can contain leading zeroes. </p><p>It is guaranteed that the input data is correct, and the answer always exists.</p>

## Output

<p>Print the smalles integer <span class="tex-span"><i>n</i></span> which Vasya could pass to Kate.</p>





```input1
003512
021

```




```input2
199966633300
63

```




```output1
30021

```




```output2
3036366999

```


