# GPS

[Global Pathway Selection](https://www.sciencedirect.com/science/article/pii/S0010218016000638) (GPS) is an algorithm to effectively generates reduced (skeletal) chemistry mechanisms, which speeds up simulations and can be used as a systematic analytics tool to extract insights from complex reacting system.

![](https://github.com/golsun/GPS/blob/master/ui/ui_main.PNG)

## How to install
This repo is developed with Python 2.7 and based on many packages. The easiest way is to install them with the [Anaconda](https://www.anaconda.com/distribution/) and [Pip](https://pip.pypa.io/en/stable/installing/). 
* You can simply set up the environment by typing `conda env create -f env.yml` in Anaconda Prompt
* Or, please use the following commands in Anaconda Prompt to set up the environment step-by-step.
```
    conda create -n gps python=2.7
    conda activate gps
    conda install -c cantera cantera
    conda install -c anaconda pyqt=4.11.4
    conda install -c anaconda networkx=1.10
    pip install matplotlib, scipy
```

## How to use
* firstly activate the anaconda environment you created `conda activate gps`
* then GPS can be started by `python GPS.py`
* you can also plot flux graph with `python plot_flux_graph.py`

for more detailed tutorial, please see [Tutorial_v1.0.0.pdf](https://github.com/golsun/GPS/blob/master/Tutorial_v1.0.0.pdf). The following interface should show up:


## How to cite
To improve the accuracy of reduced mechanisms, GPS considers all-generation relation between species, and minimizes the risk of broken pathway or dead-end issue. This algorithm is developed by Prof. Wenting Sun's group at Georgia Tech [[link](http://sun.gatech.edu/)]

* X. Gao, S. Yang, W. Sun, "A global pathway selection algorithm for the reduction of detailed chemical kinetic mechanisms", **Combustion and Flame**, 167 (2016) 238–247 [[link](https://www.sciencedirect.com/science/article/pii/S0010218016000638)]
* X. Gao, X. Gou, W. Sun, "Global Pathway Analysis: a hierarchical framework to understand complex chemical kinetics", **Combustion Theory and Modelling**, 2018 pp.1-23. [[link](https://www.tandfonline.com/doi/abs/10.1080/13647830.2018.1560503)]

## Related publication
* Gao, X., Gou, X. and Sun, W., 2018. Global Pathway Analysis: a hierarchical framework to understand complex chemical kinetics. Combustion Theory and Modelling, pp.1-23.
* X. Gao, W. Sun, Using Global Pathway Selection Method to Understand Chemical Kinetics, 55th AIAA Aerospace Sciences Meeting, (2017) AIAA 2017-0836.
* X. Gao, W. Sun, Global Pathway Analysis of the Autoignition and Extinction of Aromatic/Alkane mixture,  53rd AIAA/SAE/ASEE Joint Propulsion Conference, Atlanta, Georgia, 2017.
* S. Yang, X. Gao, W. Sun, Global Pathway Analysis of the Extinction and Re-ignition of a Turbulent Non-Premixed Flame,  53rd AIAA/SAE/ASEE Joint Propulsion Conference, Atlanta, Georgia, 2017.
