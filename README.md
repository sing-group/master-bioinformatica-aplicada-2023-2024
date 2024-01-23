# Machine Learning in Bioinformatics
> Máster en Bioinformática Aplicada a Medicina Personalizada y Salud (Curso 2023-2024)

# Scheduling

## First week (12-16 February 2024)
- Day 1 (12.02.2024):
  - 2/3 Theory
  - 1/3 Project: Session I ([project](PROJECT.md) presentation)
- Day 2 (13.02.2024):
  - 1/2 Theory
  - 1/2 Project: Session II
- Day 3 (14.02.2024): 
  - 2/3 Theory
  - 1/3 Project: Session III (with problem and dataset presentation [HITO-1](PROJECT.md))
- Day 4 (15.02.2024):
  - Practice: Hands-On (Machine Learning Basics in Python with scikit-learn Part I)
- Day 5 (16.02.2024):
  - Practice: Hands-On (Machine Learning Basics in Python with scikit-learn Part II)

## Second week (26-28 February 2024)
- Day 6 (26.02.2024):
  - 1/2 Theory: presentation of a real case-study (the [PolyDeep project](https://polydeep.org/))
  - 1/2 Project: Session IV
- Day 7 (27.02.2024):
    - Project: Session III
- Day 8 (28.02.2024):
    - Project Session: IV (with results presentation [HITO-2](PROJECT.md))

# Theory

The theory slides are available [here](resources/theory-machinelearning.pdf).

# Practice

## Install Docker in your system

Follow the steps in the official page to install Docker https://docs.docker.com/engine/install/ubuntu/

Make sure the docker user group exists.

```bash
sudo groupadd docker
```

Add your user to the docker group.

```bash
sudo usermod -aG docker $USER
```

Reboot the system and the changes will be applied.

## Running the Docker image

Run the following commands to pull the Docker image for the hands-on practice sessions:

```bash
docker pull singgroup/jupyter-machine-learning:2023-2024
```

During the hands-on sessions (Machine Learning Basics in Python with scikit-learn), we are going to use the `Breast Cancer Data` available at the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)). More information about this dataset can be found [here](https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.names) and [here](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data).

Go to an empty folder and run the following commands to download the data: 
```bash
mkdir data

wget https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.data -O data/wdbc.data

sed -i '1iid,diagnosis,radius_mean,texture_mean,perimeter_mean,area_mean,smoothness_mean,compactness_mean,concavity_mean,concave points_mean,symmetry_mean,fractal_dimension_mean,radius_se,texture_se,perimeter_se,area_se,smoothness_se,compactness_se,concavity_se,concave_points_se,symmetry_se,fractal_dimension_se,radius_worst,texture_worst,perimeter_worst,area_worst,smoothness_worst,compactness_worst,concavity_worst,concave points_worst,symmetry_worst,fractal_dimension_worst' data/wdbc.data
```

Alternatively, the file is also available [here](data/wdbc.data).

Clone or download this repository and then run the following command (from the local repository) to use the Docker image to start a Jupyter notebook with the required libraries already installed: 
```bash
docker run --rm -p 8888:8888 -v "$(pwd)":"$(pwd)" -w "$(pwd)" singgroup/jupyter-machine-learning:2023-2024
```

And then access `http://127.0.0.1:8888/lab` in a web browser. The `resources/notebook-ml-1.ipynb` file contains the notebook to develop during these sessions.

# Project

The information about the project is available [here](PROJECT.md).

# References
- [Practical Statistics for Data Scientists: 50 Essential Concepts](https://www.oreilly.com/library/view/practical-statistics-for/9781491952955/)
- [Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow, 2nd Edition](https://www.oreilly.com/library/view/hands-on-machine-learning/9781492032632/)

# Additional Resources
- Ten quick tips for machine learning in computational biology [[10.1186/s13040-017-0155-3](https://dx.doi.org/10.1186%2Fs13040-017-0155-3)]
- [LIBSVM -- A Library for Support Vector Machines](https://www.csie.ntu.edu.tw/~cjlin/libsvm/)
- [scikit-learn: machine learning in Python](https://scikit-learn.org/stable/)
