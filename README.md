# ICA user MNE-Python


## Installation


### Installing conda
If you don't have python, I recommand to install it using [conda](https://docs.conda.io/projects/conda/en/latest/). Conda is an open-source package management system and environment management system that runs on Windows, macOS, and Linux. Conda quickly installs, runs, and updates packages and their dependencies. Conda easily creates, saves, loads, and switches between environments on your local computer.

For a quick and light installation, I recommand to use [miniconda](https://docs.conda.io/en/latest/miniconda.html) a free minimal installer for conda.

Select the version corresponding to your operating system and download and install it.

### Create a new environment
Once completed, you should have access to a new shell named
`Anaconda Prompt` on your computer.

Launch it and create a new python environment using the `conda create` command.

```console
conda create -n eeg39 python=3.9
```

Here we specify the name of the new environment `eeg39` and the python version `3.9`.

Anaconda will ask you if you are sure you can to create this new environment

```console
Proceed ([y]/n)?
```
Press <kbd>y</kbd> then <kbd>Enter</kbd> to accept

### Installing dependencies

Activate the new environment using:

```console
conda activate eeg39
```
Notice that the current environment is displayed at the beginning of your shell:

```console
(eeg39) C:\Users\ferat>
```

Install the required python packages:
 - `notebook` to use jupyter notebook interface:

    ```pip install notebook```

 - `mne` the main python EEG librairy.

    ```pip install mne```

 - `picard` an implementation of the picard ICA solver. 

     ```pip install python-picard```

 - `mne-qt-browser` a 2D backend for plotting MNE data.

    ```pip install PyQt5 mne matplotlib mne-qt-browser```

 - `pybv` to export file to the brainvision format
    
    ```pip install pybv```

To install everything at once:

```console
pip install notebook mne python-picard matplotlib mne-qt-browser pybv
```

## Use the code

Each time you want to use the environment, you need to activate it using:

```console
conda activate eeg39
```

Then start the jupyter server:

```console
jupyter notebook
```

