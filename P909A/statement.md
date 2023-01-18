## Description

<div><p>The preferred way to generate user login in Polygon is to concatenate a prefix of the user's first name and a prefix of their last name, in that order. Each prefix must be non-empty, and any of the prefixes can be the full name. Typically there are multiple possible logins for each person.</p><p>You are given the first and the last name of a user. Return the alphabetically earliest login they can get (regardless of other potential Polygon users).</p><p>As a reminder, a prefix of a string <span class="tex-span"><i>s</i></span> is its substring which occurs at the beginning of <span class="tex-span"><i>s</i></span>: "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">abc</span>" etc. are prefixes of string "{abcdef}" but "<span class="tex-font-style-tt">b</span>" and '<span class="tex-font-style-tt">bc</span>" are not. A string <span class="tex-span"><i>a</i></span> is alphabetically earlier than a string <span class="tex-span"><i>b</i></span>, if <span class="tex-span"><i>a</i></span> is a prefix of <span class="tex-span"><i>b</i></span>, or <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> coincide up to some position, and then <span class="tex-span"><i>a</i></span> has a letter that is alphabetically earlier than the corresponding letter in <span class="tex-span"><i>b</i></span>: "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">ab</span>" are alphabetically earlier than "<span class="tex-font-style-tt">ac</span>" but "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">ba</span>" are alphabetically later than "<span class="tex-font-style-tt">ac</span>".</p></div><div class="input-specification"><p>The input consists of a single line containing two space-separated strings: the first and the last names. Each character of each string is a lowercase English letter. The length of each string is between 1 and 10, inclusive. </p></div><div class="output-specification"><p>Output a single string&nbsp;— alphabetically earliest possible login formed from these names. The output should be given in lowercase as well.</p></div>

## Input

<p>The input consists of a single line containing two space-separated strings: the first and the last names. Each character of each string is a lowercase English letter. The length of each string is between 1 and 10, inclusive. </p>

## Output

<p>Output a single string&nbsp;— alphabetically earliest possible login formed from these names. The output should be given in lowercase as well.</p>





```input1
harry potter

```




```input2
tom riddle

```




```output1
hap

```




```output2
tomr

```


