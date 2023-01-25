# Language

_What is the name of the language? Link the name to its webpage
(if appropriate)._

The name of the language I chose is OpenCV.

# Domain

_Describe the language's domain in five words._

images and computer vision.

# Computational model

_We don't yet have a great definition of the term "computational model".
For now, try to come up with the clearest, most concise explanation of
what happens when a program in your DSL runs._

Anything could happen? It's typically used to manipulate images, so it has
built in functions for anything from blob detection to saturation/contrast manipulation.
So when a program is ran using OpenCV, an image could be output with different contrast
values or increased saturation.

# DSL-ness

_Fowler writes about a spectrum of languages, from general-purpose languages to
"purely" domain-specific. Where does the DSL you chose fall on this spectrum,
and why?_

I think it's a mix of the two. OpenCV can have a general use cases for anything in
regards to manipulating image data, but that's about it. You're not going to be writing
conditionals/for loops in the library, thus it's domain  specific and it's domain is in 
computer vision.

# Internal or external?

_Is the language implemented as an internal or external DSL?
Justify your answer._

It is an internal DSL, as script in OpenCV can be used in any of it's host languages, which
include Python/C++/Java.

# Host language

_What language(s) was (were) used to implement the DSL?_

The languages used to implement OpenCV are C, C++, Python, Java, and Assembly, although I suspect
it's written primarily in C and assembly and hosted in C++/Python/Java implementations.

# Benefits

_Identify one potential benefit of the DSL: how is a programmer's life made
easier by the existence of this language?_

One benefit of the DSL is that intensive computer vision operations can be automated and then
accelerated with GPU acceleration. Instead of writing out for loops to loop over every pixel
in an image to perform some operation, a quick call to any of it's built in methods can make 
the code much more readable and can provide an abstraction to manipulate images. It also helps
that it can utilize GPU acceleration, as intensive resource demanding operations such as 
machine learning can be done much faster, as opposed to writing your own CUDA driver and
doing the work for that.

# Drawbacks

_Identify one potential drawback of the DSL: what does a programmer
lose by using this DSL instead of a general-purpose language?_

One thing lost is that you're no longer writing Python/Java/C++ code to manipulate the image
itself, but that you're writing using the OpenCV library. While of course you can still access the
pixel values for each individual pixel or see the image's metadata, you now have to implement
it using the openCV library, which has a learning curve with it's own documentation which can
be steep.