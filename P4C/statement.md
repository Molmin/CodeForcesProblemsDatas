## Description

<div><p>A new e-mail service "Berlandesk" is going to be opened in Berland in the near future. The site administration wants to launch their project as soon as possible, that's why they ask you to help. You're suggested to implement the prototype of site registration system. The system should work on the following principle. </p><p>Each time a new user wants to register, he sends to the system a request with his <span class="tex-font-style-tt">name</span>. If such a <span class="tex-font-style-tt">name</span> does not exist in the system database, it is inserted into the database, and the user gets the response <span class="tex-font-style-tt">OK</span>, confirming the successful registration. If the <span class="tex-font-style-tt">name</span> already exists in the system database, the system makes up a new user name, sends it to the user as a prompt and <span class="tex-font-style-it">also inserts the prompt into the database</span>. The new name is formed by the following rule. Numbers, starting with 1, are appended one after another to <span class="tex-font-style-tt">name</span> (<span class="tex-font-style-tt">name1</span>, <span class="tex-font-style-tt">name2</span>, ...), among these numbers the least <span class="tex-span"><i>i</i></span> is found so that <span class="tex-font-style-tt">name</span><span class="tex-span"><i>i</i></span> does not yet exist in the database.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The following <span class="tex-span"><i>n</i></span> lines contain the requests to the system. Each request is a non-empty line, and consists of not more than 32 characters, which are all lowercase Latin letters.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines, which are system responses to the requests: <span class="tex-font-style-tt">OK</span> in case of successful registration, or a prompt with a new name, if the requested name is already taken.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The following <span class="tex-span"><i>n</i></span> lines contain the requests to the system. Each request is a non-empty line, and consists of not more than 32 characters, which are all lowercase Latin letters.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines, which are system responses to the requests: <span class="tex-font-style-tt">OK</span> in case of successful registration, or a prompt with a new name, if the requested name is already taken.</p>





```input1
4
abacaba
acaba
abacaba
acab

```




```input2
6
first
first
second
second
third
third

```




```output1
OK
OK
abacaba1
OK

```




```output2
OK
first1
OK
second1
OK
third1

```


