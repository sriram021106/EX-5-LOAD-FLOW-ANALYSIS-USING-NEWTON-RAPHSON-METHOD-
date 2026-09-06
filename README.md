# EX-5-LOAD-FLOW-ANALYSIS-USING-NEWTON-RAPHSON-METHOD-
# AIM: 
To carry out the load flow analysis for the given network by Newton-Raphson method. 

# SOFTWARE REQUIRED: 
ETAP Software. 

# THEORY: 
# POWER FLOW SOLUTION: 
Consider the network equation Ip= YpqVq in an expanded form as 
<img width="681" height="437" alt="5PSA1IMG" src="https://github.com/user-attachments/assets/a4df9569-22c3-4071-808c-32ecc6df5ecf" />

NEWTON-RAPHSON METHOD: 
In this method mismatch version is widely used for the power flow problem. In this version we denote, 
<img width="858" height="312" alt="5PSAIMG2" src="https://github.com/user-attachments/assets/53188185-c9df-454c-96f6-acc01c86211c" />

In the n total number of nodes, let the number of P-Q nodes be (n1), P-V nodes be (n2) and let there be 
one slack bus so that 
                            nb= n1+n2+1. 
Our basic problem is to find the unknown voltage magnitudes (|V|) at the P-Q buses and 
angles ‘δ’ at the P-Q and P-V buses. 
Let x be the vector of all, unknown |V| and δm and Y the vector of specified variables. The dimension of x 
is n1+2n2+2. Thus,
<img width="430" height="468" alt="5PSA3IMG" src="https://github.com/user-attachments/assets/46bf3826-8430-4676-8fc3-e03953895056" />

From the set of equations (5) and (6) we select a number of equations equal to the number of unknowns in 
X to form the non-linear power flow equation F(X,Y) = 0. Since Y is specified we may suppress it from the 
equations. 
<img width="702" height="420" alt="5PSA4IMG" src="https://github.com/user-attachments/assets/8a73275d-5f6b-4dad-be3c-96f0eea3275d" />
<img width="1022" height="655" alt="5PSAIMG5" src="https://github.com/user-attachments/assets/87a96cd2-da7a-48b8-8d72-d37f54ec2317" />
# ALGORITHM: 
1. Form the [Y-Bus]. 
2. Initialize bus voltage and angles. 
3. Calculate mismatch real power [∆P] of all buses except slack bus. 
4. Calculate mismatch reactive power [∆Q] for all load buses. 
5. Check for convergence (i.e., whether all values of mismatch vector are within tolerance 
limits). If converged, go to step 9. 
6. Form the Jacobian matrix. 
7. Solve the equation (8) for [∆δ] and [∆V] and update the vectors [δ] and [V]. 
8. Go to step (3). 
9. Calculate all the line flows, slack bus power, line losses and reactive power generations at 
other generator buses and print the results.
# CIRCUIT DIAGRAM:
<img width="1206" height="774" alt="WhatsApp Image 2026-06-07 at 1 11 52 PM" src="https://github.com/user-attachments/assets/8dcde59c-6501-427e-b154-98709801b997" />

# OUTPUT:
<img width="1206" height="765" alt="WhatsApp Image 2026-06-07 at 1 12 10 PM" src="https://github.com/user-attachments/assets/3dd0d08a-0081-4f77-85be-86e2a5b21e46" />

# RESULT:
Thus,To carry out the load flow analysis for the given network by Newton-Raphson method 
Is successfully done using an etap software and the ouput is obtained.
