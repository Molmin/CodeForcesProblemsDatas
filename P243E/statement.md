## Description

<div><p>Let's consider an <span class="tex-span"><i>n</i> × <i>n</i></span> square matrix, consisting of digits one and zero.</p><p>We'll consider a matrix <span class="tex-font-style-it">good</span>, if it meets the following condition: in each row of the matrix all ones go in one group. That is, each row of the matrix looks like that <span class="tex-span">00...0011...1100...00</span> (or simply consists of zeroes if it has no ones).</p><p>You are given matrix <span class="tex-span"><i>a</i></span> of size <span class="tex-span"><i>n</i> × <i>n</i></span>, consisting of zeroes and ones. Your task is to determine whether you can get a good matrix <span class="tex-span"><i>b</i></span> from it by rearranging the columns or not.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>) — the size of matrix <span class="tex-span"><i>a</i></span>.</p><p>Each of <span class="tex-span"><i>n</i></span> following lines contains <span class="tex-span"><i>n</i></span> characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>" — matrix <span class="tex-span"><i>a</i></span>. Note that the characters are written without separators.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" in the first line, if you can rearrange the matrix columns so as to get a good matrix <span class="tex-span"><i>b</i></span>. In the next <span class="tex-span"><i>n</i></span> lines print the good matrix <span class="tex-span"><i>b</i></span>. If there are multiple answers, you are allowed to print any of them.</p><p>If it is impossible to get a good matrix, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>) — the size of matrix <span class="tex-span"><i>a</i></span>.</p><p>Each of <span class="tex-span"><i>n</i></span> following lines contains <span class="tex-span"><i>n</i></span> characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>" — matrix <span class="tex-span"><i>a</i></span>. Note that the characters are written without separators.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" in the first line, if you can rearrange the matrix columns so as to get a good matrix <span class="tex-span"><i>b</i></span>. In the next <span class="tex-span"><i>n</i></span> lines print the good matrix <span class="tex-span"><i>b</i></span>. If there are multiple answers, you are allowed to print any of them.</p><p>If it is impossible to get a good matrix, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
6
100010
110110
011001
010010
000100
011001

```




```input2
3
110
101
011

```




```output1
YES
011000
111100
000111
001100
100000
000111

```




```output2
NO

```


