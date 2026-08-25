## Course Webpage for Compilers (P423, P523, E313, and E513)

Indiana University, Fall 2026


High-level programming languages like Racket and Python make it easier
to program compared to low-level languages such as x86 assembly
code. But how do high-level languages work? There's a big gap between
them and machine instructions for modern computers. In this class you
learn how to translate Racket or Python programs (your choice!) all
the way to x86 assembly language.

Traditionally, compiler courses teach one phase of the compiler at a
time, such as parsing, semantic analysis, and register allocation. The
problem with that approach is it is difficult to understand how the
whole compiler fits together and why each phase is designed the way it
is. Instead, each week we implement a progressively larger subset of
the input language. The very first subset is a tiny language of
integer arithmetic, and by the time we are done the language includes
first-class functions.

**Prerequisites:** Fluency in Racket or Python is highly recommended
as students will do a lot of programming in one of those
languages. Prior knowledge of an assembly language helps, but is not
required.

**Textbook: Essentials of Compilation: An Incremental Approach in Racket/Python** 

* The Racket version of the textbook for the course is available at
  the IU bookstore and from many book sellers, links to those
  [here](https://mitpress.mit.edu/9780262047760/essentials-of-compilation/).
  The PDF is also available for free
  [here](https://www.dropbox.com/s/ktdw8j0adcc44r0/book.pdf?dl=1).
  
* The Python version of the textbook for the course is available
  at the IU bookstore and from many book sellers, links to those
  [here](https://mitpress.mit.edu/9780262048248/essentials-of-compilation/).
  The PDF is also available for free
  [here](https://www.dropbox.com/s/mfxtojk4yif3toj/python-book.pdf?dl=1).

If you have suggestions for improvement, please either send an email
to Jeremy or, even better, make edits to a branch of the book and
perform a pull request. The book is at the following location on
github:

    https://github.com/IUCompilerCourse/Essentials-of-Compilation

**Lecture:** Tuesdays and Thursdays 2:20-3:35pm, Informatics Building
  (Myles Brand Hall), Room I 107.

**Office Hours**

* Jeremy Siek (jsiek): Luddy 3016 or 3014, Tuesdays 10am-11am, Thursdays 1-2pm
* Emeka Nkurumeh (emnkuru): TBD


**Topics:**

* Instruction Selection

* Register Allocation

* Static type checking

* Conditional control flow

* Mutable data

* Garbage collection

* Procedures and calling conventions

* First-class functions and closure conversion

* Dynamic typing

* Generics

**Grading:**

Course grades are based on the following items. For the weighting, see
the Canvas panel on the right-hand side of this web page.  Grading
will take into account any technology problems that arrise, i.e., you
won't fail the class because your internet went out.

* Assignments (40%)
* Midterm Exam (25%)
* Final Exam (35%)

**Assignments:**

Organize into teams of 2-4 students. Assignments will be due bi-weekly
on Mondays at 11:59pm. Teams that include one or more graduate
students are required to complete one challenge exercise per
assignment.

Assignment descriptions are posted on Canvas.  Turn in your
assignments by submitting your code to the autograder.  There is a
Racket and Python version of each assignment.  Submit your `compiler`
file, either `compiler.rkt` or `compiler.py` depending on the language
you are using.

Assignments will be graded based on how many test cases they succeed
on. Partial credit will be given for each "pass" of the compiler.
Some of the tests are in the public support code (see Resources
below). The testing will be done on a linux (ubuntu) machine. The
testing will include both new tests and all of the tests from prior
assignments.

You may request feedback on your assignments prior to the due date.
Just submit your work to the autograder and send us email.

Students are responsible for understanding the entire assignment and
all of the code that their team produces. The midterm and final exam
are designed to test a student's understanding of the assignments.

Students are free to discuss and get help on the assignments from
anyone or anywhere. When posting questions on Slack, it is OK to post
your code.

In contrast, for quizzes and exams, students are asked to work
alone. The quizzes and exams are closed book.


**Late Assignment Policy:** Assignments may be turned in up to one
week late with a penalty of 10%.


**Slack Chat/Messaging:**


  [Workspace](https://compilers-fall-2026.slack.com) 
    ([signup](https://join.slack.com/t/compilers-fall-2026/shared_invite/zt-47ufrjybp-zLsGdTRp0EvwrUN9jPEwrQ)
  using your iu email address).

**Schedule**

Day     | Lecture Topic              | Assignment Due
--------|----------------------------|----------------
Aug. 25 | [Introduction](https://docs.google.com/presentation/d/13jmEAwqD7naNAj0c2IsF0tDhgMyQH-tBW9sZeRgzBt8/edit?usp=sharing)               |
Aug. 27 | [From Lvar to x86](https://docs.google.com/presentation/d/1KUlWTAvdcKtZNOST9ITpmiOe34lD2DFsycH5oT2oMuU/edit?usp=sharing) |
Sep. 1  | Example Compilation from Lvar to x86 in [Racket](./example-var-73.md) and [Python](./python-var-73.md) |
Sep. 3 | [Register Allocation, Introduction and Liveness](https://docs.google.com/presentation/d/1jL4M6G6DDnfqOPsCab9_6k7PcV_wRBd4p9Xn2LzobOE/edit?usp=sharing) |
Sep. 8 | [Register Allocation: graph coloring](https://docs.google.com/presentation/d/1qPKUGZnqh6ggfP5_emHVJhSTyPRI0iD02jRTdB9mbwo/edit?usp=sharing) | Integers and Variables due, submit in [Racket](https://autograder.luddy.indiana.edu/web/project/2518) or [Python](https://autograder.luddy.indiana.edu/web/project/2517) (see also, [Racket challenge](https://autograder.luddy.indiana.edu/web/project/2528) or [Python challenge](https://autograder.luddy.indiana.edu/web/project/2523))

<!-- 
Sep. 10 | Code Review: Integers and Variables
Sep. 15 | [L_If language, type checking, and x86_If](https://docs.google.com/presentation/d/1ZJWJN8mAPS3NpTBkbkY8xauZtIGbZdCwTovtN1a4gUo/edit?usp=sharing) | Integers and Variables, late deadline
Sep. 17 | [Conditionals and Explicate Control](https://docs.google.com/presentation/d/1OALjNzmyLNt_Yg3eV_xjLx7ZxQ_8q2fLLi0I9nJjX9I/edit?usp=sharing),  [Conditionals: Select Instr., Reg. Alloc., Opt. Jumps](https://docs.google.com/presentation/d/1Zcq1OpvmiMcHDkSZ0qjF2mdYNaov0t5R4qF0h66ryV8/edit?usp=sharing)
Sep. 22 | [Loops and Dataflow Analysis](https://docs.google.com/presentation/d/1RPT6wjE_MhMDPMet0nee5dv7WzaHD52shwSpUE84edM/edit?usp=sharing) | Register Allocation, submit in [Racket](https://autograder.luddy.indiana.edu/web/project/1915) or [Python](https://autograder.luddy.indiana.edu/web/project/1914) (see also, [Racket challenge](https://autograder.luddy.indiana.edu/web/project/2023) or [Python challenge](https://autograder.luddy.indiana.edu/web/project/2022))
Sep. 24 | Code Review: Register Allocation
Sep. 29 | [Loops: RCO, Explicate, Challenge](https://docs.google.com/presentation/d/18cN5P4pEuDds5U40Hqa6WDP-LdoyYBg2RCRML37QL5k/edit?usp=sharing) | Register Allocation, late deadline
Oct. 1  | [Tuples and Garbage Collection](https://docs.google.com/presentation/d/1LTyqurU5c1MfzBJAjuuLJKZYAYqyjLggaZn-MIV4ocg/edit?usp=sharing)
Oct. 6 | [Static Single Assignment](https://docs.google.com/presentation/d/1z7D52QoJ35say9kY8VuuZWlY3yZu5HxwVv_gLcdk_Jw/edit?usp=sharing) | Booleans and Conditionals, submit in [Racket](https://autograder.luddy.indiana.edu/web/project/1908) or [Python](https://autograder.luddy.indiana.edu/web/project/1907) (see also, [Racket challenge](https://autograder.luddy.indiana.edu/web/project/2048) or [Python challenge](https://autograder.luddy.indiana.edu/web/project/2047))
Oct. 8 | Code Review: Conditionals
Oct. 13 | [Tuples and GC, cont'd](https://docs.google.com/presentation/d/1SYAsDrtEP0aY9R18oibuZvJkhVzeHlfthjR1_Kii6nM/edit?usp=sharing) | Booleans and Conditionals, late deadline
Oct. 15 | [Arrays, Structs, Generational GC](https://docs.google.com/presentation/d/1GHF-JTvsnJeOSBhAn9m1HHFVpRekVPO0QHSbkbg4vX8/edit?usp=sharing)
Oct. 20 | Review for Midterm Exam | Loops, submit in [Racket](https://autograder.luddy.indiana.edu/web/project/1916) or [Python](https://autograder.luddy.indiana.edu/web/project/1904) (see also [Racket challenge](https://autograder.luddy.indiana.edu/web/project/2054) or [Python challenge](https://autograder.luddy.indiana.edu/web/project/2055))
Oct. 22 | **Midterm Exam** in class
Oct. 27 | [Compiling Functions to x86](https://docs.google.com/presentation/d/12AD6drC7k9_7Ldk8yN8HWI6MBmzqfM5ec0pSP9pj_po/edit?usp=sharing) | Loops, late deadline 
Oct. 29 | Code Review: Loops
Nov. 3  | Compiling Functions, cont'd | Tuples, submit in [Racket](https://autograder.luddy.indiana.edu/web/project/1909) or [Python](https://autograder.luddy.indiana.edu/web/project/1906) (see also [Racket challenge](https://autograder.luddy.indiana.edu/web/project/2080) or [Python challenge](https://autograder.luddy.indiana.edu/web/project/2079))
Nov. 5  | [Lexically Scoped Functions](https://docs.google.com/presentation/d/1C33rWgJFXUv4tvhEnxzNhsJCc0L6t1BMWDaswuCL47w/edit?usp=sharing)
Nov. 10 | [Dynamic Typing](https://docs.google.com/presentation/d/1vhGJ54-ZBcW7GsS2nLhaqkAkFRDGdMRGk-Onv_jQYmI/edit?usp=sharing) | Tuples, late deadline
Nov. 12 | Code Review: Tuples
Nov. 17 | [Gradual Typing](https://docs.google.com/presentation/d/17AfL6HTSGPdiLxGOs_wSRc0i5xoLF1QYPL-A7i1U_Ag/edit?usp=sharing) | Functions, submit in [Racket](https://autograder.luddy.indiana.edu/web/project/1910) or [Python](https://autograder.luddy.indiana.edu/web/project/1905)
Nov. 19 | [Generics](https://docs.google.com/presentation/d/1772Bs1E1XPF2duXquzGMEcjFt_a5Ssa0DgcureURfgI/edit?usp=sharing)
Nov. 20 | | [Proposal for Final Project](./final-project-proposal.md)
Nov. 23 - Nov. 27 | **Thanksgiving Break**
Dec. 1 | [Objects](https://docs.google.com/presentation/d/1quAiJTiIoYNlgJka8nLl3GchhDPQdoXLK6kcEzEDGVo/edit?usp=sharing) | Functions, late deadline
Dec. 3 | Procedure Inlining
Dec. 8 | Code Review: Functions
Dec. 10 | Review for Final Exam
Dec. 12 | | Final Project (no late submissions). See the canvas assignment for details.
Dec. 15 | **Final Exam** 12:40-2:40 pm -->



**Resources:**

* Practice exams:
  - Midterm from 2023: [Python with solutions](./2023-python-midterm-soln.pdf), [Racket with solutions](./2023-racket-midterm-soln.pdf)
  - Midterm from 2022: [Python](./2022-python-midterm.pdf), [Python with solutions](./2022-python-midterm-soln.pdf), [Racket](./2022-racket-midterm.pdf), [Racket with solutions](./2022-racket-midterm-soln.pdf)
  - Final from 2022: [Python](./2022-python-final.pdf), [Python with solutions](./2022-python-final-soln.pdf), [Racket](./2022-racket-final.pdf), [Racket with solutions](./2022-racket-final-soln.pdf)
  - Final from 2021: [Python](./2021-python-final.pdf), [Python with solutions](./2021-python-final-soln.pdf), [Racket](./2021-racket-final.pdf), [Racket with solutions](./2021-racket-final-soln.pdf)
  
* Lecture videos recorded from the [2020 course](https://iucompilercourse.github.io/IU-P423-P523-E313-E513-Fall-2020/).
* Github repository for the support code and test suites
    - for [Racket](https://github.com/IUCompilerCourse/public-student-support-code) 
	- for [Python](https://github.com/IUCompilerCourse/python-student-support-code)
* [Racket Download](https://download.racket-lang.org/)
* [Racket Documentation](https://docs.racket-lang.org/)
* [Python Download](https://www.python.org/downloads/)
* [Python Documentation](https://docs.python.org/)
* [Python ast module declarations](https://github.com/python/typeshed/blob/master/stdlib/_ast.pyi)
* [Notes on x86-64 programming](http://web.cecs.pdx.edu/~apt/cs491/x86-64.pdf)
* [x86-64 Machine-Level Programming](https://www.cs.cmu.edu/~fp/courses/15411-f13/misc/asm64-handout.pdf)
* [Intel x86 Manual](http://www.intel.com/content/dam/www/public/us/en/documents/manuals/64-ia-32-architectures-software-developer-manual-325462.pdf?_ga=1.200286509.2020252148.1452195021)
* [System V Application Binary Interface](https://software.intel.com/sites/default/files/article/402129/mpx-linux64-abi.pdf)
* [Uniprocessor Garbage Collection Techniques](https://iu.instructure.com/courses/1735985/files/82131907/download?wrap=1) by Wilson. 
* [Fast and Effective Procedure Inlining](https://www.cs.indiana.edu/~dyb/pubs/inlining.pdf) by Waddell and Dybvig.



