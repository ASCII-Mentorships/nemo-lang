=======================================
Nemo: A Functional Programming Language
=======================================
.. code:: haskell
	
	-- Hello, World!
	main = printLn "Hello, World!"

Project Idea 
------------
The goal is to develop an efficient compiler/interpreter for a `functional programming language <https://en.wikipedia.org/wiki/Functional_programming>`_ in a similiar vein to the very popular programming language `Haskell <https://www.haskell.org/>`_. Functional programming languages are very important when approaching computer science theory and structures found in computer science theory. In fact some functional programming languages like `Coq <https://coq.inria.fr/>`_ and `Lean <https://leanprover.github.io/>`_ allow us to **prove** mathematical results. While this project isn't aiming to be a proof assistant, just implementing a basic functional programming langauge comes with its own set of issues and research problems. So while we develop this functional programming we will also pick up and apart many of the theoretical topics that underpin functional programming languages and **much** of computer science too (like `Lambda Calculus <https://en.wikipedia.org/wiki/Lambda_calculus>`_!).

Project Pipeline
----------------
People familiar with programming languages would realise that the language will start with a `lexer <https://en.wikipedia.org/wiki/Lexical_analysis>`_ and a `parser <https://en.wikipedia.org/wiki/Parsing>`_. This tools will convert human-readable source code into computer-modifiable data structures. Just like Haskell, we will be implementing an intermediate and much simple **Core** language, which would be very similiar in structure to another functional programming language called `Lisp <https://en.wikipedia.org/wiki/Lisp_(programming_language)>`_. The front end **Nemo** language will be then `desugared <https://en.wikipedia.org/wiki/Syntactic_sugar>`_ into the **Core** language. We will then *either/both* interpret the **Core** language, *or/and* compile it into some machine readable/portable format (like assembly or C). Optimizations will occur throughout the pipeline.

Tentative Timeline
------------------
We will put most of our initial effort into perfecting the **Core** language. Once we have a stable version of the **Core** language, along with a suitable backend, we will begin work on the frontend **Nemo** language. Work on optimizing the pipeline will be perpetual. Which gives us the initial timeline:

First semester
	Finish work on a basic form of the **Core** language.

Second Semester
	Start the **Nemo** frontend to make the language usable.

Prerequisites
-------------
1. C programming language: Especially pointers!
2. C++ programming: How to `overload operators <https://en.cppreference.com/w/cpp/language/operators>`_, basic containers in the `STL <https://en.cppreference.com/w/cpp>`_, and you will have to forget some OOP concepts like inheritance.
3. Basics of functional programming: Download `Haskell <https://www.haskell.org/>`_ and give it a whirl! You should atleast *know* the paradigm you are *implementing*!
4. Basic computer science theory: Just give the `Wikipedia page on Lambda Calculus <https://en.wikipedia.org/wiki/Lambda_calculus>`_ and see if it interests you!
5. Good programming practices: Documenting your code, uniform formatting, good identifier names etc..
6. Interest in the project! 

End Result
----------
A working functional programming language that you made, which would run code like this!

.. code:: haskell
	
	fac :: (Integral a) => a -> a
	fac 0 = 1
	fac n = n * fac (n - 1)

	main = printIntLn $ fac 100
	-- Yay!

Work that has already been done
-------------------------------
TODO

Expectations
------------
TODO

Project Mentors
---------------
- `Bhargav Kulkarni <https://github.com/wags-1314>`_
- `Akhilesh Adithya <https://github.com/AkhileshAdithya>`_
- `Aaranya Prasad <https://github.com/yrzaa>`_
- `Rajath V <https://github.com/Rajath-55>`_
- `Vishal Sharma <https://github.com/V1shal1800>`_
- `Pranav KD <https://github.com/Pranav-KD>`_
- `Nimish Wadekar <https://github.com/nimishwadekar>`_
- `Sarthak Chaudhary <https://github.com/Qarthak>`_
