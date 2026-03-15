# Category Theory: A Practitioner's View

I am not a category theorist. My knowledge is basic, but I have read enough category theory and worked closely with category theorists for some time. Also my PhD thesis had some category theory. This is all to say, for a good, rigorous program on category theory, some resources that I can list are: 

- Emily Riehl's book - I am a big fan of Emily Riehl and Dom Verity (who I had the fortune to work with briefly at Symbolica). This introduction to category theory is full of examples that connect categories to many parts of mathematics. 
- Bartosz Milewski Blog and YouTube series - this especially resonates with programmers. 
- Category Theory for the Sciences - I liked this text because it 
- My good friend Bruno's Gavranovic's work - especially if you are interested in $\text{AI}\cap\text{Categories}$, this is the best place to go. 
- David Spivak's work - in particular Seven Sketches in Compositionality. 

That being said - maybe I can add something: *a practitioner's view*. Where category theory has mostly helped me is in the modelling and design of problems and understanding how abstractions relate to each other. Both in mathematical finance and artificial intelligence, we often find that there are many different models of learners and markets. Understanding how the different models compare with each other is the work of categories. 

## Benefits of Category Theory

### Moving Between Different Models
In AI, you may model a learner as a:
- A parametrised function $f_\theta: \mathbb{R}^n \rightarrow \mathbb{R}^m$, 
- A conditional probability distribution,
- A dynamical system, $(f_\theta, \mathcal{L})$
... and many others! Exotic objects such as quivers are used to study some properties. 

Markets on the other hand are:
- Vector spaces (in the sense of Arrow), 
- Stochastic processes
- Games, 
- Dynamical systems 
I'd like to think that the properties that we find in one model are reflected in all other models. Some models are simpler than others, but if we expand them, we should be able to recover different versions of the same results. 

Generally this is the idea. I have a phenomenon and I want to model it with mathematical object $X$. Mathematical object $X$ has these properties - and if this object is a good model of the phenomenon, I should be able to move back and forth between my intuitive understanding of the phenomenon and the mathematical object's properties. 

### Prescriptions for Artificial Intelligence
I initially got into categories because I thought they could *solve* the problem of architecture in artificial intelligence. Specifically, it seemed that different models (Recurrent Neural Networks, Convolutional Neural Networks etc.,) performed better at a task if they were *adapted* to that task. I talk about this in the [Geometric Deep Learning] chapter. People in Geometric Deep Learning had started speaking of category theory as a unifying framework, the way that it had helped in the Langlands Programs. So I thought, let's have a look at category theory. 

### Concepts of Sameness
Even just a basic understanding of it enriched the way that I think about mathematical modelling - and again, I don't feel like I ever got much farther than the basics. Firstly, a deeply satisfying quality of categories is their graphical aspect, which is of great help to visual thinkers such as myself. It throws equations out of the page and into *diagrams* and introducing graphical calculi to think about tensor operations. 

This alone emphasizes a truth about mathematical reasoning (and computation) which is that **langauge matters**. Language defines the atomic operations that you are allowed to do, that span the space of your thinking. You can solve an equation by joining diagrams in your mind, or you can rewrite a formula on a page - while these are technically the same operation, maybe the cognitive or metabolic cost is different. That might be what makes some people visual thinkers etc., Therefore, translating from one language (formal mathematical) to another (graphical/ visual) is like re-writing your operations as CuDA functions and finding a faster GPU implementation to run them. 

Moreover, in the context of theorem proving, categories allow us to model mathematics. 

### Yoneda's Lemma
In an interview, Emily Riehl said that she occasionally came back to Yoneda's Lemma and found new depth to it in her mathematical career. First time you read it, it is a statement about natural transformations (an important mathematical object in categories). You may not even grasp it fully. As you accept it more in your toolkit, it has operational properties: being able to use it is to understand some results in categories. For me it has percolated in my understanding of what *meaning* is. 

We will talk about Yoneda's Lemma. 