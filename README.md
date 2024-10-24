# Data-Extractor
0: Introduction

This is our end to end project where we will create a data abstractor tool .
This tool will take an elaborated text and summarize it to give us the short information or abstract
the important information to give us the summary as the output.
It is a very useful tool as it helps to reduce our time in going through the whole data and gives us the summary in the least time.


1: Github Repository Setting

First we have set up the github repository and then connected it with our local machine to work on it
    git add .
    git commit -m "done"
    git push origin main

2: Project template creation

We created the template for the project initially
    conda create -n EVM python=3.8 -y
    source activate base
    activate EVM

3: Project setup 

We create a virtual environment first

4: requirement installation

We use hugging face
Now we will go to setup.py and write it
and the install rewuirements
    pip install -r requirements.txt

5: logging ,utils and exception module

now first we will create custom logging inside the __init__.py file
now we will configure the utils common.py file(for frequent function)

We create the python code for the NLP Data Abstractor using google collab

data : https://github.com/AyushKumar177/Data/raw/main/DataAbstractorData.zip
 upload it to research folder

6: project workflow
    1.update config.yaml file 
    2.update params.yaml
    3.update entity in src
    4.update configuration manager in src config
    5.update the components
    6.update pipeline
    7.update main.py
    8.update app.py

7: notebook experiment and testing
now we create 01_data_ingestion.ipynb and configure our config.yaml and then update entity for return type ,also the params.yaml file after configurationManager is done in 01_data_ingestion.ipynb , we do the components and then pipeline
Now it created the artifacts folder and its contents
Now converting it to modular coding

8: component modular code implementation
    we use 01_data_ingestion.ipynb file for modular codes
    update __init__.py inside the entity folder
    update src/config/configuration.py  
    update src/components/data_ingestion.py
    update pipeline/stage_01_data_ingestion.py 

but for execution we have to write it in the main.py file
in main.py file we write the data ingestion stage (so the artifacts folder now would be created  automatically)

since we dont want to upload the artifacts folder we mention it inside .gitignore

Now we will create the 02_data_validation.ipynb file and follow the same order : config.yaml-entity-configuration manager-components-pipeline
after doing this it will create a data_validation folder and give a status.txt file
Now modular coding following steps in order entity-configuration manager-components-pipeline
following the previous ways

Now we will do data transformation in 03_data_transformation.ipynb in similar way to previous phases . We will convert the data to features using same functions from the DataAbstractor.ipynb notebook

Now we will configure the stage_04_model_trainer.ipynb in the same way and use the functions from DataAbstractor.ipynb
Here we will also declare the parameters in the params.yaml to use them in function like training arguments

Finally the 05_model_evaluation.ipynb and store the scores in same way

Training pipeline is completed

9: prediction pipeline & user app creation
Now we will create the prediction pipeline and user application
inside pipeline folder we create a prediction.py file and write it
then we write the app.py,to run it we create host and port
project implementation is done 

now we have to only deploy it


-----------------------------------------------
 
