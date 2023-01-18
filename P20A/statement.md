## Description

<div><p>The new operating system BerOS has a nice feature. It is possible to use any number of characters <span class="tex-font-style-tt">'/'</span> as a delimiter in path instead of one traditional <span class="tex-font-style-tt">'/'</span>. For example, strings <span class="tex-font-style-tt">//usr///local//nginx/sbin//</span> and <span class="tex-font-style-tt">/usr/local/nginx///sbin</span> are equivalent. The character <span class="tex-font-style-tt">'/'</span> (or some sequence of such characters) at the end of the path is required only in case of the path to the root directory, which can be represented as single character <span class="tex-font-style-tt">'/'</span>.</p><p>A path called normalized if it contains the smallest possible number of characters <span class="tex-font-style-tt">'/'</span>.</p><p>Your task is to transform a given path to the normalized form.</p></div><div class="input-specification"><p>The first line of the input contains only lowercase Latin letters and character <span class="tex-font-style-tt">'/'</span>&nbsp;— the path to some directory. All paths start with at least one character <span class="tex-font-style-tt">'/'</span>. The length of the given line is no more than 100 characters, it is not empty.</p></div><div class="output-specification"><p>The path in normalized form.</p></div>

## Input

<p>The first line of the input contains only lowercase Latin letters and character <span class="tex-font-style-tt">'/'</span>&nbsp;— the path to some directory. All paths start with at least one character <span class="tex-font-style-tt">'/'</span>. The length of the given line is no more than 100 characters, it is not empty.</p>

## Output

<p>The path in normalized form.</p>





```input1
//usr///local//nginx/sbin

```




```output1
/usr/local/nginx/sbin

```


