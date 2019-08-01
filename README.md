# TRISEP_ML_tutorial

## Introduction
This repository holds the notebooks and code for the Machine Learning tutorial at TRISEP 2019 on August 1st and 2nd. We will explore the application of Convolutional Neural Networks to the problem of particle identification in Water Cherenkov Detector.
Before proceeding please fork this repository by clicking on a button above in top right corner of the page.

## Acknowledgements
I borrowed code liberally from [code and tutorials](https://github.com/WatChMaL) developed by [Kazu Terao](https://github.com/drinkingkazu) and code by [Julian Ding](https://github.com/search?q=user%3Ajulianzding) and [Abhishek Kajal](https://github.com/search?q=user%3Aabhishekabhishek). Big thanks also to the [Water Cherenkov Machine Learning](https://github.com/WatChMaL) collaboration for lending their data - particularly [Nick Prouse](https://github.com/nickwp) for actually running the simulations and to Julian for 'massaging' the data.

## Starting on TRIUMF resources
Log into triumf-ml1.triumf.ca Your username has been derrived from your email by taking the part before the `@` character and removing dashes and dots. e.g. `winston-niles.rumfoord@infundibulum.space` $\rightarrow$ `winstonnilesrumfoord`. If the private key corresponding to the public key you gave me is not your default key you will need to specify it explicitly.
`ssh -Y -i <path/my_private_key> <my_username>@triumf-ml1.triumf.ca`



## Starting up on AWS instance
Log into your instance. username for everybody is `ubuntu`:
`ssh -Y -i <path/my_private_key> ubuntu@<aws_instance_assigned_to_me>`
Then launch a screen/tmux session. Next clone your repository, set up pytorch environment and launch jupyter notebook server. Instructions on how to set up ssh tunnel and bring up the jupyter root screen will be printed on your terminal.
```
screen
git clone <your forked repo url> TRISEP_ML_tutorial
. anaconda3/bin/activate pytorch_p36
cd TRISEP_ML_tutorial
. find_this_ip
./start_jupyternotebook.sh
```


