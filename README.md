

A code repository accompanying the paper (1697)


**Highlights of the attack**:
- 100% evasion rate on 10K MNIST images using 12 queries on average!
- 90% evasion rate against Ensemble Adv. trained model for IMANGENET with 1000 queries!
- 2.5x fewer queries and 3.8x less failure-prone that SOTAs combined on MNIST, CIFAR10, & IMAGENET.
- Theoretically guaranteed to perform at least as well as FGSM after 2^(log(n)+1) queries.
- Surpasses all the transfer-only zero-query attacks on Madry's Lab's challenges and is comparable with PGD using the same number of iterations with the difference that PGD uses X backprops, while SignHunter uses X forwards.


### Repository Structure

The repository is of the following structure:
- `src/`: contains the code for reproducing our work.
- `data/`: a placeholder for the data files that were used to generate our figures. These can be downloaded from the shared data link. In addition to the data, this directory should also contains MNIST, CIFAR10, and IMAGENET models. 

Refer to the directories above for code & data setups. To get started, follow the step A & B of **Setup** in `src/README.MD`, then the instructions in `data/README.MD`. With this, you are set to follow the steps of **Experiments** in `src/README.MD`.

Also, the repository has two branches:
- `master`: contains the code for the main experiments in the paper.
- `challenges`: for experiments of Section 5. 

