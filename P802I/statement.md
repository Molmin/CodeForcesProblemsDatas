## Description

<div><p>Now that you have proposed a fake post for the HC<span class="tex-span"><sup class="upper-index">2</sup></span> Facebook page, Heidi wants to measure the quality of the post before actually posting it. She recently came across a (possibly fake) article about the impact of fractal structure on multimedia messages and she is now trying to measure the self-similarity of the message, which is defined as</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://3QErjKIs.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>where the sum is over all nonempty strings <span class="tex-span"><i>p</i></span> and <img align="middle" class="tex-formula" src="file://LjBkv2p4.png" style="max-width: 100.0%;max-height: 100.0%;"> is the number of occurences of <span class="tex-span"><i>p</i></span> in <span class="tex-span"><i>s</i></span> as a <span class="tex-font-style-bf">substring</span>. (Note that the sum is infinite, but it only has a finite number of nonzero summands.)</p><p>Heidi refuses to do anything else until she knows how to calculate this self-similarity. Could you please help her? (If you would like to instead convince Heidi that a finite string cannot be a fractal anyway – do not bother, we have already tried.)</p></div><div class="input-specification"><p>The input starts with a line indicating the number of test cases <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 10</span>). After that, <span class="tex-span"><i>T</i></span> test cases follow, each of which consists of one line containing a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100 000</span>) composed of lowercase letters (<span class="tex-font-style-tt">a</span>-<span class="tex-font-style-tt">z</span>).</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>T</i></span> lines, every line containing one number – the answer to the corresponding test case.</p></div>

## Input

<p>The input starts with a line indicating the number of test cases <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 10</span>). After that, <span class="tex-span"><i>T</i></span> test cases follow, each of which consists of one line containing a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100 000</span>) composed of lowercase letters (<span class="tex-font-style-tt">a</span>-<span class="tex-font-style-tt">z</span>).</p>

## Output

<p>Output <span class="tex-span"><i>T</i></span> lines, every line containing one number – the answer to the corresponding test case.</p>





```input1
4
aa
abcd
ccc
abcc

```




```output1
5
10
14
12

```



## Note

<p>A string <span class="tex-span"><i>s</i></span> contains another string <span class="tex-span"><i>p</i></span> as a substring if <span class="tex-span"><i>p</i></span> is a contiguous subsequence of <span class="tex-span"><i>s</i></span>. For example, <span class="tex-font-style-tt">ab</span> is a substring of <span class="tex-font-style-tt">cab</span> but not of <span class="tex-font-style-tt">acb</span>.</p>
