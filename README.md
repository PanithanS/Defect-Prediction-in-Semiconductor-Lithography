# Defect prediction in chip manufacturing for yield optimization

![image](https://github.com/PanithanS/Defect-Prediction-in-Semiconductor-Lithography/assets/83627892/8ad89b43-b14d-46a4-8682-52d5ddad2908)

Over the past few decades, electronic devices such as computers, tablets, and smartphones have become integral to our daily lives. These devices function on the sophisticated electronic circuits they contain. Notably, electronic circuits have steadily decreased in size since the inception of semiconductors in 1940. Presently, we have silicon-based integrated circuits (ICs), often referred to as chips, packing more than 10,000 transistors into just a few square millimeters of space. The production of these chips involves a fascinating process. Initially, they are crafted on silicon wafers, which are circular thin slices of silicon material. Afterward, the wafer is carefully chopped into individual chips. The utilization of advanced lithography tools is the key to crafting these sophisticated electronic circuits, therefore it is crucial to optimize lithography process control to reduce defects, as here we call "die chips", to increase manufacturing yield.

# Overviews in the semiconductor manufacturing process

![image](https://github.com/PanithanS/Defect-Prediction-in-Semiconductor-Lithography/assets/83627892/2cd32c31-cbe4-467e-b74b-80cc5b0230e0)

- **Wafer Manufacturing**
This is the initial step where silicon wafers are created from a single crystal of silicon. Wafers are thin, flat, and typically round substrates used as the foundation for semiconductor devices.

- **Wafer Oxidation**
In this process, a thin layer of silicon dioxide (SiO2) is grown or deposited onto the wafer's surface. This oxide layer serves as an insulator and is crucial for isolating and protecting the semiconductor components.

- **Deposition**
Deposition involves adding or "depositing" thin films of various materials (such as metals or insulators) onto the wafer's surface. These films serve as the building blocks for the creation of electronic components.

- **Lithography**
Lithography is a critical step for defining the precise patterns and structures on the wafer's surface. It involves transferring a mask pattern onto the photoresist-coated wafer, allowing selective material removal in subsequent steps.

- **Etching**
Etching is used to remove specific material layers from the wafer's surface, precisely following the patterns defined in the previous lithography step. It is often done using chemical or plasma processes.

- **Ion Implantation**
Ion implantation introduces dopant ions (atoms of different elements) into the semiconductor material, altering its electrical properties. This process is crucial for creating the desired conductivity and functionality in semiconductor devices.

These steps collectively form the basis for semiconductor manufacturing, enabling the creation of intricate electronic components found in a wide range of devices, from microchips in computers to sensors in smartphones.


## Exposure optimization

The chip circuit pattern is made using lithography, which involves creating intricate patterns on a silicon wafer using masks. This process is essential for manufacturing microchips used in various electronic devices. Lithography uses light to transfer these patterns onto the wafer through masks, allowing for the precise creation of transistors and interconnections that make up the integrated circuit. This precise and sophisticated patterning is crucial to make the chip function correctly.

Two parameters in exposure need to be considered:
1. Exposure energy (Energy)
2. Focal length (Focus)

## Dataset visualization: exposure parameters and die chips
![image](https://github.com/PanithanS/Defect-Prediction-in-Semiconductor-Lithography/assets/83627892/2d617e5e-40fe-4fd5-9532-a37f8c729c44)

..more content will be added


## Reference
- Güler, Sila. "Bayesian optimization for lithography process control strategy selection: optimal control advisor." (2020).
