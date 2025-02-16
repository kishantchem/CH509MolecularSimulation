# The Boltzmann Distribution and Microstates of a Reservoir

## Fundamental Assumption of Statistical Mechanics  

The **fundamental assumption of statistical mechanics** states:  

> *In an isolated system at equilibrium, all accessible microstates are equally probable.*

This means that the probability of a system being in a particular state is proportional to the **number of microstates available to the surrounding reservoir**.

---

## Example: Two-State System in Contact with a Large Reservoir

### System & Reservoir Setup
Consider a **small system** (\( S \)) in thermal contact with a **large heat reservoir** (\( R \)). The **total energy** is fixed:

\[
E_{\text{total}} = E_S + E_R
\]

The system (\( S \)) can exist in **two states**:
- **State 1**: \( E_S = 0 \)  
- **State 2**: \( E_S = \Delta E \)  

Since the **total energy is constant**, if the system is in state 2 with energy \( \Delta E \), the reservoir must have energy:

\[
E_R = E_{\text{total}} - \Delta E
\]

whereas in state 1:

\[
E_R = E_{\text{total}}
\]

### Microstates & Probability Connection  

Let \( \Omega_R(E) \) be the **number of microstates** available to the reservoir at energy \( E \). The **probability** of the system being in a particular state is proportional to \( \Omega_R(E_R) \):

\[
P_1 \propto \Omega_R(E_{\text{total}})
\]

\[
P_2 \propto \Omega_R(E_{\text{total}} - \Delta E)
\]

Since entropy is related to the number of microstates via:

\[
S_R = k_B \ln \Omega_R
\]

we rewrite the probabilities as:

\[
P_1 \propto e^{S_R(E_{\text{total}}) / k_B}
\]

\[
P_2 \propto e^{S_R(E_{\text{total}} - \Delta E) / k_B}
\]

Using the **Taylor expansion**:

\[
S_R(E_{\text{total}} - \Delta E) \approx S_R(E_{\text{total}}) - \frac{\Delta E}{T}
\]

we get:

\[
P_2 \propto e^{(S_R(E_{\text{total}}) - \Delta E / T) / k_B}
\]

\[
P_2 \propto e^{S_R(E_{\text{total}}) / k_B} e^{-\Delta E / k_B T}
\]

Since \( e^{S_R(E_{\text{total}}) / k_B} \) is a constant that normalizes probabilities, we obtain:

\[
\frac{P_2}{P_1} = e^{-\Delta E / k_B T}
\]

This is the **Boltzmann factor**, showing that **higher-energy states are exponentially less probable than lower-energy states**.

---

## Physical Interpretation
- The probability of a system being in a particular energy state depends on the **number of microstates available to the reservoir**.
- A **lower system energy** means the **reservoir has more available microstates**, making that state **more probable**.
- A **higher system energy** means the **reservoir has fewer available microstates**, making that state **less probable**.
- The reservoir acts as a **thermostat**, ensuring energy is distributed according to the **Boltzmann distribution**.

---

## Key Takeaways
✅ **Probability is proportional to the number of reservoir microstates**.  
✅ **Lower-energy states are more probable because they leave more microstates for the reservoir**.  
✅ **This assumption leads directly to the Boltzmann distribution**.  

---

### **Further Reading**
- [Boltzmann Distribution (Wikipedia)](https://en.wikipedia.org/wiki/Boltzmann_distribution)
- [Statistical Mechanics by K. Huang](https://en.wikipedia.org/wiki/Kerson_Huang)

---


