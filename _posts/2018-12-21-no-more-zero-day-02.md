---
layout: post
title: '[NMZD #02] Why does deep learning actually work?'
author: Duy Huynh
published: true
---
From quora: [Why does deep learning actually work?](https://www.quora.com/Why-does-deep-learning-actually-work)

Loren Peter Lugosch:
People often say deep learning works because neural networks can approximate any function.

That's true, but that's not why deep learning works so well. After all, there are plenty of shallow function approximators - like Gaussian mixture models, polynomials, and neural nets with just one hidden layer - that can approximate any function.

Deep learning works because it's easier to write a program using functions than using just straight line code. Imagine if you had to write code and weren't allowed to use any function calls. If you wanted to reuse some code, you would have to copy it out every time you want it to run. That would make your code gigiantic and hard to maintain. (Imagine trying to write an operating system like that!)

Layer of a deep neural network are like functions. The last layer is the main function that returns the output. That function calls other funcitons - the previous layer in the network - and those functions can in turn call other functions.

