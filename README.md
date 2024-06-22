Facility Location Optimization Project

Overview
This project focuses on optimizing the placement of ATMs to maximize accessibility for clients using various optimization algorithms. The problem is formulated as a Quadratic Unconstrained Binary Optimization (QUBO) and solved using different solvers like ExactSolver, SimulatedAnnealing, DWaveSampler, CQM, and QAOA.

Features
Random Position Assignment: Assigns random geographic positions to ATMs and clients.
Profit Calculation: Assigns profits to clients based on a normal distribution.
QUBO Matrix Construction: Constructs a QUBO matrix for optimization.
Distance Calculations: Computes Euclidean distances between ATMs and clients.
Solver Implementations: Implements several solvers to find the optimal placement of ATMs.
Plotting: Visualizes the distribution of ATMs and clients, and the optimal ATM locations.
Usage
Function: FacilityLocation
Parameters:

n_atms: Number of ATMs
n_clients: Number of clients
radio_clients: Radius of client influence
radio_atms: Radius of ATM influence
solver: Solver type (ExactSolver, SimulatedAnnealing, DWaveSampler, CQM, QAOA)
lambda1: Constraint strength parameter 1
lambda2: Constraint strength parameter 2
p: Parameter for QAOA (default is 1)
Returns:

Distances between clients and ATMs
Distances between ATMs
Solution details
Optimal ATM locations
Profits
Running the Function
Example:

python
Copy code
result = FacilityLocation(19, 1000, 0.20, 0.7, 'ExactSolver', 1, 5)