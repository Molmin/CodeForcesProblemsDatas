## Description

<div><p>Vasya has several phone books, in which he recorded the telephone numbers of his friends. Each of his friends can have one or several phone numbers.</p><p>Vasya decided to organize information about the phone numbers of friends. You will be given <span class="tex-span"><i>n</i></span> strings — all entries from Vasya's phone books. Each entry starts with a friend's name. Then follows the number of phone numbers in the current entry, and then the phone numbers themselves. It is possible that several identical phones are recorded in the same record.</p><p>Vasya also believes that if the phone number <span class="tex-span"><i>a</i></span> is a suffix of the phone number <span class="tex-span"><i>b</i></span> (that is, the number <span class="tex-span"><i>b</i></span> ends up with <span class="tex-span"><i>a</i></span>), and both numbers are written by Vasya as the phone numbers of the same person, then <span class="tex-span"><i>a</i></span> is recorded without the city code and it should not be taken into account.</p><p>The task is to print organized information about the phone numbers of Vasya's friends. It is possible that two different people have the same number. If one person has two numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, and <span class="tex-span"><i>x</i></span> is a suffix of <span class="tex-span"><i>y</i></span> (that is, <span class="tex-span"><i>y</i></span> ends in <span class="tex-span"><i>x</i></span>), then you shouldn't print number <span class="tex-span"><i>x</i></span>. If the number of a friend in the Vasya's phone books is recorded several times in the same format, it is necessary to take it into account exactly once.</p><p>Read the examples to understand statement and format of the output better.</p></div><div class="input-specification"><p>First line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 20</span>)&nbsp;— number of entries in Vasya's phone books. </p><p>The following <span class="tex-span"><i>n</i></span> lines are followed by descriptions of the records in the format described in statement. Names of Vasya's friends are non-empty strings whose length does not exceed <span class="tex-span">10</span>. They consists only of lowercase English letters. Number of phone numbers in one entry is not less than <span class="tex-span">1</span> is not more than <span class="tex-span">10</span>. The telephone numbers consist of digits only. If you represent a phone number as a string, then its length will be in range from <span class="tex-span">1</span> to <span class="tex-span">10</span>. Phone numbers can contain leading zeros.</p></div><div class="output-specification"><p>Print out the ordered information about the phone numbers of Vasya's friends. First output <span class="tex-span"><i>m</i></span>&nbsp;— number of friends that are found in Vasya's phone books.</p><p>The following <span class="tex-span"><i>m</i></span> lines must contain entries in the following format "<span class="tex-font-style-tt">name number_of_phone_numbers phone_numbers</span>". Phone numbers should be separated by a space. Each record must contain all the phone numbers of current friend.</p><p>Entries can be displayed in arbitrary order, phone numbers for one record can also be printed in arbitrary order.</p></div>

## Input

<p>First line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 20</span>)&nbsp;— number of entries in Vasya's phone books. </p><p>The following <span class="tex-span"><i>n</i></span> lines are followed by descriptions of the records in the format described in statement. Names of Vasya's friends are non-empty strings whose length does not exceed <span class="tex-span">10</span>. They consists only of lowercase English letters. Number of phone numbers in one entry is not less than <span class="tex-span">1</span> is not more than <span class="tex-span">10</span>. The telephone numbers consist of digits only. If you represent a phone number as a string, then its length will be in range from <span class="tex-span">1</span> to <span class="tex-span">10</span>. Phone numbers can contain leading zeros.</p>

## Output

<p>Print out the ordered information about the phone numbers of Vasya's friends. First output <span class="tex-span"><i>m</i></span>&nbsp;— number of friends that are found in Vasya's phone books.</p><p>The following <span class="tex-span"><i>m</i></span> lines must contain entries in the following format "<span class="tex-font-style-tt">name number_of_phone_numbers phone_numbers</span>". Phone numbers should be separated by a space. Each record must contain all the phone numbers of current friend.</p><p>Entries can be displayed in arbitrary order, phone numbers for one record can also be printed in arbitrary order.</p>





```input1
2
ivan 1 00123
masha 1 00123

```




```input2
3
karl 2 612 12
petr 1 12
katya 1 612

```




```input3
4
ivan 3 123 123 456
ivan 2 456 456
ivan 8 789 3 23 6 56 9 89 2
dasha 2 23 789

```




```output1
2
masha 1 00123 
ivan 1 00123 

```




```output2
3
katya 1 612 
petr 1 12 
karl 1 612 

```




```output3
2
dasha 2 23 789 
ivan 4 789 123 2 456 

```


