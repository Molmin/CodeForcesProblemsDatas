## Description

<div><p>Vasya is writing an operating system shell, and it should have commands for working with directories. To begin with, he decided to go with just two commands: <span class="tex-font-style-tt">cd</span> (change the current directory) and <span class="tex-font-style-tt">pwd</span> (display the current directory).</p><p>Directories in Vasya's operating system form a traditional hierarchical tree structure. There is a single root directory, denoted by the slash character "<span class="tex-font-style-tt">/</span>". Every other directory has a name — a non-empty string consisting of lowercase Latin letters. Each directory (except for the root) has a parent directory — the one that contains the given directory. It is denoted as "<span class="tex-font-style-tt">..</span>".</p><p>The command <span class="tex-font-style-tt">cd</span> takes a single parameter, which is a path in the file system. The command changes the current directory to the directory specified by the path. The path consists of the names of directories separated by slashes. The name of the directory can be "<span class="tex-font-style-tt">..</span>", which means a step up to the parent directory. «<span class="tex-font-style-tt">..</span>» can be used in any place of the path, maybe several times. If the path begins with a slash, it is considered to be an absolute path, that is, the directory changes to the specified one, starting from the root. If the parameter begins with a directory name (or "<span class="tex-font-style-tt">..</span>"), it is considered to be a relative path, that is, the directory changes to the specified directory, starting from the current one.</p><p>The command <span class="tex-font-style-tt">pwd</span> should display the absolute path to the current directory. This path must not contain "<span class="tex-font-style-tt">..</span>".</p><p>Initially, the current directory is the root. All directories mentioned explicitly or passed indirectly within any command <span class="tex-font-style-tt">cd</span> are considered to exist. It is guaranteed that there is no attempt of transition to the parent directory of the root directory.</p></div><div class="input-specification"><p>The first line of the input data contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of commands.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each contains one command. Each of these lines contains either command <span class="tex-font-style-tt">pwd</span>, or command <span class="tex-font-style-tt">cd</span>, followed by a space-separated non-empty parameter.</p><p>The command parameter <span class="tex-font-style-tt">cd</span> only contains lower case Latin letters, slashes and dots, two slashes cannot go consecutively, dots occur only as the name of a parent pseudo-directory. The command parameter <span class="tex-font-style-tt">cd</span> does not end with a slash, except when it is the only symbol that points to the root directory. The command parameter has a length from 1 to 200 characters, inclusive.</p><p>Directories in the file system can have the same names.</p></div><div class="output-specification"><p>For each command <span class="tex-font-style-tt">pwd</span> you should print the full absolute path of the given directory, ending with a slash. It should start with a slash and contain the list of slash-separated directories in the order of being nested from the root to the current folder. It should contain no dots.</p></div>

## Input

<p>The first line of the input data contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of commands.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each contains one command. Each of these lines contains either command <span class="tex-font-style-tt">pwd</span>, or command <span class="tex-font-style-tt">cd</span>, followed by a space-separated non-empty parameter.</p><p>The command parameter <span class="tex-font-style-tt">cd</span> only contains lower case Latin letters, slashes and dots, two slashes cannot go consecutively, dots occur only as the name of a parent pseudo-directory. The command parameter <span class="tex-font-style-tt">cd</span> does not end with a slash, except when it is the only symbol that points to the root directory. The command parameter has a length from 1 to 200 characters, inclusive.</p><p>Directories in the file system can have the same names.</p>

## Output

<p>For each command <span class="tex-font-style-tt">pwd</span> you should print the full absolute path of the given directory, ending with a slash. It should start with a slash and contain the list of slash-separated directories in the order of being nested from the root to the current folder. It should contain no dots.</p>





```input1
7
pwd
cd /home/vasya
pwd
cd ..
pwd
cd vasya/../petya
pwd

```




```input2
4
cd /a/b
pwd
cd ../a/b
pwd

```




```output1
/
/home/vasya/
/home/
/home/petya/

```




```output2
/a/b/
/a/a/b/

```


