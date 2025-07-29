# Introduction to Quantum Inspired Mean Field Probabilistic Model (QIMF)

In this day and age, where hackers are getting more advanced and cash payment is on the decline, fraud detection systems need to move past beyond assuming that each transaction is i.i.d and should instead model interactions between transactions. 
This means that the fraud label for each transaction should depend on the labels of other transactions in the dataset, rather than being decided in isolation.. This way, we can detect complex fraud patterns that would be missed if you look at transactions individually.

For this we can use the Quadratic Binary Optimisation (QUBO) model. What this model does is to assign either a 0 or 1 to each transaction.These 0s and 1s aren't the actual labels but represent the model's best guesses based on how all the transactions relate to each other.The goal is to find the most optimal combination of 0s and 1s that best fit the overall structure of data and minimises the cost function.Since these are hard binary values, this task is deemed NP-hard and requires extensive computational resources.

However QIMF overcomes this limitation by converting the binary selection od 0 or 1 into continuous probabilistic domains between 0 to 1. This would allow us to use gradent descent to then optimise the model and improve its guesses over time. QIMF draws from mean field theory to calculate the probabilities and a quantum-inspired cost function based on the Ising Model.This allows to model complex realationships between transactions while keeping the computation manageable.


Full disclaimer: I only read came across the concepts of QUBO and QIMF from the research paper “Quantum-Inspired Mean Field Probabilistic Model for Combinatorial Optimization Problems, 1 June 2024, arxiv.org/html/2406.03502v1. " by authors Yuhan Huang,Siyuan Jin, Yichi Zhang,Ling Pan and Qiming Shao. 
