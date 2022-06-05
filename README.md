# AGFeatureSelection
Feature Selection using genetic algorithms 

The Genetic Algorithm(GA) is an evolutionary algorithm(EA) inspired by Charles Darwin’s theory of natural selection which espouses Survival of the fittest. As per the natural selection theory, the fittest individuals are selected to produce offsprings. The fittest parents' characteristics are then passed on to their offsprings using cross-over and mutation to ensure better chances of survival. Genetic algorithms are randomized search algorithms that generate high-quality optimization solutions by imitating the biologically inspired natural selection process such as selection, cross-over, and mutation.
Population contains a set of possible solutions for the stochastic search process to begin. GA will iterate over multiple generations till it finds an acceptable and optimized solution. First-generation is randomly generated.
Chromosome represents one candidate solution present in the generation or population. A chromosome is also referred to as a Genotype. A chromosome is composed of Genes that contain the value for the optimal variables.
Phenotype is the decoded parameter list for the genotype that is processed by the Genetic Algorithm. Mapping is applied to the genotype to convert to a phenotype.
The Fitness function or the objective function evaluates the individual solution or phenotypes for every generation to identify the fittest members.
Different Genetic Operators
Selection is the process of selecting the fittest solution from a population, and then the fittest solutions act as parents of the next generation of solutions. This allows the next generation to inherit the strong features naturally. Selection can be performed using Roulette Wheel Selection or Ranked Selection based on the fitness value.
Cross-over or recombination happens when genes from the two fittest parents are randomly exchanged to form a new genotype or solution. Cross over can be a One-point cross over or Multi-Point Cross over based on the parent's segments of genes exchanged.
Usage of Genetic Algorithm in Artificial Intelligence

A Genetic Algorithm is used for Search and Optimization using an iterative process to arrive at the best solution out of multiple solutions.
1. A Genetic Algorithm can find an appropriate set of hyperparameters and their values for a deep learning model to increase its performance in Deep Learning.
2. A Genetic Algorithm can also be used to determine the best amount of features to include in a machine learning model for predicting the target variable.
Function Description

1. split():
Splits the dataset into training and test set.

2. acc_score():
Returns accuracy for all the classifiers.

3. plot():
For plotting the results.
Function Description for Genetic Algorithm

1. initilization_of_population():
To initialize a random population.

2. fitness_score():
Returns the best parents along with their score.

3. selection():
Selection of the best parents.

4. crossover():
Picks half of the first parent and half of the second parent.

5. mutation():
Randomly flips selected bits from the crossover child.

6. generations():
Executes all the above functions for the specified number of generations

Implementation of Genetic Algorithm for Feature Selection
First, we run a function to initialize a random population.
The randomized population is now run through the fitness function, which returns the best parents (highest accuracy).
Selection from these best parents will occur depending on the n-parent parameter.
After doing the same, it will be put through the crossover and mutation functions respectively.
Cross over is created by combining genes from the two fittest parents by randomly picking a part of the first parent and a part of the second parent.
The mutation is achieved by randomly flipping selected bits for the crossover child.
A new generation is created by selecting the fittest parents from the previous generation and applying cross-over and mutation.
This process is repeated for n number of generations.
