This is the readme for the model associated with the papers:

Lee SG, Kim S (2006) Bifurcation analysis of mode-locking structure in
a Hodgkin-Huxley neuron under sinusoidal current. Phys Rev E Stat
Nonlin Soft Matter Phys 73:041924

Gangal et al., under preparation.

To run the code, follow these simple guidelines:

1) Unzip this archive and change directory to the new HHNeuron folder
2) compile any or each C file (most unix systems allow you to just type a
command like):
make c_file_name_without_the_dot_c_on_the_end
which should compile the C language file.
3) You will be able to run the C codes now with a command like
./c_file_name_without_the_dot_c_on_the_end
4) after a short time (less than a minute) data files will appear that you
can analyze with your favorite graphing program.

File Utilities : 
a) HHneuron_27June2013.c

This file solves the 4 parameters differential equations according to
Runge Kutta 4th order method , and generates text files with Voltage ,
Current , gate probabilities etc . Using thesis you can generate
action potential figures and find the gate probability information for
any input external current

b) Poincaremap_9thJuly2013.c

This is a mathematical tool that we used to find periodicity in the
system . Application of non linear dynamics to data analysis and
physical systems .

c) SpikeStatistics4thJulynight.c

This code returns the repeating spiking sequences in the output
voltages , and also the mode locking ratios of the O/P vs I/P in terms
of their frequencies

d) par_diag.h , par_HH.h 

We used the input to be sinusoidal , hence through the .h files we
specify the input frequency and the amplitude . You can also set a
range of frequencies or amplitudes or both . To provide a constant
input you just need to set the frequency to 0 and give the desired
amplitude . You can also modify the input to anything you want Except
the input current , the h files contains information of the simulation
time , delta frequency , delta amplitude etc

For any query on intricate functionality and bug reports , please mail
to himanshugangalcoursera@gmail.com
