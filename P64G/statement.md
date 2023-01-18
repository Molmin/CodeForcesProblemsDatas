## Description

<div><p>A path in some Unix-similar file system is given. The path consists of elements separated with characters "<span class="tex-font-style-tt">/</span>". For example: "<span class="tex-font-style-tt">/usr/share/mysql/../tomcat6/conf/server.xml</span>". The path starts with the root directory (i.e. starts with the character "<span class="tex-font-style-tt">/</span>"). Each element means a name of file or directory, or it is one of two special elements: "<span class="tex-font-style-tt">.</span>" или "<span class="tex-font-style-tt">..</span>". First of them stands for the current directory (for example, path "<span class="tex-font-style-tt">/./usr/././share</span>" is equal to "<span class="tex-font-style-tt">/usr/share</span>"). The second element "<span class="tex-font-style-tt">..</span>" stands for the moving to the parent directory (for example, path "<span class="tex-font-style-tt">/usr/share/../lib</span>" is equal to "<span class="tex-font-style-tt">/usr/lib</span>").</p><p>You task is to convert the given path to such a path, which doesn't contain special elements "<span class="tex-font-style-tt">.</span>" and/or "<span class="tex-font-style-tt">..</span>". If it is impossible, print "<span class="tex-font-style-tt">-1</span>". The only reason for it is an attempt to move to the parent directory from the root.</p></div><div class="input-specification"><p>The only line contains the given path. The path starts with "<span class="tex-font-style-tt">/</span>" and consists of elements separated with "<span class="tex-font-style-tt">/</span>". No two "<span class="tex-font-style-tt">/</span>" follow one after another (consecutively). The only path which can end with "<span class="tex-font-style-tt">/</span>" is the root directory path equal to "<span class="tex-font-style-tt">/</span>".</p><p>Each element may contain "<span class="tex-font-style-tt">a</span>"-"<span class="tex-font-style-tt">z</span>", "<span class="tex-font-style-tt">0</span>"-"<span class="tex-font-style-tt">9</span>" and dots. Any element different from specials "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">..</span>" contains at least one character different from the dots.</p><p>The path length is between 1 and 1000 inclusively.</p></div><div class="output-specification"><p>Print the required path or "<span class="tex-font-style-tt">-1</span>".</p></div>

## Input

<p>The only line contains the given path. The path starts with "<span class="tex-font-style-tt">/</span>" and consists of elements separated with "<span class="tex-font-style-tt">/</span>". No two "<span class="tex-font-style-tt">/</span>" follow one after another (consecutively). The only path which can end with "<span class="tex-font-style-tt">/</span>" is the root directory path equal to "<span class="tex-font-style-tt">/</span>".</p><p>Each element may contain "<span class="tex-font-style-tt">a</span>"-"<span class="tex-font-style-tt">z</span>", "<span class="tex-font-style-tt">0</span>"-"<span class="tex-font-style-tt">9</span>" and dots. Any element different from specials "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">..</span>" contains at least one character different from the dots.</p><p>The path length is between 1 and 1000 inclusively.</p>

## Output

<p>Print the required path or "<span class="tex-font-style-tt">-1</span>".</p>





```input1
/usr/share/mysql/../tomcat6/conf/server.xml

```




```input2
/a/./././..

```




```output1
/usr/share/tomcat6/conf/server.xml

```




```output2
/

```


