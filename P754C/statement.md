## Description

<div><p>Recently Vladik discovered a new entertainment&nbsp;— coding bots for social networks. He would like to use machine learning in his bots so now he want to prepare some learning data for them.</p><p>At first, he need to download <span class="tex-span"><i>t</i></span> chats. Vladik coded a script which should have downloaded the chats, however, something went wrong. In particular, some of the messages have no information of their sender. It is known that if a person sends several messages in a row, they all are merged into a single message. It means that <span class="tex-font-style-bf">there could not be two or more messages in a row with the same sender</span>. Moreover, <span class="tex-font-style-bf">a sender never mention himself in his messages</span>.</p><p>Vladik wants to recover senders of all the messages so that each two neighboring messages will have different senders and no sender will mention himself in his messages.</p><p>He has no idea of how to do this, and asks you for help. Help Vladik to recover senders in each of the chats!</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10</span>) — the number of chats. The <span class="tex-span"><i>t</i></span> chats follow. Each chat is given in the following format.</p><p>The first line of each chat description contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of users in the chat.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated distinct usernames. Each username consists of lowercase and uppercase English letters and digits. The usernames can't start with a digit. Two usernames are different even if they differ only with letters' case. The length of username is positive and doesn't exceed <span class="tex-span">10</span> characters.</p><p>The next line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>)&nbsp;— the number of messages in the chat. The next <span class="tex-span"><i>m</i></span> line contain the messages in the following formats, one per line: </p><ul> <li> <span class="tex-font-style-tt">&lt;username&gt;:&lt;text&gt;</span>&nbsp;— the format of a message with known sender. The username should appear in the list of usernames of the chat. </li><li> <span class="tex-font-style-tt">&lt;?&gt;:&lt;text&gt;</span>&nbsp;— the format of a message with unknown sender. </li></ul><p>The text of a message can consist of lowercase and uppercase English letter, digits, characters <span class="tex-font-style-tt">'.'</span> (dot), <span class="tex-font-style-tt">','</span> (comma), <span class="tex-font-style-tt">'!'</span> (exclamation mark), <span class="tex-font-style-tt">'?'</span> (question mark) and <span class="tex-font-style-tt">' '</span> (space). The text doesn't contain trailing spaces. The length of the text is positive and doesn't exceed <span class="tex-span">100</span> characters.</p><p>We say that a text mention a user if his username appears in the text as a word. In other words, the username appears in a such a position that the two characters before and after its appearance either do not exist or are not English letters or digits. For example, the text "<span class="tex-font-style-tt">Vasya, masha13 and Kate!</span>" can mention users "<span class="tex-font-style-tt">Vasya</span>", "<span class="tex-font-style-tt">masha13</span>", "<span class="tex-font-style-tt">and</span>" and "<span class="tex-font-style-tt">Kate</span>", but not "<span class="tex-font-style-tt">masha</span>".</p><p>It is guaranteed that in each chat <span class="tex-font-style-bf">no known sender mention himself in his messages</span> and there are no two neighboring messages with the same known sender.</p></div><div class="output-specification"><p>Print the information about the <span class="tex-span"><i>t</i></span> chats in the following format:</p><p>If it is not possible to recover senders, print single line "<span class="tex-font-style-tt">Impossible</span>" for this chat. Otherwise print <span class="tex-span"><i>m</i></span> messages in the following format:</p><p><span class="tex-font-style-tt">&lt;username&gt;:&lt;text&gt;</span></p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10</span>) — the number of chats. The <span class="tex-span"><i>t</i></span> chats follow. Each chat is given in the following format.</p><p>The first line of each chat description contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of users in the chat.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated distinct usernames. Each username consists of lowercase and uppercase English letters and digits. The usernames can't start with a digit. Two usernames are different even if they differ only with letters' case. The length of username is positive and doesn't exceed <span class="tex-span">10</span> characters.</p><p>The next line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>)&nbsp;— the number of messages in the chat. The next <span class="tex-span"><i>m</i></span> line contain the messages in the following formats, one per line: </p><ul> <li> <span class="tex-font-style-tt">&lt;username&gt;:&lt;text&gt;</span>&nbsp;— the format of a message with known sender. The username should appear in the list of usernames of the chat. </li><li> <span class="tex-font-style-tt">&lt;?&gt;:&lt;text&gt;</span>&nbsp;— the format of a message with unknown sender. </li></ul><p>The text of a message can consist of lowercase and uppercase English letter, digits, characters <span class="tex-font-style-tt">'.'</span> (dot), <span class="tex-font-style-tt">','</span> (comma), <span class="tex-font-style-tt">'!'</span> (exclamation mark), <span class="tex-font-style-tt">'?'</span> (question mark) and <span class="tex-font-style-tt">' '</span> (space). The text doesn't contain trailing spaces. The length of the text is positive and doesn't exceed <span class="tex-span">100</span> characters.</p><p>We say that a text mention a user if his username appears in the text as a word. In other words, the username appears in a such a position that the two characters before and after its appearance either do not exist or are not English letters or digits. For example, the text "<span class="tex-font-style-tt">Vasya, masha13 and Kate!</span>" can mention users "<span class="tex-font-style-tt">Vasya</span>", "<span class="tex-font-style-tt">masha13</span>", "<span class="tex-font-style-tt">and</span>" and "<span class="tex-font-style-tt">Kate</span>", but not "<span class="tex-font-style-tt">masha</span>".</p><p>It is guaranteed that in each chat <span class="tex-font-style-bf">no known sender mention himself in his messages</span> and there are no two neighboring messages with the same known sender.</p>

## Output

<p>Print the information about the <span class="tex-span"><i>t</i></span> chats in the following format:</p><p>If it is not possible to recover senders, print single line "<span class="tex-font-style-tt">Impossible</span>" for this chat. Otherwise print <span class="tex-span"><i>m</i></span> messages in the following format:</p><p><span class="tex-font-style-tt">&lt;username&gt;:&lt;text&gt;</span></p><p>If there are multiple answers, print any of them.</p>





```input1
1
2
Vladik netman
2
?: Hello, Vladik!
?: Hi

```




```input2
1
2
netman vladik
3
netman:how are you?
?:wrong message
vladik:im fine

```




```input3
2
3
netman vladik Fedosik
2
?: users are netman, vladik, Fedosik
vladik: something wrong with this chat
4
netman tigerrrrr banany2001 klinchuh
4
?: tigerrrrr, banany2001, klinchuh, my favourite team ever, are you ready?
klinchuh: yes, coach!
?: yes, netman
banany2001: yes of course.

```




```output1
netman: Hello, Vladik!
Vladik: Hi

```




```output2
Impossible

```




```output3
Impossible
netman: tigerrrrr, banany2001, klinchuh, my favourite team ever, are you ready?
klinchuh: yes, coach!
tigerrrrr: yes, netman
banany2001: yes of course.

```


