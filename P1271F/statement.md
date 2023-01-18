## Description

<div><p>Recently a lot of students were enrolled in Berland State University. All students were divided into groups according to their education program. Some groups turned out to be too large to attend lessons in the same auditorium, so these groups should be divided into two subgroups. Your task is to help divide the first-year students of the computer science faculty.</p><p>There are $t$ new groups belonging to this faculty. Students have to attend classes on three different subjects — maths, programming and P. E. All classes are held in different places according to the subject — maths classes are held in auditoriums, programming classes are held in computer labs, and P. E. classes are held in gyms.</p><p>Each group should be divided into two subgroups so that there is enough space in every auditorium, lab or gym for all students of the subgroup. For the first subgroup of the $i$-th group, maths classes are held in an auditorium with capacity of $a_{i, 1}$ students; programming classes are held in a lab that accomodates up to $b_{i, 1}$ students; and P. E. classes are held in a gym having enough place for $c_{i, 1}$ students. Analogically, the auditorium, lab and gym for the second subgroup can accept no more than $a_{i, 2}$, $b_{i, 2}$ and $c_{i, 2}$ students, respectively.</p><p>As usual, some students skip some classes. Each student considers some number of subjects (from $0$ to $3$) to be useless — that means, he skips all classes on these subjects (and attends all other classes). This data is given to you as follows — the $i$-th group consists of:</p><ol> <li> $d_{i, 1}$ students which attend all classes; </li><li> $d_{i, 2}$ students which attend all classes, except for P. E.; </li><li> $d_{i, 3}$ students which attend all classes, except for programming; </li><li> $d_{i, 4}$ students which attend only maths classes; </li><li> $d_{i, 5}$ students which attend all classes, except for maths; </li><li> $d_{i, 6}$ students which attend only programming classes; </li><li> $d_{i, 7}$ students which attend only P. E. </li></ol><p>There is one more type of students — those who don't attend any classes at all (but they, obviously, don't need any place in auditoriums, labs or gyms, so the number of those students is insignificant in this problem).</p><p>Your task is to divide each group into two subgroups so that every auditorium (or lab, or gym) assigned to each subgroup has enough place for all students from this subgroup attending the corresponding classes (if it is possible). Each student of the $i$-th group should belong to exactly one subgroup of the $i$-th group; it is forbidden to move students between groups.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 300$) — the number of groups.</p><p>Then the descriptions of groups follow. The description of the $i$-th group consists of three lines:</p><ul> <li> the first line contains three integers $a_{i, 1}$, $b_{i, 1}$ and $c_{i, 1}$ ($1 \le a_{i, 1}, b_{i, 1}, c_{i, 1} \le 3000$) — the capacity of the auditorium, lab and gym assigned to the first subgroup of the $i$-th group, respectively; </li><li> the second line contains three integers $a_{i, 2}$, $b_{i, 2}$ and $c_{i, 2}$ ($1 \le a_{i, 2}, b_{i, 2}, c_{i, 2} \le 3000$) — the capacity of the auditorium, lab and gym assigned to the second subgroup of the $i$-th group, respectively; </li><li> the third line contains integers $d_{i, 1}$, $d_{i, 2}$, ..., $d_{i, 7}$ ($0 \le d_{i, j} \le 3000$) — the number of students belonging to each of the seven aforementioned types in the $i$-th group. <span class="tex-font-style-bf">It is not guaranteed</span> that the sum of these values is positive — a group can consist entirely of students that don't attend classes at all. </li></ul><p>It is guaranteed that the total number of students in all groups is not greater than $3000$.</p></div><div class="output-specification"><p>For each group, print the result of its division as follows:</p><ul> <li> if it is impossible to divide the group, print one integer $-1$; </li><li> otherwise print seven integers $f_{i, 1}$, $f_{i, 2}$, ..., $f_{i, 7}$ ($0 \le f_{i, j} \le d_{i, j}$) — the number of students the first, second, ..., seventh type in the first subgroup of the $i$-th group (all other students will be assigned to the second subgroup). If there are multiple answers, print any of them. </li></ul></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 300$) — the number of groups.</p><p>Then the descriptions of groups follow. The description of the $i$-th group consists of three lines:</p><ul> <li> the first line contains three integers $a_{i, 1}$, $b_{i, 1}$ and $c_{i, 1}$ ($1 \le a_{i, 1}, b_{i, 1}, c_{i, 1} \le 3000$) — the capacity of the auditorium, lab and gym assigned to the first subgroup of the $i$-th group, respectively; </li><li> the second line contains three integers $a_{i, 2}$, $b_{i, 2}$ and $c_{i, 2}$ ($1 \le a_{i, 2}, b_{i, 2}, c_{i, 2} \le 3000$) — the capacity of the auditorium, lab and gym assigned to the second subgroup of the $i$-th group, respectively; </li><li> the third line contains integers $d_{i, 1}$, $d_{i, 2}$, ..., $d_{i, 7}$ ($0 \le d_{i, j} \le 3000$) — the number of students belonging to each of the seven aforementioned types in the $i$-th group. <span class="tex-font-style-bf">It is not guaranteed</span> that the sum of these values is positive — a group can consist entirely of students that don't attend classes at all. </li></ul><p>It is guaranteed that the total number of students in all groups is not greater than $3000$.</p>

## Output

<p>For each group, print the result of its division as follows:</p><ul> <li> if it is impossible to divide the group, print one integer $-1$; </li><li> otherwise print seven integers $f_{i, 1}$, $f_{i, 2}$, ..., $f_{i, 7}$ ($0 \le f_{i, j} \le d_{i, j}$) — the number of students the first, second, ..., seventh type in the first subgroup of the $i$-th group (all other students will be assigned to the second subgroup). If there are multiple answers, print any of them. </li></ul>





```input1
3
9 4 13
1 10 3
1 2 3 4 5 6 7
9 4 13
1 10 3
2 1 3 4 5 6 7
1 2 3
4 5 6
0 0 0 0 0 0 0
```




```output1
1 1 3 4 2 0 7
-1
0 0 0 0 0 0 0
```


