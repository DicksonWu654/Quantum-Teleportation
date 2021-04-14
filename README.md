# Quantum-Teleportation

Hi There! 👋<br/>
This is a repo where you have access to all the Jupiter Notebooks, along with some resources that made it all possible!<br/>

## Table of Contents
* [Quantum Teleportation?](#Quantum-Teleportation?)
* [Diabetic Retinopathy](#Diabetic-Retinopathy)
* [Acknowledgements](#Acknowledgements)
* [Connect with me](#Connect-with-me)

## Quantum Teleportation?

### TL;DR 
Straight off the bat: quantum teleportation isn't really teleportation. What happens is the state of the qubit is transferred to another qubit. To understand let's run through a scenario. 

Let's say we have 2 labs: Lab A and Lab B. Lab A has a qubit that they want to transfer to Lab B. Lab A has no idea what state the mysterious qubit is in. So how do we do it?

One option would be to physically transfer the qubit. But that's boring! We want to do cool things so we'll move on. Another proposal would be to try and measure the state of the qubit - but that's not possible too because of the no-cloning theorem! 

What do we do?

Quantum Teleportation!

### A Longer Explanation:

<p align="center">
<img src="circuit.png" width="350"/><br/>
Credit: Quantum.Country
</p>

Now it might look a bit complicated, but if you think about it, with only 3 qubits and 6 gates we can perform quantum teleportation! 

Part of the Circuit
- The first 2 lanes are Lab A
- The last lane is Lab B
- The very first lane is the qubit that we'll be teleporting

How the Circuit Works
- An entangled pair of qubits (Qubit 2 and 3) are sent to each lab
- A CNOT gate has a target of Qubit 2 with a control of Qubit 1
- A Hadamard gate is applied to Qubit 1
- Qubit 1 and 2 are measured. With a z gate and x gate respectively
- At this moment, Qubit 3 becomes Qubit 1 (but we need to modify it a bit)
- Depending on the outputs of Qubit 1 and 2, we rotate Qubit 3
- Success! The qubit is successfully teleported!

Alright! We just performed quantum teleportation. Now the reason why it's teleported at step 5 is that Qubit 2 and 3 are entangled. But if that answer isn't satisfactory enough, you can go into the mathematical proof and intuition in [my article](https://dickson-wu.medium.com/beam-me-up-scotty-2de01834be0c)! Also check out my [Video!](https://youtu.be/Rffi7-7zjLc)

## Acknowledgements

* [Resource to help me Code](https://qiskit.org/textbook/ch-algorithms/teleportation.html)
* [Excellent Essay Explaining Quantum Teleportation](https://quantum.country/teleportation)
* [Paper on it's Applications](https://iopscience.iop.org/article/10.1088/1742-6596/1634/1/012089/pdf)

## Connect with me

If you want to follow along on my journey, you can join my [monthly newsletter](https://www.subscribepage.com/g1p8w4), check out my [website](https://dicksonwu654.github.io/), and connect on [Linkedin](https://www.linkedin.com/in/real-dickson-wu/) or [Twitter](https://twitter.com/DicksonWu3) 😃
