This scripts enables to generate the figure and the supplementary animation

Requirements
------------

Outside of the built-in libraries it has a five dependencies:
- numpy
- matplotlib
- h5py
- traits
- neuron

The first four dependencies can be installed easily using pip or easy_install. The last one requires the installation of the NEURON software (this might alas be tricky). 
(first install pip if you do not have it)
> sudo apt-get install python-pip
(install the depedency for h5 file)
> sudo apt-get install libhdf5-dev
(then install the dependencies)
> sudo pip install numpy matplotlib h5py traits
For the neuron dependency you have to figure it out with NEURON (sorry)

You also need to compile the .mod files before any usage of these scripts. You compile NmdaSynapse.mod and vecstim.mod by typing 
>nrnivmodl
when you are in the folder containing the script and the .mod files. 

To generate the figures just type in a terminal 
>python main.py 
when you are in the folder containing the script, it will first generate the data and then save the figures.

To generate the animation type 
>python anim.py
Same thing you need to be in the good folder.

Et voila
