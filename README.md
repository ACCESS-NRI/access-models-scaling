# access-models-scaling
Scaling data for the ACCESS models and the generate to generate them.

## Setup

The notebooks require that you're running on NCI Gadi for running the models to
generate the model outputs. However, if you're working with existing data, you
can run the notebook on whichever machine the data lives on.

### 1. Getting the notebooks

Cloning the repository is the easiest way to get the notebooks.

On Gadi, you'll probably want to clone the repository somewhere on scratch.

```bash
cd /scratch/$PROJECT/$USER
git clone https://github.com/ACCESS-NRI/access-models-scaling.git
cd access-models-scaling
```

### 2. Creating a virtual environment

Before starting the notebook, a Python virtual environment can be used to ensure all the
dependencies are accessible.

Create a virtual environment with a recent-ish version of Python.

```bash
# on gadi:
module load python3/3.12.1
python -m venv .venv
. .venv/bin/activate
```

### 3. Install dependencies and register environment

The dependencies will be enough to run the notebook, run the models, and then process the timing data.

```bash
pip install -r requirements.txt
```

### 4. Start the notebook

This can be done on the login node (e.g. through VSCode) or NCI ARE. If through ARE:
* remember to set the path to your venv in the Advanced Settings -> Python or Conda virtual environment base.
* A "small" compute size will be enough as not a lot of compute is happening.
* If you plan on generating the data from scratch, you can either set a long walltime eg. 12h, or start a short job to launch the jobs, then start a job later to process the results.
