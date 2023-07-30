# Determining Degrees of Separation between Marvel Superheroes with Breadth-first Search in PySpark RDD

[![GitHub](https://badgen.net/badge/icon/GitHub?icon=github&color=black&label)](https://github.com/MaxineXiong)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Made with Python](https://img.shields.io/badge/Python->3.6%2C_<=3.8-3776AB?logo=python&logoColor=white)](https://www.python.org)
[![Apache Spark](https://img.shields.io/static/v1?label=&message=Apache+Spark&color=%23000000&logo=Apache+Spark&logoColor=%23E25A1C)](https://spark.apache.org/)

<br>

In this project, we aim to determine the degree of separation between two Marvel superheroes based on their network connections within the [Marvel universe](https://www.marvel.com/). 
The connections between superheroes are established by analysing their appearances together in the same comic books, reflecting their interactions and collaborations 
within the Marvel universe. If two superheroes have ever appeared in the same comic books, they are considered directly connected to each other. To find the degrees of separation, 
we employ the powerful **[Breadth-first Search (BFS)](https://www.geeksforgeeks.org/breadth-first-search-or-bfs-for-a-graph/)** algorithm implemented in **[PySpark RDD](https://spark.apache.org/docs/latest/api/python/reference/api/pyspark.RDD.html)**. This algorithm allows us to efficiently explore the network of superhero connections 
and calculate the shortest path(s) between any two given superheroes. The concept of implementing BFS algorithm in this project is demonstrated through a simple example illustrated below:

![spark-BFS](https://github.com/MaxineXiong/Degrees-of-Separation-with-Breadth-first-Search/assets/55864839/ebf8fa3d-3726-47db-a716-e84baf19b509)

<br>

## **Features**

- Utilizes the **Breadth-first Search (BFS)** algorithm implemented in **PySpark RDD** to find the degrees of separation between two given superheroes efficiently.
- Employs user-defined functions to perform the BFS algorithm and efficiently explore the network of superhero connections.
- Provides an interactive function to search for superheroes by their names or IDs, facilitating easy query of hero information.
- Supports the analysis of various superhero pairs to determine their degrees of separation.

<br>

## **Repository Structure**

This repository consists of the following files:

```
Degrees of Separation with Breadth-first Search
├── Degrees of Separation with Breadth-first Search Algorithm.ipynb
├── data
│   ├── Marvel-graph.txt
│   └── Marvel-names.txt
├── README.md
├── APACHE LICENSE
└── MIT LICENSE
```
**Degrees of Separation with Breadth-first Search Algorithm.ipynb**: This Jupyter Notebook serves as the main spark driver file. It contains the code implementation of the BFS algorithm in PySpark RDD to find degrees of separation between heroes.

**data/Marvel-graph.txt**: Represents the network of Marvel superheroes based on their comic book appearances. It is a [dataset](https://www.projectpro.io/article/100-machine-learning-datasets-curated-for-you/407) containing heroIDs and their corresponding connections with other superheroes.

**data/Marvel-names.txt**: Provides a mapping between heroIDs and their corresponding superhero names. This [dataset](https://www.projectpro.io/article/100-machine-learning-datasets-curated-for-you/407) allows easy identification and reference to specific superheroes within the Marvel universe.

**README.md**: The current file you are reading. It provides an overview of the repository, project description, usage, and other relevant information.

**APACHE LICENSE**: The license file for the project.

**MIT LICENSE**: The license file for the project.

<br>

## **Usage**

**Note:** As of July 2023, PySpark is not fully compatible with Python 3.11. It is highly recommended to use ***Python 3.7*** or ***3.8*** for executing any PySpark-related operations.

To set up the environment for running the Spark code, follow these steps:

1. Open **Anaconda Prompt** and execute the following command to create a conda environment powered by Python 3.8:

   ```
   conda create -n py38 python=3.8 anaconda
   ```

3. Open **Anaconda Navigator**, go to **Environments**, and select the **py38** environment to install the "**pyspark**" package.
4. In the **py38** environment folder (e.g. "C:\Users\\[your-user-name]\anaconda3\envs\py38"), create a copy of **python.exe** and rename it to "**python3.exe**".
5. Open the **Jupyter Notebook** application from your **Anaconda Navigator**. The notebooks you open should now run on Python 3.8. You can check the Python version by executing `!python --version` in a notebook code cell.
6. Download this repository and open the **Degrees of Separation with Breadth-first Search Algorithm.ipynb** in your Jupyter Notebook.

<br>

## **Contribution**

Contributions to the project are welcome! If you find any issues or have suggestions for improvement, please feel free to open an issue or submit a pull request.

<br>

## **License**

The project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/) and [Apache License](http://www.apache.org/licenses/).

<br>

## **Acknowledgement**

I extend my gratitude to the [Marvel universe](https://www.marvel.com/) and its creators for providing the rich dataset that makes this project possible. Additionally, I thank the [PySpark](https://spark.apache.org/docs/latest/api/python/#:~:text=PySpark%20is%20the%20Python%20API,for%20interactively%20analyzing%20your%20data.) and [Apache Spark](https://spark.apache.org/) communities for their valuable contributions to the data processing and analysis ecosystem.
