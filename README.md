# Advanced data science and programming course

## General information

Semmelweis University - 2021 spring course on data science, programming,
advanced data analysis, including sequencing data analysis, using command line
tools, R and Python with lecture outlines, recommended reading material and
other information.

The course builds heavily on the [Carpentries
Foundation](https://carpentries.org) material and teaching philosophy. This
version is intended for people with already some experience using R and Python
to do basic data analysis and visualization.

**Location**: Histology Seminar Room (ground floor), Semmelweis University,
1<sup>st</sup> Department of Pathology and Experimental Cancer Research, H-1085
Budapest, Üllői út 26. The IRL class might or might not happen, depending on the
pandemic.

**Network**: Use the `HISTOLOGY-1` or `HISTOLOGY-2` wireless networks, and ask
the teachers for password.

**Time**: every Wednesday, from 16:30 to 18:00, starting with the 3<sup>rd</sup>
of February for 14 weeks.

**Requirements**: participants must bring a laptop with a Mac, Linux, or Windows
operating system (not a tablet, Chromebook, etc.) that they have administrative
privileges on. They are also required to abide by the [Carpentries Code of
Conduct](https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html).

**Grading and homeworks**: there are going to be 12 short homework exercises (no
homework for Week 1 and Week 14), where you will be asked to think about a
problem, try to solve it, and most importantly, document your thoughts, the
issues or problems you ran into. You will need to submit one or a few small text
files, tables, documents, or scripts through Dropbox File Requests. We are going
to discuss solutions and issues next week. You will need to submit at least 6 of
them to pass, and 10 for excellent. Keep in mind that you are here to learn and
try things out. Active participation, discussing issues and asking questions is
much more important, than submitting perfectly written programming exercises.

**Contact**: send an email to sebestyen.endre at med dot semmelweis-univ dot hu
if you have any questions or comments.

**Teachers**: Endre Sebestyén, Bence Szalai, Gábor Turu, Miklós Cserző

**Online setup**: The course will be shared on [Zoom](https://zoom.us/), and the
classes will be recorded. This way, you can join and follow the material even if
you are abroad, in quarantine, have another class at the same time, etc.

If you haven't used Zoom before, go to the official website to download and
install the Zoom client for your computer.

Like other Carpentries workshops, you will be learning by "coding along" with
the teachers. To do this, you will need to have both the window for the tool you
will be learning about (a terminal, RStudio, your web browser, etc..) and the
window for the Zoom video conference client open. In order to see both at once,
we recommend using one of the following set up options:

- **Two monitors**: If you have two monitors, plan to have your terminal or
  RStudio up on one monitor and the video conferencing software on the other.

- **Two devices**: If you don't have two monitors, do you have another device
  (tablet, smartphone) with a medium to large sized screen? If so, try using the
  smaller device as your video conference connection and your larger device
  (laptop or desktop) to follow along with code examples and instructions.

- **Divide your screen**: If you only have one device and one screen, practice
  having two windows (the video conference program and one of the tools you will
  be using at the workshop) open together. How can you best fit both on your
  screen? Will it work better for you to toggle between them using a keyboard
  shortcut? Try it out in advance to decide what will work best for you.

The course will be recorded on Zoom automatically. Ask the teachers for a link,
if you missed class, or want to check the examples, explanations, etc again.

This [blog post](https://carpentries.org/blog/2020/06/online-workshop-logistics-and_screen-layouts/)
includes detailed information on how to set up your screen to follow along
during the course.

[Semmelweis PhD School Course Database](http://old.semmelweis.hu/wp-content/phd/phd_live/)

## Schedule

|Week |Date      |Instructor     |
|-----|----------|---------------|
|1.   |2021-02-03|Endre Sebestyén|
|2.   |2021-02-10|Endre Sebestyén|
|3.   |2021-02-17|Endre Sebestyén|
|4.   |2021-02-24|Endre Sebestyén|
|5.   |2021-03-03|Gábor Turu     |
|6.   |2021-03-10|Gábor Turu     |
|7.   |2021-03-17|Bence Szalai   |
|8.   |2021-03-24|Bence Szalai   |
|9.   |2021-03-31|Gábor Turu     |
|10.  |2021-04-07|Gábor Turu     |
|11.  |2021-04-14|Miklós Cserző  |
|12.  |2021-04-21|Miklós Cserző  |
|13.  |2021-04-28|Gábor Turu     |
|14.  |2021-05-05|Bence Szalai   |

## Week 1 - 2021-02-03

*Introduction, software setup, basics of command-line.*

Delivery plan:

- Explain content of course
- Explain [Code of Conduct](https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html)
- Homeworks and grading
- Short introduction from everybody
- Getting started with the iPython terminal

During this lesson we will do some introduction, setup and then learn about the
Unix shell. We will discuss how to work in a shell, why is it useful and learn
some basic commands.

### Server setup and VPN

An iPython browser-based terminal, is accessible
[here](https://10.114.112.81:4040). This address can be only seen from inside
the Semmelweis University network and/or by setting up VPN.

More details on how to setup the VPN connection:

- [Part 1](https://lib.semmelweis.hu/se_kk_vpn/info)
- [Part 2](https://lib.semmelweis.hu/index.php?app=content&id=128)
- [Part 3](https://semmelweis.hu/informatika/egyeb-szolgaltatasok/eroforrasok-tavoli-elerese/)
- [Part 4](http://openvpnigenylo.semmelweis.hu/login)

There are different versions available, for students with a NEPTUN code (PPTP or
L2TP), for employees of the university with a SEKA id (L2TP) or by applying for
an OpenVPN login and specifying the server IPs and protocols you want to access.

After connecting to the server, and opening an iPython terminal, the very first
command that you type in, should be `bash -l`.

### Local setup without VPN

If you can't connect to the server above, you can do the exercises locally, on
your laptop. Please follow the setup instructions
[here](http://swcarpentry.github.io/shell-novice/setup.html).

### Lesson material

We will use the Software Carpentry lesson titled [The Unix
Shell](http://swcarpentry.github.io/shell-novice/).

- [Introducing the Shell](http://swcarpentry.github.io/shell-novice/01-intro/index.html)
- [Navigating Files and Directories](http://swcarpentry.github.io/shell-novice/02-filedir/index.html)

### Recommended readings

- [Linux Command Line Cheat Sheet](https://cheatography.com/davechild/cheat-sheets/linux-command-line/)
- [GNU Manuals Online](http://www.gnu.org/manual/manual.html)
- [GNU Manuals Online - coreutils](http://www.gnu.org/software/coreutils/manual/html_node/index.html)
- The Unix shell at [Wikipedia](https://en.wikipedia.org/wiki/Unix_shell)
- [Git BASH](https://gitforwindows.org), a lightweight, native set of tools for
  Windows to provide command-line emulation and other things

## Week 2 - 2021-02-10

*Working with files and directories, pipes, filters*

Delivery plan:

- Short recap of previous lesson
- Creating, moving, deleting files and directories
- Command output redirection, intro to pipes

### Lesson material

We will continue with the Software Carpentry lesson titled [The Unix
Shell](http://swcarpentry.github.io/shell-novice/).

- [Working With Files and
  Directories](http://swcarpentry.github.io/shell-novice/03-create/index.html)
- [Pipes and Filters](http://swcarpentry.github.io/shell-novice/04-pipefilter/index.html)

### Recommended readings

- [Introduction to the Command Line for
  Genomics](https://datacarpentry.org/shell-genomics/). This material uses an
  Amazon virtual machine, and you can't practice directly on one, but might
  contain useful info.

### Homework

Submit homework using the Dropbox File Request link. We will discuss the
homework next week. There is no strict deadline, but please send the files at
least a day in advance before the next lesson, so we can check, and give some
feedback if needed.

Using the commands we discussed until now, create a directory structure and a
few example files for a new project that you think would be useful. Use `nano` to
record all commands in a txt file, and send the file. Use `ls`, `cd`, `mkdir`,
`cp`, `mv`, `touch`, `pwd`, `rm` in any combination you need (you might not need
all of them).

## Week 3 - 2021-02-17

*Pipes, filters and loops*

Delivery plan:

- Homework discussion
- Short recap of previous lesson
- Building more complex pipes
- Loops for repeating commands

### Lesson material

We will continue with the Software Carpentry lesson titled [The Unix
Shell](http://swcarpentry.github.io/shell-novice/).

- [Pipes and Filters](http://swcarpentry.github.io/shell-novice/04-pipefilter/index.html)
- [Loops](http://swcarpentry.github.io/shell-novice/05-loop/index.html)

### Recommended readings

- There is more to life than for loops. We have `while` and `until` loops too.
  Check [here](https://tldp.org/HOWTO/Bash-Prog-Intro-HOWTO-7.html) or
  [here](https://ryanstutorials.net/bash-scripting-tutorial/bash-loops.php).
- [How to name files](https://speakerdeck.com/jennybc/how-to-name-files) by
  Jenny Bryan.

### Homework

Submit homework using the Dropbox File Request link. We will discuss the
homework next week. There is no strict deadline, but please send the files at
least a day in advance before the next lesson, so we can check, and give some
feedback if needed.

Download the `surveys.csv` file from
[here](https://ndownloader.figshare.com/files/10717177). Check the content of
the file, and record a few statistics using command line tools.

- The total number of observations in the file
- The total number of different species ids in descending order
- The total number of different sexes

Write down *both the commands used and the results* in a file, and check for any
irregularities or problems. Use the `cut`, `sort`, `uniq`, `wc` commands,
redirection with `>` or `>>`, `nano` or anything else we learned.

## Week 4 - 2021-02-24

*Finding things and shell scripting*

Delivery plan:

- Homework discussion
- Short recap of previous lesson
- Finding things with grep and find
- Writing shell scripts

### Lesson material

We will continue with the Software Carpentry lesson titled [The Unix
Shell](http://swcarpentry.github.io/shell-novice/).

- [Finding Things](http://swcarpentry.github.io/shell-novice/07-find/index.html)
- [Shell Scripts](http://swcarpentry.github.io/shell-novice/06-script/index.html)

### Recommended readings

More on regular expressions.

- Bash Guide for Beginners: [Regular expressions](https://tldp.org/LDP/Bash-Beginners-Guide/html/chap_04.html)
- Advanced Bash-Scripting Guide: [Regular Expressions](https://tldp.org/LDP/abs/html/regexp.htmla)
- [File Permissions](https://linuxize.com/post/chmod-command-in-linux/)

### Homework

Submit homework using the Dropbox File Request link. We will discuss the
homework next week. There is no strict deadline, but please send the files at
least a day in advance before the next lesson, so we can check, and give some
feedback if needed.

Update your script from previous week, so it runs as a proper shell script, with
the starting "magical" line, proper documentation, comments included, and using
the `$1` variable for defining the input file.

## Week 5 - 2021-03-03

*The programmer's toolkit*

Planned topics:

- Linux, git, github, virtual environment, containerization, remote control, command line tools

### Homework (optional)

Create a project/git repository and share it on github

## Week 6 - 2021-03-10
You can find the data, and also the Colab Notebook here:
[Data](https://drive.google.com/drive/folders/1rWRpqM6qxuW46F7NPpZEZ05k4_Ojcvs4?usp=sharing)
####Homework: 

* Calculate coefficients (for SARS-CoV-2 treatment) for Calu-3 and A549 cells, and plot them (scatter plot) against each other. This will show us how similar are the response of these cells to infection. You will have to filter for these data (have 2 DataFrames, containing Mock and SARS-CoV-2 infected samples, and either Calu-3 or A549 cell lines), and run a statistical model with only 'Treatment' factor (basically it is a t-test).
* Please upload this notbook (your_name.ipynb) to the Week6 folder (you should have write access to this, if not please let me know)
* install [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) library in R.

Please upload you homework here:
[Homework](https://drive.google.com/drive/folders/1Z5EjvGLvyIrRlxOuw9wISQ2DtgnZ6JQU?usp=sharing)

## Week 7 - 2021-03-17

## Week 8 - 2021-03-24

## Week 9 - 2021-03-31

*Starting a deployement project*

We will start to create a web app to share some data on the web. We will practice the followings:
- creation of a remote linux server
- connection to the server through ssh
- installing docker 
- creation of a remote development environment using a docker container
- creation of a github repository for the project

Useful links, tutorials, not all of these information will be covered in our course:
  - docker: https://www.youtube.com/watch?v=pTFZFxd4hOI
  - ml-workspace: https://github.com/ml-tooling/ml-workspace
  - git: 
      - https://www.youtube.com/watch?v=uR6G2v_WsRA
      - https://www.youtube.com/watch?v=HVsySz-h9r4
      - https://www.youtube.com/watch?v=FdZecVxzJbk

## Week 10 - 2021-04-07
  *Continuing the deployement project*

Planned:
- creation of the project on the remote server
- playing with the plotly library
- streamlit library
- playing a little bit with git
- structuring the project folder

## Week 11 - 2021-04-14

## Week 12 - 2021-04-21

## Week 13 - 2021-04-28

## Week 14 - 2021-05-05
