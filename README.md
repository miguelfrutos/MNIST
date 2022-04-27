

Folders Structure:
- input/: This folder consists of all the input files and data for your machine learning project. If you are working on NLP projects, you can keep your embeddings here. If you are working on image projects, all images go to a subfolder inside this folder. 
    - train.csv
    - test.csv
- src/: We will keep all the python scripts associated with the project here. If I talk about a python script, i.e. any *.py file, it is stored in the src folder.
    - model_dispatcher.py: will dispatch our models to our training script
    - config.py: Avoid including a hardcoded a training file and the output folder.
    - create_folds.py: Create the folds for cross-validation.
    - train.py: contains the training process 
    - inference.py:NA
    - models.py:NA
    - run.sh : shell script with different commands for different folds and run them all together. (sh run.sh)
- models/: This folder keeps all the trained models.
    - dt_{folds}.bin: Save the different k-folds model.
- notebooks/: All jupyter notebooks (i.e. any *.ipynb file) are stored in the notebooks folder.
- README.md: This is a markdown file where you can describe your project and write instructions on how to train the model or to serve this in a production environment.
- LICENSE: This is a simple text file that consists of a license for the project, such as MIT, Apache, etc. Going into details of the licenses is beyond the scope of this book.