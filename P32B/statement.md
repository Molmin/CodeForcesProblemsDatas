## Description

<div><p>Ternary numeric notation is quite popular in Berland. To telegraph the ternary number the Borze alphabet is used. Digit 0 is transmitted as <span class="tex-font-style-tt">«.»</span>, 1 as <span class="tex-font-style-tt">«-.»</span> and 2 as <span class="tex-font-style-tt">«--»</span>. You are to decode the Borze code, i.e. to find out the ternary number given its representation in Borze alphabet.</p></div><div class="input-specification"><p>The first line contains a number in Borze code. The length of the string is between 1 and 200 characters. It's guaranteed that the given string is a valid Borze code of some ternary number (this number can have leading zeroes).</p></div><div class="output-specification"><p>Output the decoded ternary number. It can have leading zeroes.</p></div>

## Input

<p>The first line contains a number in Borze code. The length of the string is between 1 and 200 characters. It's guaranteed that the given string is a valid Borze code of some ternary number (this number can have leading zeroes).</p>

## Output

<p>Output the decoded ternary number. It can have leading zeroes.</p>





```input1
.-.--

```




```input2
--.

```




```input3
-..-.--

```




```output1
012
```




```output2
20
```




```output3
1012
```


