# Induction-machine-parameters-without-testing
Finding parameters of induction machine without physical testing, using PSO algorithm

The parameter estimation methodology describes a method for estimating the steady state equivalent circuit parameters from the motor performance characteristics, which is normally available from the nameplate data or experimental tests. This method is used to estimate the stator and rotor resistances, the stator and rotor leakage reactances, and the magnetizing reactance in the steady- state equivalent circuit. The validity of the method is demonstrated for a present model of induction motor in MATLAB.

An induction motor can be modelled by using a steady state equivalent circuit. The parameter estimation problem is formulated as a least squares optimization problem so that the objective function is the minimization of the deviation between the estimated and the nameplate data.
The problem formulation uses the manufacturer data, such as the starting torque, the full load torque, the maximum torque, and the full load power factor. The method is used to estimate the stator and rotor resistances, the stator and rotor leakage reactances, and the magnetizing reactance in the steady-state equivalent circuit of the motor. The rotor parameters have been referred to as the stator side. Also, it is assumed that the core-losses are negligible.
 
The problem formulation and objective function are as follows:







where 𝑅𝑠 is the stator resistance; 𝑅’𝑟 is the rotor resistance which has been referred to as the stator side; 𝑋𝑠 is the stator leakage reactance; 𝑋’𝑟 is the rotor leakage reactance which has been referred to as the stator side; 𝑋𝑚 is the magnetizing reactance; and 𝑠 is the slip. Also, it is assumed that 𝑋𝑠 is equal to 𝑋’𝑟. The other variables are introduced as follows:


where 𝑉ph is input phase voltage; 𝑉th is Thevenin voltage; ´ 𝑅th and 𝑋th are Thevenin resistance and Th´evenin reactance, ´ respectively; 𝜔𝑠 is angular velocity; and 𝐾𝑡 is the constant coefficient. Also, “mf ” index is used for the manufacturer data so that 𝑇st(mf), 𝑇fl(mf), and 𝑇max(mf) are the manufacturer values of the starting torque, full load torque, and maximum torque, respectively. Also, 𝑓1, 𝑓2, and 𝑓3 are error between the calculated and manufacturer value of the full load torque, starting torque, and maximum torque, respectively. Also, 𝑓4 is error between the calculated and manufacturer value of the full load power factor.
The objective function using aforementioned equations is defined as follows:
 

