# mortgage-prediction-html
Uses the new IAM authentication method for WML authentication as well. 

View demo of app here (deployed on IBM Cloud): https://mortgage-pred-anchal-surprised-ratel.eu-de.mybluemix.net/ 

## Steps to create Model on SPSS 

1. Create a watson studio and machine learning service on cloud 
2. Lauch watson studio 
3. Create a project
4. Go to the project and click on add to project 
5. Select Modeler Flow, give the flow a name and select SPSS flow
   a. Select from file and upload the modeler.str file 
6. Run the flow 
Note: if you get an error to run the flow, delete the data files and drag and drop them and use the data files from the repo 
7. Deploy the model when the WML model is created on Watson studio. 


## Steps to create front-end application 

1. Edit the server.py file: 
2. Edit your credentials from IBM cloud account: 
 - Add api key 
 - Add ML instance ID

3. Add the scoring URL of the model created on Watson Studio. This will be present in the deployments tab when you deploy the model. 
4. Run application using the following command: python server.py 
5. Open your browser and go to https://localhost:8080
