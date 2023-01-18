## Description

<div><p>Polycarp is working on a new project called "Polychat". Following modern tendencies in IT, he decided, that this project should contain chat as well. To achieve this goal, Polycarp has spent several hours in front of his laptop and implemented a chat server that can process three types of commands:</p><ul> <li> Include a person to the chat (<span class="tex-font-style-tt">'Add'</span> command). </li><li> Remove a person from the chat (<span class="tex-font-style-tt">'Remove'</span> command). </li><li> Send a message from a person to all people, who are currently in the chat, including the one, who sends the message (<span class="tex-font-style-tt">'Send'</span> command). </li></ul><p>Now Polycarp wants to find out the amount of outgoing traffic that the server will produce while processing a particular set of commands.</p><p>Polycarp knows that chat server sends no traffic for 'Add' and 'Remove' commands. When 'Send' command is processed, server sends <span class="tex-span"><i>l</i></span> bytes to each participant of the chat, where <span class="tex-span"><i>l</i></span> is the length of the message.</p><p>As Polycarp has no time, he is asking for your help in solving this problem.</p></div><div class="input-specification"><p>Input file will contain not more than 100 commands, each in its own line. No line will exceed 100 characters. Formats of the commands will be the following:</p><ul> <li> <span class="tex-font-style-tt">+&lt;name&gt;</span> for <span class="tex-font-style-tt">'Add'</span> command. </li><li> <span class="tex-font-style-tt">-&lt;name&gt;</span> for <span class="tex-font-style-tt">'Remove'</span> command. </li><li> <span class="tex-font-style-tt">&lt;sender_name&gt;:&lt;message_text&gt;</span> for <span class="tex-font-style-tt">'Send'</span> command. </li></ul><p><span class="tex-font-style-tt">&lt;name&gt;</span> and <span class="tex-font-style-tt">&lt;sender_name&gt;</span> is a non-empty sequence of Latin letters and digits. <span class="tex-font-style-tt">&lt;message_text&gt;</span> can contain letters, digits and spaces, but can't start or end with a space. <span class="tex-font-style-tt">&lt;message_text&gt;</span> can be an empty line.</p><p>It is guaranteed, that input data are correct, i.e. there will be no <span class="tex-font-style-tt">'Add'</span> command if person with such a name is already in the chat, there will be no <span class="tex-font-style-tt">'Remove'</span> command if there is no person with such a name in the chat etc.</p><p>All names are case-sensitive.</p></div><div class="output-specification"><p>Print a single number — answer to the problem.</p></div>

## Input

<p>Input file will contain not more than 100 commands, each in its own line. No line will exceed 100 characters. Formats of the commands will be the following:</p><ul> <li> <span class="tex-font-style-tt">+&lt;name&gt;</span> for <span class="tex-font-style-tt">'Add'</span> command. </li><li> <span class="tex-font-style-tt">-&lt;name&gt;</span> for <span class="tex-font-style-tt">'Remove'</span> command. </li><li> <span class="tex-font-style-tt">&lt;sender_name&gt;:&lt;message_text&gt;</span> for <span class="tex-font-style-tt">'Send'</span> command. </li></ul><p><span class="tex-font-style-tt">&lt;name&gt;</span> and <span class="tex-font-style-tt">&lt;sender_name&gt;</span> is a non-empty sequence of Latin letters and digits. <span class="tex-font-style-tt">&lt;message_text&gt;</span> can contain letters, digits and spaces, but can't start or end with a space. <span class="tex-font-style-tt">&lt;message_text&gt;</span> can be an empty line.</p><p>It is guaranteed, that input data are correct, i.e. there will be no <span class="tex-font-style-tt">'Add'</span> command if person with such a name is already in the chat, there will be no <span class="tex-font-style-tt">'Remove'</span> command if there is no person with such a name in the chat etc.</p><p>All names are case-sensitive.</p>

## Output

<p>Print a single number — answer to the problem.</p>





```input1
+Mike
Mike:hello
+Kate
+Dmitry
-Dmitry
Kate:hi
-Kate

```




```input2
+Mike
-Mike
+Mike
Mike:Hi   I am here
-Mike
+Kate
-Kate

```




```output1
9

```




```output2
14

```


