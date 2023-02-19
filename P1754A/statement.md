## Description

<div><p>You work in the quality control department of technical support for a large company. Your job is to make sure all client issues have been resolved.</p><p>Today you need to check a copy of a dialog between a client and a technical support manager. According to the rules of work, each message of the client must be followed by <span class="tex-font-style-bf">one or several</span> messages, which are the answer of a support manager. However, sometimes clients ask questions so quickly that some of the manager's answers to old questions appear after the client has asked some new questions.</p><p>Due to the privacy policy, the full text of messages is not available to you, only the order of messages is visible, as well as the type of each message: a customer question or a response from the technical support manager. <span class="tex-font-style-bf">It is guaranteed that the dialog begins with the question of the client.</span></p><p>You have to determine, if this dialog may correspond to the rules of work described above, or the rules are certainly breached.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). Description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 100$)&nbsp;— the total number of messages in the dialog.</p><p>The second line of each test case consists of $n$ characters "<span class="tex-font-style-tt">Q</span>" and "<span class="tex-font-style-tt">A</span>", describing types of messages in the dialog in chronological order. Character "<span class="tex-font-style-tt">Q</span>" denotes the message with client question, and character "<span class="tex-font-style-tt">A</span>"&nbsp;— the message with technical support manager answer. It is guaranteed that the first character in the line equals to "<span class="tex-font-style-tt">Q</span>".</p></div><div class="output-specification"><p>For each test case print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if dialog may correspond to the rules of work, or "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). Description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 100$)&nbsp;— the total number of messages in the dialog.</p><p>The second line of each test case consists of $n$ characters "<span class="tex-font-style-tt">Q</span>" and "<span class="tex-font-style-tt">A</span>", describing types of messages in the dialog in chronological order. Character "<span class="tex-font-style-tt">Q</span>" denotes the message with client question, and character "<span class="tex-font-style-tt">A</span>"&nbsp;— the message with technical support manager answer. It is guaranteed that the first character in the line equals to "<span class="tex-font-style-tt">Q</span>".</p>

## Output

<p>For each test case print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if dialog may correspond to the rules of work, or "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p>





```input1|2,3,6,7,10,11
5
4
QQAA
4
QQAQ
3
QAA
1
Q
14
QAQQAQAAQQQAAA
```




```output1
Yes
No
Yes
No
Yes
```



## Note

<p>In the first test case the two questions from the client are followed with two specialist's answers. So this dialog may correspond to the rules of work.</p><p>In the second test case one of the first two questions was not answered.</p><p>In the third test case the technical support manager sent two messaged as the answer to the only message of the client.</p>
