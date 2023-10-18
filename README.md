# HEMT_Simulation-Optimization
This is a repository for my B-Tech final year project


**Abstract**

This report offers an extensive exploration of High Electron Mobility Transistors (HEMTs) with a
particular focus on the fundamental principle governing their operation—the formation of a two-dimensional electron gas (2DEG). HEMTs, composed of Group III-nitride materials, play a pivotal
role in high-power RF and microwave applications. The unique characteristic of HEMTs lies in
the creation of a 2DEG at the heterointerface, which is accomplished by strategically designing the
semiconductor layers with varying band gaps. By engineering the layers to have distinct bandgap
energies, a potential energy step is established at the heterointerface. This energy discontinuity
confines electrons within a two-dimensional plane, creating the 2DEG. The report introduces an
innovative simulation system employing Kronecker matrices with convolution-based interpolation
to solve the Poisson and Schrodinger equations self-consistently. This system offers comprehensive insights into electron wave functions, electric potential distribution, electron density, Fermi
surface energy, and current density distribution throughout the HEMT device. This research significantly advances our understanding and optimization of HEMTs for advanced nanoscale electronic
applications.

**Outputs Till Midsem**


Basically, working with the intrinsic characteristics of Al(0.3)Ga(0.7)N-GaN HEMT. x>0.3 proves to be very dodgy. Will extend it to incorporate doping profiles later.
Need to develop GUI now and incorporate Greens quation to incorporate quantum effects. So far the simulation is totally based on consistently solving Schrodingers Eqn, Posissons Equation and then updating the values obtained with the fermi Dirac distribution to obtain the density of electrons. Note. it is extremely difficult to converge the outputs. Had to use GPU for the simulation and developed a Kronecker + conv (yes I work in ML) based interpolation method to get consistent outputs. RMSE curve proves that the solution obtained is not random. (Do incorporate Dirichlet and Neumann boundary conditions else it wont converge)

![image](https://github.com/Sourjya261/HEMT_Simulation-Optimization/assets/89221563/d3c06078-afc7-46b7-be38-e32dd8865a1d)
![image](https://github.com/Sourjya261/HEMT_Simulation-Optimization/assets/89221563/fd2ef393-7c32-4ba5-935d-872e3be79d6f)
![image](https://github.com/Sourjya261/HEMT_Simulation-Optimization/assets/89221563/fa1a8418-4c8c-495e-9249-4f944dd4d85c)

![image](https://github.com/Sourjya261/HEMT_Simulation-Optimization/assets/89221563/321ec771-daaa-4db6-89e8-f4e6a0aec561)
![image](https://github.com/Sourjya261/HEMT_Simulation-Optimization/assets/89221563/fe5392e1-0a64-4d37-9ff6-7dcc6546f0f1)



