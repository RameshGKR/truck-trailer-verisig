# Formal verification of autonomous truck-trailer maneuvering using Verisig

This repository contains the implementation of a hybrid automaton model of a truck-trailer system and its verification using the **Verisig** tool. The project explores formal verification techniques to ensure the safety of the truck-trailer system, using a deep neural network (DNN) to mimic the Model Predictive Control (MPC) behavior within the hybrid automaton.

## Project Goals

1. **Model a Hybrid Automaton**:
   - Develop a hybrid automaton for the truck-trailer system, including modes and transitions.

2. **DNN as a Controller**:
   - Train a DNN to approximate the MPC and integrate it into the hybrid automaton.

3. **Verification using Verisig**:
   - Perform reachability analysis and safety verification using Verisig to ensure the truck-trailer adheres to safety constraints.

4. **Documentation of the Optimal Control Problem (OCP)**:
   - Describe the OCP and its modeling within the hybrid automaton framework.

### **Key Files**
- **`automaton/D.cfg`**: Configuration file for Verisig that specifies system parameters and analysis configurations.
- **`automaton/D.model`**: Flow* model file that represents the dynamics of the truck-trailer system.
- **`automaton/D.xml`**: Hybrid automaton model in XML format, detailing system modes, transitions, and invariants.
- **`automaton/DNN_truck_trailer.yml`**: Serialized DNN model trained to mimic the MPC behavior.

---
## Links
- **DNN Training Repository**: The repository for training the DNN controller can be found here: [DNN_truck_trailer](https://github.com/RameshGKR/DNN_truck_trailer).
- **Write-Up**: The detailed project write-up is available on Overleaf: [Project Write-Up](https://www.overleaf.com/project/66436a0ceb9f1831561bd728).

## Tools and Dependencies

### **1. Verisig**
- Verisig is a tool for verifying hybrid automata with neural network controllers. It uses Flow* for reachability analysis and supports DNN-based control systems.

### **2. Flow***
- Flow* is used by Verisig to perform reachability analysis for nonlinear hybrid systems.




## Acknowledgments

This project uses the following tools:
- [Verisig](https://github.com/verisig)
- [Flow*](http://flowstar.org)
