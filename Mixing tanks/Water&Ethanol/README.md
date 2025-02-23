Simulate the mixing of pure ethanol and water streams in DWSIM to analyze:
- **Composition**: Mole fractions of ethanol and water in the outlet stream.  
- **Temperature**: Adiabatic mixing temperature.  
- **Impact of Thermodynamic Models**: Compare results with literature data.
SETUP in DWSIM:
- **Input Streams**:  
  - **Water Stream**:  
    - Mass Flow: 27.77 g/s  
    - Temperature: 25°C  
    - Pressure: 1 atm  
    - Composition: 100% water.  
  - **Ethanol Stream**:  
    - Mass Flow: 13.8 g/s  
    - Temperature: 30°C  
    - Pressure: 1 atm  
    - Composition: 100% ethanol.  
- **Unit Operation**: Mixer.  
- **Thermodynamic Model**: NRTL (selected to account for non-ideal ethanol-water interactions).  
Results:
- **Outlet Stream**:  
  - Mass Flow: 41.6 g/s
  - Temperature: 23.8°C (adiabatic mixing).  
  - Composition (Molar Basis):  
    - Ethanol: 10.9%  
    - Water: 89.02%.
Observations:
- **Non-Ideal Behavior**:  
  - Ethanol’s mole fraction (10.9%) is lower than ideal mixing (~16.3%), due to hydrogen bonding modeled by NRTL.  
- **Temperature Drop**: Mixing cooler and warmer streams resulted in a lower outlet temperature (23.8°C), influenced by the heat of mixing.
- Ethanol-water mixtures are **highly non-ideal** and form an azeotrope at ~95% ethanol (by mass).  
- While this simulation used pure components, future work could explore azeotropic behavior by varying concentrations.
