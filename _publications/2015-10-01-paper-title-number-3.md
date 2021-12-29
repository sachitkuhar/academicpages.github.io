<!--  ---
title: "SumMerge: an efficient algorithm and implementation for weight repetition-aware DNN inference"
authors_before_me: "Rohan Baskar Prabhakar*,"
author_me: "Sachit Kuhar*,"
authors_after_me: "Rohit Agrawal, Christopher J Hughes, Christopher W Fletcher"
collection: publications
permalink: /publication/2021-ics-summerge
date: 2021-6-3
excerpt: 
venue: 'ACM International Conference on Supercomputing'

--- -->
<!-- This paper is about the number 3. The number 4 is left for future work. -->
<!--
[Paper](https://dl.acm.org/doi/abs/10.1145/3447818.3460375)

Deep Neural Network (DNN) inference efficiency is a key concern across the myriad of domains now relying on Deep Learning. A recent promising direction to speed-up inference is to exploit weight repetition. The key observation is that due to DNN quantization schemes—which attempt to reduce DNN storage requirements by reducing the number of bits needed to represent each weight—the same weight is bound to repeat many times within and across filters. This enables a weight-repetition aware inference kernel to factorize and memoize out common sub-computations, reducing arithmetic per inference while still maintaining the compression benefits of quantization. Yet, significant challenges remain. For instance, weight repetition introduces significant irregularity in the inference operation and hence (up to this point) has required custom hardware accelerators to derive net benefit.

This paper proposes SumMerge: a new algorithm and set of im- plementation techniques to make weight repetition practical on general-purpose devices such as CPUs. The key idea is to formu- late inference as traversing a sequence of data-flow graphs with weight-dependent structure. We develop an offline heuristic to select a data-flow graph structure that minimizes arithmetic operations per inference (given trained weight values) and use an efficient online procedure to traverse each data-flow graph and compute the inference result given DNN inputs. We implement the above as an optimized C++ routine that runs on a commercial multicore processor with vector extensions and evaluate performance rela- tive to Intel’s optimized library oneDNN and the prior-art weight repetition algorithm (AGR). When applied on top of six different quantization schemes, SumMerge achieves a speedup of between 1.09×-2.05× and 1.04×-1.51× relative to oneDNN and AGR, respec- tively, while simultaneously compressing the DNN model by 8.7× to 15.4×. -->

<!-- Recommended citation: Your Name, You. (2015). "Paper Title Number 3." <i>Journal 1</i>. 1(3). -->
