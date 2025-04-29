
# DataVersion_DVC

This repository demonstrates data versioning using DVC (Data Version Control) in conjunction with Git. It provides a simple example of tracking and managing data files efficiently



# ​ Project Structure


To deploy this project run

```bash
DataVersion_DVC/
├── .dvc/               # DVC configuration and cache
├── .dvcignore          # Files and directories ignored by DVC
├── .gitignore          # Files and directories ignored by Git
├── Code.py             # Python script for data processing
├── data.dvc            # DVC-tracked data file
├── requirements.txt    # Python dependencies
├── text.txt            # Sample data file
└── S3/                 # Directory for S3-related files

```


## Getting Started
Prerequisites
 - Python 3.x
 - Git
- DVC
## Installation 
1. Clone the repository:
```
git  clone https://github.com/SandeepSuthar169/DataVersion_DVC.git
cd DataVersion_DVC

```
2. Install dependencies
```
pip install -r requirements.txt

```

3. Initialize DVC:
```
dvc init

```
4. Add a file to DVC,  push the data remote storage:
``` 
dvc add <data_file>

git add <data_file>.dvc .gitignore
git commit -m "Add new data file with DVC tracking"

dvc push


```
