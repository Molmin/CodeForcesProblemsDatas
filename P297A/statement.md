## Description

<div><p>You are fishing with polar bears Alice and Bob. While waiting for the fish to bite, the polar bears get bored. They come up with a game. First Alice and Bob each writes a 01-string (strings that only contain character "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>") <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Then you try to turn <span class="tex-span"><i>a</i></span> into <span class="tex-span"><i>b</i></span> using two types of operations:</p><ul> <li> Write <span class="tex-span"><i>parity</i>(<i>a</i>)</span> to the end of <span class="tex-span"><i>a</i></span>. For example, <img align="middle" class="tex-formula" src="file://zE8NjTfy.png" style="max-width: 100.0%;max-height: 100.0%;">. </li><li> Remove the first character of <span class="tex-span"><i>a</i></span>. For example, <img align="middle" class="tex-formula" src="file://3Dsn0qF6.png" style="max-width: 100.0%;max-height: 100.0%;">. You cannot perform this operation if <span class="tex-span"><i>a</i></span> is empty. </li></ul><p>You can use as many operations as you want. The problem is, is it possible to turn <span class="tex-span"><i>a</i></span> into <span class="tex-span"><i>b</i></span>?</p><p>The <span class="tex-span"><i>parity</i></span> of a 01-string is <span class="tex-span">1</span> if there is an odd number of "<span class="tex-font-style-tt">1</span>"s in the string, and <span class="tex-span">0</span> otherwise.</p></div><div class="input-specification"><p>The first line contains the string <span class="tex-span"><i>a</i></span> and the second line contains the string <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ |<i>a</i>|, |<i>b</i>| ≤ 1000)</span>. Both strings contain only the characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>". Here <span class="tex-span">|<i>x</i>|</span> denotes the length of the string <span class="tex-span"><i>x</i></span>.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to turn <span class="tex-span"><i>a</i></span> into <span class="tex-span"><i>b</i></span>, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p></div>

## Input

<p>The first line contains the string <span class="tex-span"><i>a</i></span> and the second line contains the string <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ |<i>a</i>|, |<i>b</i>| ≤ 1000)</span>. Both strings contain only the characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>". Here <span class="tex-span">|<i>x</i>|</span> denotes the length of the string <span class="tex-span"><i>x</i></span>.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to turn <span class="tex-span"><i>a</i></span> into <span class="tex-span"><i>b</i></span>, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p>





```input1
01011
0110

```




```input2
0011
1110

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample, the steps are as follows: <span class="tex-span">01011 → 1011 → 011 → 0110</span></p>
