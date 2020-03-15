# Masters-Thesis-Neural-Network
My Master Thesis on Temperature and Humidity Profile Retrieval using Neural Network

This project deals with the technique of Remote Sensing using the Infrared Longwave Radiation emitted by the earth’s surface and atmosphere interplay (Earth’s Radiation Budget). Its application is specifically for the tropical regions of the earth, under the condition of clear sky with no presence of clouds. It is aimed at improving the data processing of the INSAT satellite observations, by applying principles of Optimization and Deep Learning that would speed up the process of retrieving vital
atmospheric parameters (Temperature Distribution, Humidity / Ozone Distributions) and at the same
time maintain a prescribed level of accuracy within the retrieved information.

To begin with, I simulated the earth’s radiation budget in the wavelength range of 640 cm-1-740 cm-1 using a
freeware, kCARTA, developed at UMBC. kCARTA is a pseudo line by line code developed for the purpose
of Radiative Heat Transfers through the earth’s atmosphere. It utilizes the Radiosonde measurement at
various pressure levels of the atmosphere and thereby gives the response (i.e. the Infrared Absorption
Spectrum) at the top of the atmosphere. Using these as the inputs, I retrieved the Atmospheric Temperature
Profiles, which is of prime importance in the project.

For the purpose of retrieval, I choose to implement an Artificial Neural Network model (ANN) which
requires far lesser memory consumption for its operation and is faster in its calculations. In the process, the
ANN model was trained rigorously to improve the accuracy of its prediction. To optimize the retrieval
further, I introduced the method of Principal Component Analysis (PCA) on the inputs. PCA method
classifies various dimensions (channels) of the input, by comparing the eigenvalues of its covariance matrix.
Using PCA classification, I discarded the dimensions having relatively lower eigenvalues, reducing the
dimensionality of the input considerably and subsequently improve the training, validation and testing of the
ANN model.

This project is focused on retrieving the Humidity and Temperature Profiles simultaneously and testing
the resultant ANN model with actual satellite observations. Though kCARTA is accurate in its predictions, the freeware suffers from excessive time consumption and
requires high performance computing to run efficiently. To overcome these drawbacks, an ANN model can
be proposed as a substitute to kCARTA. This ANN, if trained properly, will be an improved alternative for
the simulations of Earth’s Radiation Budget.
