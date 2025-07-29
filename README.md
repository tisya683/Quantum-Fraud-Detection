# Introduction to Quantum Inspired Mean Field Probabilistic Model (QIMF)

In this day and age, where hackers are getting more advanced and cash payments are on the decline, fraud detection systems need to move beyond the assumption that each transaction is i.i.d. and should instead model interactions between transactions.
This means that the fraud label for each transaction should depend on the labels of other transactions in the dataset, rather than being decided in isolation. This way, we can detect complex fraud patterns that would be missed if transactions were looked at individually.

For this, we can use the Quadratic Unconstrained Binary Optimization (QUBO) model. What this model does is assign either a 0 or 1 to each transaction. These 0s and 1s aren't the actual labels but represent the model's best guesses based on how all the transactions relate to each other. The goal is to find the most optimal combination of 0s and 1s that best fits the overall structure of the data and minimises the cost function. Since these are hard binary values, this task is deemed NP-hard and requires extensive computational resources.

However, QIMF overcomes this limitation by converting the binary selection of 0 or 1 into continuous probabilistic values between 0 and 1. This allows us to use gradient descent to optimise the model and improve its guesses over time. QIMF draws from mean field theory to calculate the probabilities and uses a quantum-inspired cost function based on the Ising Model. This allows us to model complex relationships between transactions while keeping the computation manageable.

Full disclaimer: I only came across the concepts of QUBO and QIMF from the research paper “Quantum-Inspired Mean Field Probabilistic Model for Combinatorial Optimization Problems” (1 June 2024, arxiv.org/html/2406.03502v1) by authors Yuhan Huang, Siyuan Jin, Yichi Zhang, Ling Pan, and Qiming Shao.
