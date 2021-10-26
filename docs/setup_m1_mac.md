# Installing Tensorflow on m1 macs

Install XCode command line tools:
```
    xcode-select --install
```

Install miniforge from their github:

```
    https://github.com/conda-forge/miniforge
```

disable the default conda environment:
```
    conda config --set auto_activate_base false
```

Create and activate new virtual environment:
```
    conda create --name buffpy python=3.8
    conda activate buffpy
```
*(you will need to run the last line whenever you use buffpy)*


Install Apple's version of Tensorflow (tensorflow-metal optional)
```
    conda install -c apple tensorflow-deps
    conda install tensorflow-macos
    conda install tensorflow-metal
```

Launch a jupyter notebook with the conda environment:

```
    jupyter notebook
```







