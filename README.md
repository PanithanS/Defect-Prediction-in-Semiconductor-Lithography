# Defect prediction in chip manufacturing for yield optimization

![image](https://github.com/PanithanS/Defect-Prediction-in-Semiconductor-Lithography/assets/83627892/8ad89b43-b14d-46a4-8682-52d5ddad2908)

In recent decades, electronic devices like computers, tablets, and smartphones have become essential, thanks to ever-shrinking electronic circuits. Silicon-based integrated circuits, or chips, now squeeze over 10,000 transistors into a few square millimeters. The chip-making process starts on silicon wafers, sliced into chips. Advanced lithography tools are crucial for precise control and defect reduction, increasing manufacturing yield

# Manufacturing processes

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

# Lithography process control: light exposure parameters

The chip circuit pattern is made using lithography, which creates precise and sophisticated on a silicon wafers using masks. The well-optimized lithography system is expected to yield a high percentage of chips that function correctly within one wafer. Therefore, the lithography-involved parameter needs to be optimized, accordingly, there are two crucial parameters in the exposure process that need to be controlled to get a "good chip":

1. Exposure energy (Energy)
2. Focal length (Focus)

Therefore, to optimize manufacturing yield by focusing on the lithography process, it is required to explore the relationship between light exposure parameters and the good/die chips yields.

# Dataset: exposure parameters and 'die chip'
The dataset ".csv" files that we use in this work can be downloaded from https://github.com/jpcain/data-analytics-machine-learning/tree/master.
Here, We do a scatter plot demonstrating the exposure energy, i.e., Dose (mJ), and focal length, i.e., Focus (nm) as the two axis variables, which we use different colors as labels (Die chips/Good chips).

![image](https://github.com/PanithanS/Defect-Prediction-in-Semiconductor-Lithography/assets/83627892/fe352cbb-2be3-47f5-9e72-0bcd7d499931)

# Results: defect prediction using machine learning
In our analysis, we use various classifiers provided by the scikit-learn module to predict the defective chip yield from the exposure parameters. 
1. Multilayer Perceptron (MLP): the validation accuracy is 0.97
2. Gaussian Process Classifier (GP): the validation accuracy is 0.97
3. Supporting Vector Machine(SVM) : he validation accuracy is 0.95

 Overall, this classifier seems to make accurate predictions.

![image](https://github.com/PanithanS/Defect-Prediction-in-Semiconductor-Lithography/assets/83627892/461100d1-72a0-4096-8240-79eb15dc13cc)
***The decision boundaries***: We visualized the decision boundaries of each classifier that indicate the area on the 'Focus-Dose' plane where the classifier predicted the yield of 'good chips.'

### Application
According to the decision boundaries, we aim to optimize the lithography process parameter, ensuring it falls within the area associated with the successful 'good chip' that we predicted. This approach can enhance manufacturing yield and allows us to fine-tune the exposure parameter for optimal, high-quality chip production.


# Inspiration and acknowledgments
- Practical example from the SPIE short course "Data Analytics and Machine Learning in Semiconductor Manufacturing: Applications for Physical Design, Process and Yield Optimization" by Luigi Capodieci and Jason Cain.
- Inspired by: https://github.com/jpcain/data-analytics-machine-learning/tree/master
- Lithography principles: https://www.asml.com/en/technology/lithography-principles
# Reference
- Güler, Sila. "Bayesian optimization for lithography process control strategy selection: optimal control advisor." (2020).
