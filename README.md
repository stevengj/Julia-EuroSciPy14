# Julia at EuroSciPy 2014

These are the slides and IJulia notebooks from [a
talk](https://www.euroscipy.org/2014/schedule/presentation/53/) by
Steven G. Johnson at [EuroSciPy 2014](https://www.euroscipy.org/2014):

## Keynote: Crossing Language Barriers with Julia, Scipy, and IPython

<blockquote>
Julia ([julialang.org](http://julialang.org/)) is a new language
targeted at scientific computing, which combines the high-level
abstractions and dynamic interactivity of languages like Python with
the performance of low-level languages like C, thanks to being
designed from the beginning for efficient just-in-time compilation by
LLVM. But a major challenge for any young programming language is the
availability of a large ecosystem of mature libraries and tools. To
overcome this difficulty, Julia is "bootstrapping" off of the Python
ecosystem, both by making it easy to call Python code and also by
exploiting infrastructure such as
[IPython](http://ipython.org/)/[Jupyter](http://jupyter.org/).

This talk will begin with an introduction to the Julia language, both
explaining why it is able to attain C-like performance in many
cases. At the same time, Julia supports a number of unusual
programming features, such as multiple dispatch (a kind of
generalization of object-oriented programming) and metaprogramming. We
will also describe how Julia connects with Python via the
[PyCall](gj/PyCall.jl) package, which enables straightforward,
low-overhead calls to Python libraries, copy-free sharing of NumPy
arrays and other large data structures, and even sharing higher-order
callback functions. This gives Julia direct access to SciPy and
numerous other Python packages, such as
[SymPy](https://github.com/jverzani/SymPy.jl) and
[Matplotlib](https://github.com/stevengj/PyPlot.jl). Another key
component of the Python universe is IPython, and we will explain how
connecting to the IPython "Jupyter" front-end from an
[IJulia](https://github.com/JuliaLang/IJulia.jl) back-end allows Julia
to benefit from IPython's rich multimedia notebook interface, and how
Julia can even use IPython 2's [interactive-widget
infrastructure](https://github.com/JuliaLang/Interact.jl) to provide
truly interactive computations.

Although most Julia–Python interaction is from Julia users calling
Python, there is potential for benefits to flow in both directions in
the future. The same PyCall software that allows Julia code to call
Python can also [allow Python code to call
Julia](https://github.com/JuliaLang/pyjulia), with the same
data-sharing and rich interactivity. And Julia code can also be
compiled to C-compatible interfaces—currently, this is mainly used to
pass Julia callback routines to C library functions (including
libpython), but in the future the same facility should allow the
generation of C-callable libraries written in Julia.
</blockquote>

## Slides and IJulia notebooks

To use the IJulia notebooks, you will need to download Julia and
install IJulia: see the [IJulia installation
instructions](https://github.com/JuliaLang/IJulia.jl#installation).

* Slides in [PDF](Julia@EuroSciPy.pdf) and [PowerPoint (pptx)](Julia@EuroSciPy.pptx) formats.

* [IJulia tutorial notebook](http://nbviewer.ipython.org/github/stevengj/Julia-EuroSciPy14/blob/master/Overview.ipynb)
