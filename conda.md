# Using Conda and setting up environents.

Conda is a useful way to create containers for python environments. Normally using anaconda navigator everything can be done thoruhg GUI,
but sometime using conda gives additional access.

## Create a new enviornment using Anaconda Navigator.

Create a new environment by hitting 'create' in the environments panel. Install any required packages, for lumapi v231, make sure to include:
- SciPy v###
- Matplotlib v###

Be carefull to select the correct version for different packages or you will end-up spending a lot of time figuring out dependencies that are wrongly referenced. 

## Adding up local folders to a Conda env

List existing environments
```
conda env list
```

Select your intended environment
```
conda activate python3912_lumapi231
```

Add the Lumapi API to the environment path
```
conda develop "C:\Program Files\Lumerical\v231\api\python"
```


## Using your environment
Using visual studio code you can use the environments created in conda. First install the Python Extension, then from the command pallette (Ctrl + Shift + P), run  
```
Python: Select Interpreter
```
And select the enviornment we have just created.
