# Undergraduate Final Project
This work is a Undergraduate Final Project (TCC, in portuguese) in Electrical Engineering. In this Final Project is discussed the optimization process of nanophotonics devices using Deep Neural Networks.

- This research work was reported in an article and submitted to a conference (**IEEE Congress on Evolutionary Computation 2021**). Some relevant information is described below.

- Experimental content such as the Deep Neural Network and the entire optimization process can be accessed in the repository https://github.com/luizheinrich/DeepLearning-PhC

# Introduction
Nanophotonics is a branch of optical engineering that studies the behavior of light on the nanometer scale. In this approach, so many devices can be built by modifying and controlling the optical properties of materials, and that opens up possibilities for designing devices with diverse functionality. For example, in communication systems, there are important passive components nonreciprocal and control, such as isolators, switches, circulators, and power dividers. One of the fundamental tasks that they operate in integrated circuits is in the protection of electromagnetic sources against possible reflections of the signal from different parts of the circuit, in this way the transmission of this signal occurs only to desired parts of the circuit. Some of these devices are discussed in [[1]](#1) [[2]](#2) [[3]](#3) [[4]](#4).

Design these devices through computer simulations is a task that involves a high computational cost as their complexity increases. So many possibilities of device geometry need to be done experimentally until the geometry model that offers the best performance for the device is arrived at.

On the other hand, artificial intelligence has grown considerably in recent years. In large part, due to the great advance in deep learning (DL), which has had a powerful impact in the technology field, such as speech recognition, computer vision, autonomous car, and others. Deep learning is a machine learning (ML) technics that is inspired by the architecture of the human brain, which allows the machine to learn. It uses multiple layers of non-linear transformation to model high-level abstraction in data to obtain a learning model [[5]](#5).

In this context of optimization, a deep neural network (DNN) can learn how the geometry of the device is related to its frequency response. That fact is important in the optimization process, as it allows the neural network to indicate which is the most optimize geometry configuration for the device. This entire procedure is the scope of this paper.

# Problem Description
Nanophotonics devices are designed and studied from electromagnetic simulations and the goal is that they have the best efficiency possible. That can be evaluated by the performance of the transmission coefficients in their frequency response.

Therefore, each geometric modification results in different frequency responses. In this scenario, there is an ideal frequency response that we desired, for example, an isolations curves better than -20dB, transmission coefficient working at the center frequency (each device has its operating frequency), and their bandwidth higher as much as possible. However, by traditional methods, manual optimization is a very time-consuming process, since the number of variables involved is very large, to the point that, at times, the power of human decision may be imprecise.

# Goals
From simulations, we can generate a dataset contain features in geometry and frequency response. In the optimization approach, our goal is to extract a learning model form dataset with the DNN. Therefore, from a target frequency response, the DNN can design the device geometry, solving the inverse problem, inferring geometry from the desired frequency response.

# Results
Here we present an optimization procedure using Deep Neural Networks, a subfield from Machine Learning, to design photonic devices. This approach shows how DNNs can synthesize and streamline the design process and at the same time provide an accurate and time-efficient device characterization capability for complex nanostructures, where this process is based on data extracted from their frequency responses and geometry.

Our optimization procedure involves several different services and we have developed a script to automatizate the communication between them. This allowed the process to happen faster and automated.

This method was applies to optimize a circulator based in 2-D Photonic Crystal in [[6]](#6), in which has two resonators with dipole and qudrupole resonances. In both circulators there are nine curves in frequency response that need to be optimizade by geometry modification. The variables involved in the problem are so many that human precision can be ineffective. 

In this approach, the DNN demonstrated to be a powerful tool for the inverse design of nanophotonics devices discussed in this work.

# Informations
- Title: Otimização de Dispositivos Baseados em Cristais Fotônicos Usando Métodos em Machine Learning
- Author: Luiz Henrique P. Assunção
- Orientador: Victor Dmitriev
- Co-orientador: Ronaldo Zampolo
- E-mail: luiz.heinrich@live.com
- Instituição: Universidade Federal do Pará - UFPA
- Instituto: Istituto de Tecnologia - ITEC
- Curso: Engenharia Elétrica
- Cidade: Belém
- Categoria: Monografia
- Tags: TCC, engenharia, elétrica

## References
<a id="1">[1]</a> 
Dmitriev, Victor and Kawakatsu, Marcelo N. 
"Nonreciprocal optical divider based on two-dimensional photonic crystal and magneto-optical cavity". 
Optical Society of America.
vol. 51.
no. 24.
pp. 5917-5920.
2012.

<a id="2">[2]</a> 
Dmitriev, Victor and Portela, Gianni and Batista, Raphael.
"Magneto-optical resonator switches in two-dimensional photonic crystals: geometry, symmetry, scattering matrices, and two examples". 
Applied Optics.
vol. 53.
no. 20.
pp. 4460-4467.
2014.

<a id="3">[3]</a> 
Dmitriev, Victor and Portela, Gianni and Batista, Raphael.
"Dynamically controllable graphene terahertz splitters with nonreciprocal properties". 
Applied Optics.
vol. 58.
no. 24.
pp. 6513-6518.
2019.

<a id="4">[4]</a> 
Dmitriev, Victor and Portela, Gianni.
"Optical component: nonreciprocal three-way divider based on magneto-optical resonator". 
Applied Optics.
vol. 52.
no. 27.
pp. 6657-6662.
2013.

<a id="5">[5]</a> 
Géron, Aurélien.
"Hands-on machine learning with Scikit-Learn, Keras, and TensorFlow: Concepts, tools, and techniques to build intelligent systems".
O'Reilly Media.
ed. 2.
2019.

<a id="6">[6]</a> 
Dmitriev, Victor and Martins, Leno and Portela, Gianni and Assunção, Luiz. 
"Quadrupole resonator mode versus dipole one in photonic crystal ferrite circulators". 
Photonics and Nanostructures.
2021.
(Submitted).