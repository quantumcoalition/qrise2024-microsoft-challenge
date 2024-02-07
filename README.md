# Microsoft Quantum research challenge at QRISE 2024: Resource estimation of quantum algorithms 

## Challenge overview

In this research challenge you will implement one or several quantum algorithms and obtain and analyze the estimates of resources required for running them on fault tolerant quantum computers. 

## Background: quantum resource estimation

Quantum resource estimation is the area of quantum information science that aims to answer the question “How many physical qubits and how much time is necessary to execute a quantum algorithm under specific assumptions about the hardware platform used?” The estimates of the answers are done under realistic assumptions about architecture of fault tolerant quantum computers, such as physical qubit parameters and error correction schemes used. 

Getting these kinds of resource estimates serves at least three purposes. First, we can use it to deduce the conditions that quantum hardware needs to meet to offer practical quantum advantage. Second, resource estimation clarifies which algorithms truly give quantum advantage over their classical counterparts, and which ones do not. Third, it allows us to compare the efficiency of different algorithms that solve the same problem long before they become viable to run on quantum machines. Being able to answer such questions gives us essential information for defining our vision for the future of quantum computing. 

## Challenge details 

In this challenge, you will obtain resource estimates for a quantum algorithm of your choice. 

* Choose a quantum algorithm (for example, quantum state preparation, arbitrary unitary implementation, reversible quantum computing algorithms such as integer comparison or arithmetic, Grover’s search for solving a specific problem, qRAM, etc.) to explore. 

* Implement it in Q# (you can use Python as a classical host for your Q# code, for example, to run simulation on small instances of the problem, and to analyze the resource estimates). 

* Get the resource estimates for your implementation using Azure Quantum Resource Estimator. 

* Keep exploring! 
  - If you've implemented an algorithm described in a paper that includes the analysis of logical resource counts, compare the logical resource estimates produced by Azure Quantum Resource Estimator with the numbers obtained theoretically.

  - Obtain the resource estimates for using the algorithm for solving the problem for increasing input sizes. 

  - Compare resource requirements for running the algorithm under different assumptions about the parameters of the hardware platform it could run on, using different error correction schemes, and so on. 

  - Compare efficiency of different implementations of the same algorithm. 

## Submission criteria

Submit a GitHub repository with complete Q# and Python code for your project and a write-up of your results, which includes a brief description of the algorithm/primitive you chose, the problem instances on which you verified the correctness of your solution, the resource estimates you obtained, and your analysis of the estimates. 

## Useful resources

### Azure Quantum Development Kit and Resource Estimator documentation

* [Set up Azure Quantum Development Kit](https://learn.microsoft.com/azure/quantum/install-overview-qdk) (we recommend setting up Visual Studio Code on your machine and using Python to analyze the resource estimates you get for your Q# code) 

* [Introduction to Resource Estimator](https://learn.microsoft.com/azure/quantum/intro-to-resource-estimation) (official documentation) 

* [Resource estimation samples](https://github.com/microsoft/qsharp/tree/main/samples/estimation) (GitHub repo) 

* [Assessing requirements to scale to practical quantum advantage](https://arxiv.org/abs/2211.07629) (details the theoretical background for Azure Quantum Resource Estimator) 

* [Using Azure Quantum Resource Estimator for Assessing Performance of Fault Tolerant Quantum Computation](https://arxiv.org/abs/2311.05801) 


### Examples of papers that use automatic tools for quantum resource estimation: 

* [Resource Estimation of Quantum Multiplication Algorithms](https://arxiv.org/abs/2402.01891)

* [Implementing Grover oracles for quantum key search on AES and LowMC](https://arxiv.org/abs/1910.01700)

* [Towards efficient automatic oracle synthesis and resource estimation using QDK and QIR](https://ieeexplore.ieee.org/document/10313630)

