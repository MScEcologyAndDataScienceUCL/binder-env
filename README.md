# MSc Ecology and Data Science - Lab Coding Environment

This repository defines the coding environment for the MSc practicals. We use
[Binder](https://mybinder.org/) to create and manage easy-to-setup and
reproducible environments in which students can learn through coding.

> Binder allows you to create custom computing environments that can be shared and used by many remote users.

## Running the Environment

To run the environment, click the "launch binder" button.

## Libraries and Dependencies

* Add libraries in the `apt.txt` file.
* Add R dependencies in `install.R`.
* Add Python dependencies in `requirements.txt` using version pinning for environment stability.

For detailed information on how to setup the environment using Binder please
refer to the
[official documentation](https://mybinder.readthedocs.io/en/latest/index.html).

### Example dependency files

Libraries are installed in the `apt.txt` file:

```
libgdal-dev
libproj-dev
...
```

R dependencies are installed in the R script `install.R`:

```R
install.packages("ggplot2")
install.packages("dplyr")
...
```

Python packages are added to the environment by listing them in the
requirements.txt file. Specific package versions can be specified through
[string specifiers](https://peps.python.org/pep-0440/#version-specifiers).

```
scikit-learn
pandas==1.5.3
matplotlib>=3.5.0
https://github.com/MScEcologyAndDataScienceUCL/BIOS0032_AI4Environment
```
