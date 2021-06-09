---
title: My Data Science Internship Story
date: 2021-01-10 09:00:00
tags:
    - Experience
    - Internship

category: Experiences 
keywords:
    - Data Science
    - Internship Experience
mathjax: true
---

### My Data Science Internship Story
*Originally Published in [TowardsDataScience](https://towardsdatascience.com/ai-learns-to-multiply-ce844c68aefe)*

#### Things I experienced during my 9-month stint at an AI-Healthcare startup

> Hey everyone! A very happy new year. I wanted to start this year off by sharing
> my recent experience as a Data Science Intern at Dozee, an AI based healthcare
startup in India. I’ll try to cover everything from what my daily schedule to my
learnings and overall experience.

![](https://cdn-images-1.medium.com/max/1200/1*bQ7d3uy8rCFOyQoOMvQOmA.jpeg)
<span class="figcaption_hack">Photo by [Hemerson
Coelho](https://unsplash.com/@hemersoncoelho?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
on
[Unsplash](https://unsplash.com/s/photos/animal-laptop?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)</span>

### Some Context

Towards the end of my junior year, I was introduced to the field of deep
learning and computer vision. What caught my attention the most was their use in
biology and medicine to accelerate their rather saturated growth over the past
few decades. By the end of my sophomore year, I was quite convinced to work in
the intersection of medicine and AI for my final year internship. I successfully
secured a position in one of the world’s leading medical robotics institute in
France to work on computer vision challenges. But then, COVID hit. The travel
restrictions rescinded my goal of working in such a setting. I felt broken and
also a bit anxious, for the opportunity was a perfect match. Little did I know
what was waiting for me ahead.

In April of 2020, I interviewed with [Dozee](https://www.dozee.io/), and soon
after a week, I had the offer to work with their research team as a Data Science
Intern. Today, I’m delighted with the experience I’ve had, especially the
possibility of experiencing both the research side and the production side.

> If you ever miss on an opportunity that you feel was the most perfect match that
> the universe could offer, Don’t worry! There’s an equally good (if not better)
opportunity waiting around in the corner. All you have to do is put in the
effort and unearth it.

*****

### Daily Groove

Starting out, I’d like to give a brief into what my daily schedule looked like.
With the flexibility of timings, I started working around 11 AM each day and
would end by 8 PM. With pandemic limiting the experience to a *Work From Home*
one, I didn’t have to worry much about lunch or dinner breaks.

![](https://cdn-images-1.medium.com/max/1200/1*aX3K-rFVF7jNdTtuUCFnMA.jpeg)
<span class="figcaption_hack">Photo by [Lukas
Blazek](https://unsplash.com/@goumbik?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
on
[Unsplash](https://unsplash.com/s/photos/work?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)</span>

The day generally started with a scrum call at 10 AM sharp. During this, the
team discussed the recent development in their respective verticals and the
proposed plans for the day. It usually lasted between 10 and 15 minutes, and the
call certainly set the tone for the day. On some days, there were tasks with
high priority, and on other days, it was all about upcoming meetings and
discussions.

I broke my sessions into three parts(*at least tried to*). Between 11 AM to 2
PM, I tried finishing up small scattered tasks that didn’t take much time. For
instance, updating a function as per new requirements, completing the daily
testing of deployed algorithms, or writing scripts for some quick automation
task. I then took a pause for about thirty-forty minutes and was back active on
slack. Before leaving for lunch, I usually left some time-taking tasks running
on our GPUs. Between 2:30 PM to 5:30 PM, I spent my time working on the central
tasks of the day. These included perusing through articles and research papers,
formulating solutions, and gathering all that was required for building the MVP
for the task. This was the most interesting part of the day as I discovered and
explored the most here. I usually spent the time between 6:00 PM to 8:00 PM,
converting the logic and idea developed in the previous session into code. This
was quite straight forward most of the time. I tried to have a working code
ready before calling it a day and optimized it the following morning. In
between, there were calls spread out throughout the day for project discussions
and bug fixing. However, the schedule every day was not that neat and sectioned;
sometimes, I spent two-thirds of the day just fixing bugs.

Apart from this, we had weekly research and development discussions on our
ongoing project in the team. I loved them! It was an extensive open-ended
discussion where we all bounced off ideas on different approaches to hurdles in
our projects. They were healthy 2–3 hour long discussions ranging from ideation
of a new project to optimizing the strategies that were already developed.

> I loved the idea of weekly R&D discussions. It was a great way to get everyone
> on board with the progress in different projects and also gave everyone a chance
of collaborating and contributing. In fact, the idea for a very fundamental part
of the project I was working on took shape in one of our R&D discussions.

After working on an idea thoroughly, we habitually had presentation sessions
where we explicated the idea, it’s performance and scrutinizing the possibility
of integration. It consolidated everything with considerations to the project.

*****

### Project Breakdown

Talking about the project, I’d break it down into three main stages: Ideation,
Test, Production, each being more important than the other.

![](https://cdn-images-1.medium.com/max/1200/1*5X0v7PSv3Nn7Nxoa-uak9A.jpeg)
<span class="figcaption_hack">Photo by [Jo
Szczepanska](https://unsplash.com/@joszczepanska?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
on
[Unsplash](https://unsplash.com/s/photos/project?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)</span>

#### Ideation

Some might argue this being the most crucial of all stages, for the idea will
decide the performance in the latter stages. As a newbie intern, this was my
first broad task. I was given the problem statement, and I had to find ways to
solve it. It was quite overwhelming at first! I remember spending days reading
research papers, experimenting with the existing techniques, and other previous
work around the topic. The interesting part was that Dozee is based on
Ballistocardiography(BCG), a method in which vitals are monitored by measuring
the body’s reaction to the cardiac ejection of blood. Not much work was done
around this topic, let alone my specific project statement. I had to derive many
ideas from past work on ECG and Actigraphy. If you are wondering how your
smartwatch is able to measure your heart rate, it is wrist actigraphy, an
interesting area of convergence of healthcare and machine learning. The thought
of the possibility of our idea being a first of its kind kept me going and
pushed me to explore deeper.

There were two levels of idea rejections I encountered. The first one was
easy-to-reject. After briefly assaying an idea or approach and its compatibility
with our product, we could easily discard the idea. Maybe we don't have the
required inputs, or maybe it is impossible to imagine it in real-time. The
second type of ideas were plausible ones—the ones which *could *work. The only
way to find was to proceed with working on the idea. This was time taking, and
it was imperative not to waste time on ideas that won’t fit. Over a period of
three months, I worked on four promising ideas and strategies. The first three
turned out to be a total bust. We were achieving results below our existing
benchmarks. The final method was the one that crossed all our benchmarks and, in
fact, beating every work on BCG with a similar problem statement.

It’s worth mentioning that hadn’t I tried the first three methods, it would be
difficult for me to arrive at our current successful strategy. Working on each
idea helped me look at the problem from a different dimension and collectively
developed a conception of the reasons for their failure. This also helped me
dive profound and understand what exactly we were trying to solve, why it was
important, and not to mention the biological side of the problem.

#### Testing

There were four approaches that iteratively made it to the testing phase. By
*iteratively, *I mean that the second approach was built based on learnings from
the first one, or the final approach was based on learnings from the previous
three approaches. This was a time-consuming stage. It involved generating data
points, handcrafting features, and training deep learning models for hours or
days together. A pipeline had to be built to convert the raw signals that I had
to a form that can be used as an input to the model. Building the pipeline for
the first approach was the most challenging as for the other three approaches
the same pipeline could be modified and used. The general procedure that I
followed, guided by other data scientists in our team was to:

a) Build the most basic architecture for benchmarking.

b) Experiment with different feature spaces with this architecture.

c) Proceed with designing better architectures with the most promising feature
space.

This really helped me in evaluating and comparing features, model architectures
in an active and organized manner. My first two approaches were based on an
image as a feature, and I remember waiting eagerly to visualize and evaluate the
cause of the bad performance of the model. At one point, I was building so many
models with varied feature space that they stopped seeming like *Black Boxes,
*and it was as if I knew why they failed and what would fix them (and it
appeared true in 60% of the cases :D)*. *This stage was the penultimate
challenge for the approach to prove its state of the art performance. Usually,
there is one winner, and it goes on to the final state. However, it can still be
rejected in the final stage if it doesn’t meet server and production criteria.

#### Production

*The Holy Grail. *After building the best model with legendary scores, it’s time
to fit it into the working pipeline of your product. Many factors now come into
play, such as computational costs, real-time feasibility (depends on product),
storage requirements (and costs), satisfying the server configuration (or the
need to build a new instance), and many more. It is crucial to evaluate the
model performance for each of these factors. A failure in one of them may mean
you will be starting on a new idea or using other approaches that made it to the
testing phase. Generally, these are solvable. It is reasonably easy to optimize
your architecture and make it lightweight. We generally use techniques such as
Pruning and Quantization to reduce the compute requirement significantly.
Intermediate pipelines might be required to make the model compatible with the
running pipeline. Keeping in mind the server configuration and other factors
that can’t be changed right in the ideation stage can save you a ton of hours.

Satisfying all the requirements still doesn’t mean that your model is ready to
be deployed. A lot of beta testing goes on between making your code
production-ready and actually deploying it to all users. Internal users receive
the updates with the new model, and a month or two of testing is carried on
where a daily log is maintained on the performance. Users are also reviewed on
their experience with model performance. After a thorough period with stable
performance free of code breaks, the model is all set to be released to everyone
using the product. I remember the day when the pull request was sent to merge
our project with the main branch. It was an amazing feeling. The feeling of
having my work up and running on thousands of devices was totally amazing. It
took almost seven months to get the work into production, and it was worth every
minute spent.

*****

### My Overall Experience

Today tens of thousands of data points are passed each day through the pipeline
we built, and it makes me ecstatic. I loved how I was given the freedom to
experiment with different techniques and come out with an approach that
satisfied all our needs. I loved being included in the testing and production
stage and just on building the model. I loved the opportunity of contributing to
other ongoing research projects. And finally, I loved being part of all research
discussions, scrum calls, monthly team meetings, which gave me a feel of a
full-time data scientist.

> If you are looking for a full fletched exposure as a Data Scientist, ML/AI
> Engineer, you can’t go wrong by working with a Startup, given your goals and
interests align.

With increasing importance being given to healthcare, today, we see more such
startups coming up. Working at Dozee certainly brought me closer to my interest
in the intersection of medicine and AI, and the future potential in the field
really excites me.

Interested in knowing more about our findings? Our Pre-print is live:

Thanks a ton for reading. I hope you enjoyed it. If you feel I missed something
or if you'd like to know more, please leave it in the comments below if someone
from the Dozee team is reading this; thanks for the opportunity!

Intersected in reading more on AI? Explore the articles below.

![](https://cdn-images-1.medium.com/max/1200/1*CFZ9evlIdxoKpVUSEsfiBA.jpeg)
<span class="figcaption_hack">Image by Author (A recent click)</span>

<br> 
