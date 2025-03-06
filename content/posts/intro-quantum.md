---
title: "1 - Intro To Quantum"
date: 2025-02-26T21:51:01-05:00
tags: ["Quantum"]
draft: true
---
  
#### Intro

In this series I am going to be posting my notes about quantum computing. My goal is to share knowledge as I go, with the hope that my discoveries and understandings could help and influence another person interested in the topic.

In this section we will start from the very basics of quantum computing and quantum information. Most of this section will be very closely coupled to the textbook _Quantum Computation And Quantum Information 10th Edition_ by Nielsen and Chuang.

This textbook is extremely thorough in the amount of content it provides. I couldn't recommend it more for anyone looking for a starting point in quantum computing.

#### The Basics

In classical computing, computers can do operations such as arithmetic, comparisons and logic using bits.

- **bit** - most basic unit of information in classical computing and digital information

Bits are binary, meaning that there are only two logical states, generally represented with \(1\) or \(0\). Using only one bit to convey information is somewhat trivial because it can only give us maximum 2 outcomes. Is the bit on or off? However, if we string multiple of these bits together we can start doing more advanced things, as the possible amount of information we can hold increases.

Once useful thing we can do with bits is represent numbers. Stringing together bits, we can represent any real integer in base 2. For example this is how we would represent the number 187:

$$10111011$$

$$(2^{7}*1) + (2^{6}*0) + (2^{5}*1) + (2^{4}*1) + (2^{3}*1) + (2^{2}*0) + (2^{1}*1) + (2^{0}*1) = 187$$

I won't go into further about classical computing because that is out of scope for this series. However, the above example should highlight the limitation of classical computing.  Bits can only hold two outcomes of information, meaning to encode more information, we need more bits and to compute this information we need more steps in our algorithms.

The beauty in quantum computing is that contrary to a classical bit being either \(0\) or \(1\) at a given point in time, qubits (quantum bits) can be a blend of the these two positions. Due to this we need a way to describe these states in a mathematical way rather than a single value.

- **qubits** - _mathematical objects_ with certain specific properties

For this we often describe a qubit as a two-dimensional vector in complex space, the equation below describes this relationship:

$$|\psi\rangle = \alpha|0\rangle + \beta|1\rangle$$

The coefficients \(\alpha\) and \(\beta\) are complex numbers describing the state of a qubit at a given point. This linear combination of \(|0\rangle\) and \(|1\rangle\) is what we consider _superposition_. We cannot examine the these coefficients directly, however. If we try to determine the state of this vector the state will actually collapse directly to either \(0\) or \(1\). Instead, we can only know the probability of \(0\) being \(|\alpha|^{2}\) and the probability of \(1\) being \(|\beta|^{2}\).  
