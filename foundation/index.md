---
title: Foundations of Artificial Intelligence
description: "The foundations of artificial intelligence: the eight disciplines AI grew out of, the founding papers from Turing to Dartmouth, and the math modern models still rely on."
updated: "2026-11-18"
keywords:
  - foundations of artificial intelligence
  - foundations of AI research
  - history of AI
  - Dartmouth workshop 1956
  - Turing test
  - mathematics for machine learning
  - search and reasoning
---

# Foundations of Artificial Intelligence

Artificial intelligence is the study of building systems that perceive their environment, reason about it, learn from experience, and act to achieve goals. It did not appear from nowhere in the 1950s. AI was assembled from older questions asked in at least eight other disciplines, and each one still supplies a piece of how modern systems work.

This page covers three things: the disciplines AI is built on, the founding papers and events that turned those ideas into a research field, and the core concepts (search, representation, uncertainty, learning, optimization) that every later section of this library depends on.

## What "foundations" means in AI

When textbooks talk about the foundations of AI, they usually mean the answer to a simple question: *which older fields contributed the ideas, tools and problems that AI researchers use?* The standard answer, popularized by Russell and Norvig's textbook *Artificial Intelligence: A Modern Approach*, lists philosophy, mathematics, economics, neuroscience, psychology, computer engineering, control theory and linguistics. The sections below take them one at a time and name what each one actually contributed.

## The disciplines AI is built on

### Philosophy: can reasoning be mechanized?

Philosophers asked whether correct reasoning follows rules, and if so, whether those rules could be written down. Aristotle's syllogisms were an early catalogue of valid inference patterns. Much later, philosophers debated the relationship between mind and matter: if thinking is a physical process, a machine might in principle carry it out. AI inherits both the hope that intelligence can be described precisely and the unresolved questions about what understanding and consciousness are.

### Mathematics: logic, computation and probability

Mathematics turned those philosophical hopes into formal tools:

- **Logic.** George Boole's *The Laws of Thought* (1854) treated reasoning as algebra over true and false values. Gottlob Frege's *Begriffsschrift* (1879) extended this to first-order logic, the language still used in knowledge representation and automated theorem proving.
- **Limits of computation.** Kurt Gödel's incompleteness theorems (1931) showed that sufficiently powerful formal systems contain true statements they cannot prove. In 1936 Alan Turing and Alonzo Church independently gave precise definitions of what can be computed at all. Turing's abstract machine became the model for every digital computer, and the notion of problems that are computable but intractable (too slow to solve in practice) shapes how AI systems approximate instead of solving exactly.
- **Probability.** Bayes' rule, published posthumously in 1763, gives a principled way to update beliefs when new evidence arrives. It underlies spam filters, medical diagnosis systems, and the probabilistic view of machine learning.

### Economics: decisions and utility

Economics asked how agents should choose when outcomes are uncertain and preferences conflict. John von Neumann and Oskar Morgenstern's *Theory of Games and Economic Behavior* (1944) formalized utility and game theory. Richard Bellman's work on dynamic programming in the 1950s gave a way to plan sequences of decisions. Together these ideas became decision theory and Markov decision processes, the mathematical framework behind reinforcement learning.

### Neuroscience: the brain as an information processor

In 1943 Warren McCulloch and Walter Pitts published "A Logical Calculus of the Ideas Immanent in Nervous Activity", a simplified model of neurons as threshold units that can compute logical functions. It is generally treated as the first artificial neural network. Donald Hebb's *The Organization of Behavior* (1949) proposed that connections between neurons strengthen when they fire together, an early learning rule. Modern deep learning borrows the vocabulary of neurons and layers, though today's networks are far simpler than biological brains in some ways and far larger in others.

### Psychology: thinking as information processing

Behaviorism had treated the mind as a black box. Cognitive psychology, which grew in the 1950s alongside early AI, instead modeled thinking as the manipulation of internal representations. This "information processing" view gave AI its early research program: build programs that represent knowledge and reason over it, then compare their behavior with human problem solving.

### Computer engineering: the machine to run it on

AI needs hardware fast enough to run its algorithms. Stored-program electronic computers appeared in the late 1940s, and every major AI advance since has been tied to cheaper computation and memory. The deep learning breakthroughs of the 2010s depended on graphics processors (GPUs) that perform many matrix operations in parallel.

### Control theory and cybernetics: feedback and goals

Norbert Wiener's *Cybernetics* (1948) studied systems that use feedback to reach a goal, from thermostats to animals. Control theory contributed the idea of an agent minimizing an error or cost over time, which reappears in optimization, robotics and reinforcement learning.

### Linguistics: language as structure

Noam Chomsky's *Syntactic Structures* (1957) described language with formal generative grammars, and his 1959 review of B. F. Skinner's *Verbal Behavior* argued that behaviorist accounts could not explain how people produce sentences they have never heard. Natural language processing grew from the meeting of linguistics and AI, and today's large language models are the latest attempt to answer the question Chomsky raised: how a finite system can understand and produce unlimited new sentences.

## The founding papers and events

A handful of documents turned these scattered ideas into a field with a name:

| Year | Work | Why it matters |
| --- | --- | --- |
| 1943 | McCulloch and Pitts, "A Logical Calculus of the Ideas Immanent in Nervous Activity" | First mathematical model of a neural network |
| 1948 | Claude Shannon, "A Mathematical Theory of Communication" | Founded information theory; entropy and cross-entropy are still used to train models |
| 1950 | Alan Turing, "Computing Machinery and Intelligence" (*Mind*) | Opened with "Can machines think?" and proposed the imitation game, now called the Turing test |
| 1955 | McCarthy, Minsky, Rochester and Shannon, Dartmouth proposal | Coined the term "artificial intelligence" |
| 1956 | Dartmouth Summer Research Project | The workshop usually treated as the founding event of AI as a field |
| 1958 | Frank Rosenblatt, the perceptron | A neural network that learned its weights from examples |
| 1959 | Arthur Samuel, checkers program | Popularized the term "machine learning" with a program that improved by playing |

The Dartmouth proposal, dated August 31, 1955, stated the field's founding conjecture: that "every aspect of learning or any other feature of intelligence can in principle be so precisely described that a machine can be made to simulate it." The proposal listed language use, abstraction, neural nets, self-improvement and randomness as problems to study, which is still a recognizable map of AI research.

## How the field developed after the founding

AI has moved through several waves rather than a straight line:

1. **Symbolic AI (1950s to 1980s).** Programs searched through possible states and applied explicit rules. Early successes included the Logic Theorist (1956), which proved theorems from *Principia Mathematica*, and later the expert systems of the 1970s and 1980s.
2. **AI winters.** Promises outran results. Minsky and Papert's *Perceptrons* (1969) showed the limits of single-layer networks, and the UK's Lighthill report (1973) criticized the field's progress, contributing to funding cuts. A second downturn followed the collapse of the expert systems market in the late 1980s.
3. **Statistical and probabilistic AI (1980s to 2000s).** Judea Pearl's Bayesian networks gave a practical way to reason under uncertainty, and machine learning methods such as decision trees and support vector machines learned patterns from data instead of hand-written rules. In 1986, Rumelhart, Hinton and Williams popularized backpropagation for training multi-layer networks.
4. **Deep learning (2012 onward).** Large labeled datasets, GPUs and better training methods made deep neural networks practical. A convolutional network (AlexNet) won the 2012 ImageNet image recognition challenge by a wide margin, and the transformer architecture introduced in "Attention Is All You Need" (2017) became the basis of today's large language models.

The lesson repeated in every wave is that ideas often fail first for lack of data or computing power, then succeed decades later. Backpropagation and neural networks are the clearest example.

## The core concepts every AI system uses

Whatever the technique, most AI systems combine a few recurring ideas:

- **Agents and environments.** An agent perceives its environment and takes actions to achieve a goal. Framing a problem this way (what can it observe, what can it do, what counts as success) is the first step of any AI design.
- **Search.** Many problems, from route planning to game playing, are solved by exploring possible sequences of actions. Algorithms such as breadth-first search, A\* and minimax are the classical toolkit.
- **Knowledge representation and reasoning.** Logic, rules, semantic networks and knowledge graphs let a system store facts and derive new ones.
- **Reasoning under uncertainty.** Probability, Bayesian networks and Markov models let a system act sensibly when information is incomplete or noisy.
- **Learning.** Instead of being programmed with rules, the system improves its performance from data or experience. The three main paradigms (supervised, unsupervised and reinforcement learning) are covered in [Machine Learning](/en/docs/machine-learning).

## The mathematics behind modern AI

Four areas of mathematics make modern AI readable:

- **Linear algebra.** Data, images and words are stored as vectors and matrices, and a neural network layer is essentially a matrix multiplication followed by a simple non-linear function.
- **Probability and statistics.** These describe uncertainty, measure how well a model generalizes beyond its training data, and explain why a model can be confident and still wrong.
- **Calculus and optimization.** Training means minimizing a loss function. Gradient descent computes how the loss changes with each parameter and nudges the parameters downhill; backpropagation is the efficient way to compute those gradients in a network.
- **Information theory.** Shannon's entropy measures uncertainty. The cross-entropy loss used to train classifiers and language models comes directly from it.

These are not prerequisites to memorize in isolation. The same gradient-based optimization that trains a small classifier also trains a large language model, which is why these foundations stay useful as techniques change.

## Where to go next

- [Machine Learning](/en/docs/machine-learning) covers supervised, unsupervised and reinforcement learning.
- [Deep Learning](/en/docs/deep-learning) explains neural networks, backpropagation and transformers.
- [Generative AI](/en/docs/generative-ai) covers large language models and diffusion models.
- [AI Safety](/en/docs/safety) covers robustness, fairness, interpretability and alignment.

## Primary sources

- A. M. Turing, "Computing Machinery and Intelligence", *Mind* 59 (236), 1950.
- J. McCarthy, M. L. Minsky, N. Rochester, C. E. Shannon, "A Proposal for the Dartmouth Summer Research Project on Artificial Intelligence", August 31, 1955.
- W. S. McCulloch and W. Pitts, "A Logical Calculus of the Ideas Immanent in Nervous Activity", *Bulletin of Mathematical Biophysics* 5, 1943.
- C. E. Shannon, "A Mathematical Theory of Communication", *Bell System Technical Journal* 27, 1948.
- D. E. Rumelhart, G. E. Hinton, R. J. Williams, "Learning representations by back-propagating errors", *Nature* 323, 1986.
- A. Vaswani et al., "Attention Is All You Need", *Advances in Neural Information Processing Systems*, 2017.
- S. Russell and P. Norvig, *Artificial Intelligence: A Modern Approach*, chapter 1.
