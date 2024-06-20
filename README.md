# Grover-s-Alogo-
This contains code and readme file for a project factorisation using Grover's algorithm.


Implementing a quantum algorithm for integer factorization using PennyLane. Below is an explanation of the code:

Add_k_fourier:This function is for adding a Fourier series component.
Multiplication: This function should perform the multiplication operation in the quantum domain. It uses Quantum Fourier Transform (QFT) for addition in the quantum circuit.
What it essentially does is compute the 'classical product' of qubits.


Then the code calculates the number of iterations for the quantum algorithm, which is typically related to the square root of the input number.

The factorization function is the main quantum circuit. It initializes the qubits in superposition and then iterates over a sequence of operations that include the multiplication,changing the sign of amplitude, and Grover's operator which is a diffusion operator which amplifies the probability of our factors(p and q).
The function returns the array of probabilities.

After this the execution the code draws the quantum circuit using PennyLane's drawing capabilities.

Then the next section attempts to find the factors of N by identifying the peaks in the probability distribution returned by the quantum circuit This is achieved using numpy's argmax function, which returns the position of the element having the largest probabilities.Which are in turn the factos of the input biprime number. 


References 
1)https://pennylane.ai/qml/demos/tutorial_qft_arithmetics/

2)https://youtu.be/tsbCSkvHhMo?feature=shared

3)https://youtu.be/EoH3JeqA55A?feature=shared

4)https://youtu.be/YEI5vYdcoQ4?feature=shared