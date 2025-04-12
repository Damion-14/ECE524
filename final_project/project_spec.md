# Project Specification: Optimize Compute Resources

## 1. Issue Being Addressed
The project focuses on addressing the complexities of compute infrastructure. The main objective is to design an optimal layout for compute resources. This involves:
- Determining the best combination of compute modules to meet various hosting requirements.
- Balancing resource constraints (e.g., power, performance, uptime) against the needs of hosted services.

## 2. Data Collection and Sources
**Data Origin:**  
The data will be derived from performance tests conducted on specific hardware. The focus will be on:
- Hardware resource limits (e.g., processing power, memory)
- Uptimes and reliability measures
- Power consumption under different loads

**Scope:**  
- Concentrate on a limited group of compute resources, such as Raspberry Pi devices or other well known computers.  
- Ensure tests replicate realistic operating conditions to model behavior under typical workloads.

## 3. Underlying Optimization Problem
**Problem Statement:**  
Determine the optimal number and configuration of compute modules that can satisfy hosting requirements. This problem is characterized by:
- **Resource Allocation:** Balancing compute capacity, storage, and network throughput.
- **Constraint Management:** Each service has specific requirements (e.g., number of websites, required storage per service, user load, and necessary uptime).
- **Decision Variables:** 
  - The number of compute modules.
  - The allocation of services to available hardware resources. (possibly remove this, we can think of the system as more fulid where services can be migrated from one computer to another)
- **Objective:**  
  Minimize costs and maximize efficiency and minimize power consumption subject to the constraints provided by performance, capacity, and reliability requirements.

## 4. Anticipated Challenges
- **Hardware Variability:** Obtaining reliable and reproducible performance limits from different compute resources.
- **Data Translation:** Accurately converting service requirements (like the number of users or data storage needs) into quantitative processing or compute demand.
- **Scalability:** Ensuring that the optimization model can accommodate changes in service requirements or hardware capabilities over time.

## 5. Points for Consideration and Feedback Questions
- **Detail needed:** This specification presents a high-level outline to define the project's direction. As the project develops, additional parameters such as cost per compute unit, detailed power profiles, thermal constraints, network latency, and redundancy strategies would be incorporated into the model.
- **Scope:** Is this in scope of what we have learned in class and what methods would you like to see used to solve this problem?