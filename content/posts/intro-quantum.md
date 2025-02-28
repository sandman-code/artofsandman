---
title: "1 - Intro To Quantum"
date: 2025-02-26T21:51:01-05:00
tags: ["Quantum"]
draft: true
---

In this series I am going to be posting my notes about quantum computing. My goal is to share knowledge as I go, with the hope that my discoveries and understandings could help and influence another person interested in the topic.

In this section we will start from the very basics of quantum computing and quantum information. Most of this section will be very closely coupled to the textbook _Quantum Computation And Quantum Information 10th Edition_ by Nielsen and Chuang.

This textbook is extremely thorough in the amount of content it provides. I couldn't recommend it more for anyone looking for a starting point in quantum computing.

#### The Basics

In classical computing, computers can do operations such as arithmetic, comparisons and logic using bits.

- **bit** - most basic unit of information in classical computing and digital information

Bits are binary, meaning that there are only two logical states, generally represented with **1** or **0**. Using only one bit to convey information is somewhat trivial because it can only give us maximum 2 outcomes. Is the bit on or off? However, if we string multiple of these bits together we can start doing more advanced things, as the possible amount of information we can hold increases.

Once useful thing we can do with bits is represent numbers. Stringing together bits, we can represent any real integer in base 2. For example this is how we would represent the number 187:

$$
10111011
$$

$$
(2^{7}*1) + (2^{6}*0) + (2^{5}*1) + (2^{4}*1) + (2^{3}*1) + (2^{2}*0) + (2^{1}*1) + (2^{0}*1) = 187
$$

**qubits** - _mathematical objects_ with certain specific properties

$$
|\psi\rangle =  \alpha|0\rangle + \beta|1\rangle
$$
