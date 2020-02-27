# Deutsch-Josza Algorithm
My goal with this repository is to describe one of the projects that I have been working out and successfully replicated call the
Deutsch-Joza algorithm. This was one of the first projects that I worked on after starting my focus on quantum computers. The Deutsch
Jozsa algorithm is one of the most basic but genius examples leveraging quantum technology to manufacture a computational speed up.
Using the IBM Qiskit interface, I was able to replicate the circuit that would be used to create the quantum speed up proposed by David
Deutsch and Richard Jozsa in 1992. Within the article, I wrote about this project and how the math behind it works. I also went into
depth about some quantum computational ideas like gates and how the quantum computers are actually speeding up the processes to display
the ideas of supremacy.

On this page, I want to try to explain some of the logic I used to code this project.

The projects focus is to solve a problem proposed by these two scientists that basically described a situation where there are two types of black box funcitons. With this in mind, your goal is to try to query the black box (this means you don't know what it does) function the least amount of times as possible and find out if the function is a balanced funciton or a constant function.

What we need: We need to find out whether the function is constant or balanced. A constant function has two subsets, a function in which no matter the input, the output is 1 or 0. The first type of constant function is the 1 function. If you put in a {1, 0}, you would receive a {1, 1}. The second type of constant function is the 0 function. If you put in a {1, 0}, you would receive a {0, 0}. A balanced function has two subsets as well, both of which depend on the input. The first type of balanced function is the identity function. If you put in a {1, 0}, you would receive a {1, 0}. Your outputs are the same values as your inputs. The second subset of balanced functions is the “NOT” function. If you put in a {1, 0}, you would receive a {0, 1}. Your outputs are the opposite values of your inputs.

In the case of my implimentation, I created specific names for each of these seperate cases. The constant case where the outputs are in the 0 state is created by the command constant0. The user can choose which case they want by just changing the function name at the top of the code to change the type of blackbox function. Depending on the type of function that is called, there are different gates that are applied to the circuit to replicate how this black box would normally react.
