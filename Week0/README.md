# Cerebral Cinema - Week 0

## Introduction
Hey everyone, hope y'all are a bit rejuvenated after your endsems :)). As mentioned before we'll be starting week 0 of the project from today - there are no assignments this week, I just want all of you to understand the problem we are going to be solving and some of the techniques that we will be using to solve it. 

On a side note, I plan on having the first offline meet sometime next week so please make sure you are on campus by then. We will be discussing the contents of this week in the meet. 

Also I would encourage you guys to form **groups of 3-5** to work. We will circulate a google sheet later in the day where you'll have to fill out your groups. 

If anyone is left with their intros on whatsapp then do that as well :)

You all will have different levels of knowledge when it comes to ML, so I am going to give all the resources one would need but feel free to skip whatever you already know. 

## The Problem at Hand

I'm currently watching Suits for the 4th time and I'm on season 6 which means for those of you who have watched it, it's a season that keeps you on the edge, but have you ever wondered what goes on in your brain when you watch a movie that keeps you on the edge?

Neuroscience has been trying to answer this for decades, but the traditional approach has been very narrow, studying one cognitive function at a time, in highly controlled lab settings. Recently people have started using Deep Learning methods to decode and predict brain activity.

The Algonauts 2025 Challenge brought the world's best researchers together around exactly this problem. Meta AI's winning solution, TRIBE, showed that a well-designed multimodal model could predict how the brain responds to movies. It was a landmark result, and it's what directly inspired this project. Over the next 8 weeks, you're going to build something along those same lines — a model that watches a video, reads the corresponding text, and predicts what the human brain would look like responding to it.

## Resources
### The Basics
1. **Refresher on ANNs:** [This](https://www.youtube.com/watch?v=w8yWXqWQYmU&t=1458s) is not a standard 3B1B video, you all must have watched that already, watching this video will give you an idea of the math behind AI and how a neural network actually works. 
2. **Different types of machine learning:** [IBM Article on types of machine learning](https://www.ibm.com/think/topics/machine-learning-types). We are going to be exploring JEPA models in this project and for that you need to understand how AI progressed from supervised learning to the current paradigms. 
3. **Yann LeCun's blog on Self-Supervised learning:** [Meta's Article on SSL](https://ai.meta.com/blog/self-supervised-learning-the-dark-matter-of-intelligence/). This is a rather advanced article and it doesn't matter if you don't understand everything but try to get an idea of SSL and how it is going to be the future of AI. 
4. **Embedding Spaces and Embeddings:** [This video](https://www.youtube.com/watch?v=hVM8qGRTaOA) will give you an overview of what an embedding really is and **YOU NEED TO UNDERSTAND THIS** as this will be the backbone of our project. 

**Yann is one of the most highly regarded researchers in this field and he has, on multiple occasions, made claims that LLMs are NOT the future of AI!**

### LLMs and JEPA

Now that you have an idea of why self-supervised learning matters, let's look at the two architectures that are at the core of our pipeline: LLMs for the text modality, and JEPA for the video modality.

But before we dive into either, let's first understand the building block that powers both: **the transformer.**

1. **Transformer Architecture:** [Grant Sanderson's talk on transformers](https://www.youtube.com/watch?v=KJtZARuO3JY&t=581s). He is the guy who runs the YouTube channel 3B1B and this hour long video will get you a very good idea about transformers and basically sums up his series on transformers.  
**(Optional) If interested, you can read [Attention is All You Need](https://arxiv.org/abs/1706.03762), the original paper that introduced the transformer.**

2. **Large Language Models (LLMs):**
   - Start by reading this [IBM Article](https://www.ibm.com/think/topics/large-language-models#692473873) for an overview on LLMs.
   - Watch [Andrej Karpathy's video](https://www.youtube.com/watch?v=zjkBMFhNj_g&t=1510s) for an intro to LLMs. This video abstracts the idea of an LLM and gives practical insights into how they work.
   - **(Optional) [Building GPT from scratch](https://www.youtube.com/watch?v=kCc8FmEb1nY&t=3416s): Another video by Andrej Karpathy, only for those interested.**

3. **JEPA and SSL:**  
   So if LLMs predict the next *token*, JEPA asks a more interesting question: can a model learn to predict the next *representation* of the world? Instead of working in raw pixel or token space, JEPA learns in an abstract embedding space, which turns out to be much closer to how the brain actually works. This is what makes it so well-suited for our project.
   - There's this channel, [Welch Labs](https://www.youtube.com/@WelchLabs/videos), that has started posting about AI recently. He makes videos about the most non-mainstream and fascinating topics in AI, I'd highly recommend checking him out, the videos are often lengthy but always worth it.
   - Specifically, watch [this video](https://www.youtube.com/watch?v=kYkIdXwW2AE&t=2s), it's at the heart of our project and has insights from Yann himself! He'll also be releasing a second part soon, so stay tuned :)
