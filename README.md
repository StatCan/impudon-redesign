# Impudon Python Redesign

This repository hosts the code for redesigning and refactoring an imputation system called Impudon. The original implementation of Impudon was in SAS, but this repository focuses on implementing the donor imputation and historical imputation features in Python.

## Overview

This is an imputation system used to impute missing values in a dataset coming from The Central Provident Fund Board administers the Retirement and Health Study (RHS), a longitudinal study since 2014 – data is collected in biennial increments called *Waves*. 

This redesign project aims to migrate Impudon from its original SAS implementation to Python, providing a more flexible and accessible solution for imputation tasks. The repository includes code, documentation, and examples to demonstrate the functionality and usage of the redesigned Impudon system.

## Features

The Impudon Python Redesign repository focuses on implementing the following features:

1. **Donor Imputation**: This feature allows for imputation using donor values from similar records in the dataset. It helps fill in missing values by leveraging the information from other non-missing records.

2. **Historical Imputation**: Historical imputation utilizes temporal information to fill in missing values based on the historical patterns within the dataset. This feature is particularly useful when dealing with longitudinal data.

## Repository Structure

The repository is organized as follows:

```
├── src/
│   ├── config.yaml
│   ├── donor_imputation_functions.py
│   ├── historical_imputation_functions.py
│   └── main.py
│  
├── example/
│   └── imputation_functions_for_client_testing.ipynb
│  
├── requirements.txt
├── LICENSE
├── SECURITY.md
└── README.md
```

- The `src/` directory contains the Python scripts that implement the donor imputation and historical imputation features.

- The `examples/` directory provides Jupyter notebooks demonstrating the usage and application of the donor imputation and historical imputation features.


## Getting Started

To get started with the Impudon Python Redesign repository, follow these steps:

1. SSH Clone the repository to your local machine using the following command:

```bash
git clone git@gitlab-ssh.k8s.cloud.statcan.ca:impudon/impudon-python.git <repo-name>
```

2. Navigate to the cloned repository directory:

```bash
cd <repo-name>
```

3. Set up the necessary dependencies and environment for running the code. Refer to the documentation provided in each script or notebook for any specific requirements.

4. Explore the `src/` directory to find the Python scripts implementing the donor imputation and historical imputation features.

5. Refer to the `experiments/` directory for Jupyter notebooks that hosts imputation experiments.

5. Refer to the `examples/` directory for Jupyter notebooks that demonstrate the usage and application of the imputation methods.



## Requirements
To install the dependencies:
 
```bash
$ pip install --index-url=https://f3eaipitcat12.statcan.ca:8443/artifactory/api/pypi/pypi/simple --trusted-host=f3eaipitcat12.statcan.ca:8443 --user -r requirements.txt
```
If you get the following error:
 
**ERROR:** *Can not perform a '--user' install. User site-packages are not visible in this virtualenv.*
 
Then remove the *--user* option from the command:
 
 
```bash
$ pip install --index-url=https://f3eaipitcat12.statcan.ca:8443/artifactory/api/pypi/pypi/simple --trusted-host=f3eaipitcat12.statcan.ca:8443 -r requirements.txt
```
 
To deactivate your virtual environment:
 
```bash
$ deactivate
```

 
## License
 
Unless otherwise specified, the source code of this project is covered under Crown Copyright, Government of Canada, and is distributed under the [MIT License](https://gitlab.k8s.cloud.statcan.ca/impudon/impudon-python/-/blob/main/LICENSE).
 
The Canada wordmark and related graphics associated with this distribution are protected under trademark law and copyright law. No permission is granted to use them outside the parameters of the Government of Canada's corporate identity program. For more information, see [https://www.canada.ca/en/treasury-board-secretariat/topics/government-communications/federal-identity-requirements.html](Federal identity requirements).
 
 
 
## Authors
 
* **Loïc Muhirwa** - *Initial work* - [muhiloi](https://f3eaipitcap01.statcan.ca/muhiloi) <br/>
* **Angela Wang-Lin** - *Initial work* - [angela.wang-lin](https://gitlab.k8s.cloud.statcan.ca/angela.wang-lin) <br/>
* **Siddhartha Haldar** - *Initial work* - [siddhartha.haldar ](https://gitlab.k8s.cloud.statcan.ca/siddhartha.haldar) <br/>
