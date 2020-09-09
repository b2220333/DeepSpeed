---
layout: single
title: "Up to 5x less communication and 3.4x faster training through 1-bit Adam"
excerpt: ""
categories: news
new_post: true
date: 2020-09-09 00:00:00
---


Adam is an effective and probably the most well-utilized optimizer for
training many large-scale deep learning models.  However, Adam is generally
not compatible with communication-efficient optimization algorithms, and
therefore the communication cost could become a bottleneck while scaling
across distributed devices. We introduce a new algorithm - 1-bit Adam - and
its efficient implementation in DeepSpeed. 1-bit Adam offers the ***same convergence*** as Adam, incurs up to ***5x less communication*** that enables up to ***3.5x higher throughput for BERT-Large pretraining*** and up to ***2.7x higher throughput for SQuAD fine-tuning*** on bandwidth-limited clusters.

* Brief overview, see our [press release](https://www.microsoft.com/en-us/research/blog/zero-2-deepspeed-shattering-barriers-of-deep-learning-speed-scale/).
* Detailed technology deep dive, see our [blog post](https://www.deepspeed.ai/news/2020/09/09/onebit-adam-blog-post.md).
* Tutorial on how to reproduce our results, see our [1-bit Adam tutorial](https://www.deepspeed.ai/tutorials/onebit-adam/).
* The source code for 1-bit Adam can be found in the [DeepSpeed repo](https://github.com/microsoft/deepspeed) and example codes to try this feature can be found in the [DeepSpeedExamples repo](https://github.com/microsoft/deepspeedexamples).