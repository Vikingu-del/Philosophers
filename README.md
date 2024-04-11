# Philosophers: I never thought philosophy would be so deadly

## Summary

In this project, you will delve into the implementation of the dining philosophers problem in C, a classic synchronization challenge in computer science. You will learn the fundamentals of threading and mutexes, essential concepts for managing synchronization and concurrency in multi-threaded applications. Through the exploration of various solutions, algorithms, and implementations, you will gain hands-on experience in tackling the complexities of resource allocation and coordination in concurrent systems.


## Contents
- [Introduction](#introduction)
- [Common Instructions](#common-instructions)
- [Overview](#overview)
- [Mandatory Part](#mandatory-part)
- [Bonus Part](#bonus-part)
- [License](#license)

## Introduction
Philosophy, derived from the Greek word 'philosophia,' meaning "love of wisdom," explores fundamental questions about existence, knowledge, values, reason, mind, and language. Philosophical methods involve questioning, critical discussion, rational argument, and systematic presentation. This project delves into the dining philosophers problem, a classic synchronization problem in computer science.

## Common Instructions
- The project must be written in C.
- It must adhere to the Norm, including bonus files/functions.
- Functions should not quit unexpectedly, except for undefined behaviors.
- Heap allocated memory space must be properly freed to avoid leaks.
- If specified, a Makefile must be submitted with required flags and rules.
- Bonuses must be included separately from the main project.
- Libft usage is authorized if specified.
- Test programs are encouraged for self-evaluation and defense.

## Overview
The project simulates philosophers sitting at a round table, alternately eating, thinking, or sleeping. Each philosopher requires two forks to eat, with as many forks as philosophers present. Philosophers interact without speaking and are unaware of each other's status. The simulation stops when a philosopher dies of starvation.

## Mandatory Part
- Program Name: philo
- Turn-in Files: Makefile, *.h, *.c in the philo/ directory
- Arguments: number_of_philosophers time_to_die time_to_eat time_to_sleep [number_of_times_each_philosopher_must_eat]
- External Functions: pthread functions
- Description: Philosophers with threads and mutexes
- Specific Rules: Each philosopher is a thread; forks are protected with mutexes.

## Bonus Part
- Program Name: philo_bonus
- Turn-in Files: Makefile, *.h, *.c in the philo_bonus/ directory
- Arguments: Same as the mandatory program
- External Functions: pthread and semaphore functions
- Description: Philosophers with processes and semaphores
- Specific Rules: Forks are placed in the middle of the table and represented by a semaphore; each philosopher is a process.

## Usage
- Clone the repo: git clone \<repository url\>
- Run Mandatory Part
    1. Navigate to philo and type make
    2. ./philo \<number of philos\> \<time to die\> \<time to eat\> \<time to sleap\> and optional \<num of times each philo must eat\>
    3. Example: ./philo 5 800 200 200 || ./philo 5 800 200 200 7 (7 is the optional arguments which each philo must eat)
- Run Bonus Part
    1. Navigate to philo_bonus and type make
    2. type ./philo \<number of philos\> \<time to die\> \<time to eat\> \<time to sleap\> and optional \<num of times each philo must eat\>
    3. Example: ./philo 5 800 200 200 || ./philo 5 800 200 200 7 (7 is the optional arguments which each philo must eat)

## License

This project is licensed under the [MIT License](LICENSE).
