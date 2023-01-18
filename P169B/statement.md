## Description

<div><p>You are given an integer <span class="tex-span"><i>a</i></span> that consists of <span class="tex-span"><i>n</i></span> digits. You are also given a sequence of digits <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>m</i></span>. The digit in position <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>) of sequence <span class="tex-span"><i>s</i></span> means that you can choose an arbitrary position <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) in <span class="tex-span"><i>a</i></span> and replace the digit in the chosen position <span class="tex-span"><i>i</i></span> with <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub></span>. Each element in the sequence <span class="tex-span"><i>s</i></span> can participate in no more than one replacing operation.</p><p>Your task is to perform such sequence of replacements, that the given number <span class="tex-span"><i>a</i></span> gets maximum value. You are allowed to use not all elements from <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The first line contains positive integer <span class="tex-span"><i>a</i></span>. Its length <span class="tex-span"><i>n</i></span> is positive and doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. The second line contains sequence of digits <span class="tex-span"><i>s</i></span>. Its length <span class="tex-span"><i>m</i></span> is positive and doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. The digits in the sequence <span class="tex-span"><i>s</i></span> are written consecutively without any separators.</p><p>The given number <span class="tex-span"><i>a</i></span> doesn't contain leading zeroes. </p></div><div class="output-specification"><p>Print the maximum value that can be obtained from <span class="tex-span"><i>a</i></span> after a series of replacements. You are allowed to use not all elements from <span class="tex-span"><i>s</i></span>. The printed number shouldn't contain any leading zeroes.</p></div>

## Input

<p>The first line contains positive integer <span class="tex-span"><i>a</i></span>. Its length <span class="tex-span"><i>n</i></span> is positive and doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. The second line contains sequence of digits <span class="tex-span"><i>s</i></span>. Its length <span class="tex-span"><i>m</i></span> is positive and doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. The digits in the sequence <span class="tex-span"><i>s</i></span> are written consecutively without any separators.</p><p>The given number <span class="tex-span"><i>a</i></span> doesn't contain leading zeroes. </p>

## Output

<p>Print the maximum value that can be obtained from <span class="tex-span"><i>a</i></span> after a series of replacements. You are allowed to use not all elements from <span class="tex-span"><i>s</i></span>. The printed number shouldn't contain any leading zeroes.</p>





```input1
1024
010

```




```input2
987
1234567

```




```output1
1124

```




```output2
987

```


