---
title: The Rush to Push AI to Edge
date: 2020-06-27 09:00:00
tags:
    - Startups
    - Technology

category: Technology 
keywords:
    - Technology
    - AI
mathjax: true
---

### The Rush to Push AI to Edge

#### Why companies such as Apple, Intel, Google are trying to move AI from cloud to edge

Earlier this year, Apple announced its US$200 million acquisition of
Seattle-based edge-AI startup Xnor.ai. This was one of its many other moves to
bring the AI-inferencing from cloud to the local hardware.

![](https://cdn-images-1.medium.com/max/2600/1*PCzubicRuPeHqrZKC739xw.png)
<span class="figcaption_hack">Canva.com</span>

Today, algorithms sit on the cloud and serve your requests. As you can guess,
there can be a latency as the data has to travel between the cloud servers and
the remote client. There might also be many privacy concerns attached. The
steady growth in the power of smart-devices is slowly giving rise to the
opportunity to run the algorithms locally on edge instead of on the cloud. All
major tech-giants are now in the race to push AI to the edge.

> “Machine learning is going to happen at the edge in a big way, The big question
> is how do you do it efficiently?” says Stanford Professor Subhasish Mitra.

### What is Edge AI?

In Edge computing, data is processed by the device itself or by a local computer
or server, rather than being transmitted to a data center, says HP. Now when we
talk about AI, these computations become quite complicated, and ordinary edge
devices become incapable of performing them. That is why presently, these
complex computations are left to the hefty servers at the data center.

If you have ever used FaceApp (Application to try different looks), you might
have noticed the considerable amount of time that it takes to give you the
result. What’s happening on the backend is that your image(encrypted) is being
sent to the remote server, the server applies the algorithm requested by you and
sends it back to your device. Now, if that complete process somehow takes place
in your local itself, it would be much faster and not mention much secure. This
is where Edge-AI comes in, and companies like Xnor.ai are building tech that
enables local inferencing possible.

![](https://cdn-images-1.medium.com/max/900/1*XZhWZpKTzAma6zIlc-zgNg.png)
<span class="figcaption_hack">The Rush to acquire the best ~CBINSIGHTS</span>

### Why does Edge AI matter?

Edge AI gives rise to a possibility for mission-critical and time-sensitive
decisions to be made faster, more reliable, and with greater security. For Apple
and many other companies that claim to put the privacy of a user above all, edge
AI would definitely be a go-to piece of technology.

Xnor.ai’s technology runs deep learning models efficiently ​on edge devices such
as phones, IoT devices, cameras, drones, and embedded CPUs. The trick is to
build highly efficient hardware that is capable of running power-hungry
algorithms without much loss in the accuracy of these algorithms. Apple’s
acquisition of Xnor.ai will potentially help it challenge the big guys in cloud
technology, Amazon Web Services, Microsoft Azure, and Google Cloud. On the
otherwise, all of these are also continuously increasing their focus on
harnessing the benefits of AI and edge computing.

### How do you optimize for the edge

There can be two broad ways in which you can go about improving the performance
of the algorithms on edge: Optimizing the model architecture, Optimizing the
device hardware, or both.

**Optimizing the model architecture**

Traditional AI algorithms use a conventional representation of numbers. For
example, your 32-bit PC might be using 32-bit weights and biases for the model.
Over the years, what people have observed is that the weights and biases don’t
need to be precise to 32 or 64-bit to give good accuracies. Studies show that
when 32-bit precision weights and biases are replaced by 8 or 16-bit precision,
there is no significant drop in the accuracy of the model.

One Publication by Xnor.ai titled [ImageNet Classification Using Binary
Convolutional Neural Networks](https://arxiv.org/pdf/1603.05279.pdf), published
in 2016, proposes two efficient approximations to standard convolutional neural
networks: Binary-Weight-Networks and XNOR-Networks. They reduce the precision to
1-bit(binary) in order to save memory by 32 times. The XNOR-Networks approximate
convolutions using primarily binary operations resulting in 58 times faster
computation. The final scores were excellent; the paper says, “the
classification accuracy with a Binary-Weight-Network version of AlexNet is the
same as the full-precision AlexNet,” which is purely amazing. One thing to note
is that the paper was published in 2016 and, there are better architectures
today.

**Optimizing the Hardware**

The next approach could be building better hardware to support compute and
power-hungry AI algorithms. Myriad was one such company working on developing
hardware units, especially for AI Inferencing. In 2016, AI acquired Movidius and
the hardware today is known as Intel’s Neural Compute Stick. The Neural Compute
Stick or NCS allows you to develop, fine-tune, and deploy traditional
convolutional neural networks (CNNs) on low-power applications that require
real-time inferencing.

![](https://cdn-images-1.medium.com/max/900/1*GDFsE0GRjbst0zXqf3_Nlg.png)
<span class="figcaption_hack">Intel NCS2 ~ intel.com</span>

NCS Stick works with Intel’s OpenVINO toolkit that helps you to take your
traditional machine learning model, generate Intermediate Representations, and
then use the Inference Engine to infer the result for a given input data. The
intermediate representations are generated by the Model Optimizer module of the
toolkit that converts your model to a form that’s faster in inferencing.

The best method would, however, be the software-hardware co-design of the entire
pipeline. This would ensure that your performance is optimized on both hardware
and software levels. In the video below you, can see how Xnor.ai does a
fantastic job of building a solar-powered object detection chip. The use of such
chips can span thousands of real-life applications.

#### What’s in hold for us

As Edge AI gets more powerful and starts taking shape, we will witness true-AI
on our devices. Our smart devices would no longer be required to connect to the
internet to access AI-based applications; the latency would reduce drastically,
and above all, true-privacy would be ensured.

![](https://cdn-images-1.medium.com/max/1200/1*uAFDt1cT_2sGOfidnLuixg.png)
<span class="figcaption_hack">Canva.com</span>

*****

*It’s one exciting time to be alive with a lot of exciting stuff happening
across the globe. One thing that I definitely look forward to is how edge AI
influences healthcare once it is mature. Thanks for reading the article and I
hope you enjoyed it. See you soon :)*
