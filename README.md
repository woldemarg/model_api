# Deploy a Machine Learning Model as an API on AWS


### Build the Model
1. Fork and clone the repository
2. Navigate to the model_api directory `cd model_api`
3. Run the model engine `python model_engine.py`


### Develop and Deploy the API
Follow along **[here](https://medium.com/@brent_64035/deploy-a-machine-learning-model-as-an-api-on-aws-43e92d08d05b)**

Test like this from Spyder IDE (locally):
!curl -H "Content-Type: application/json" -X GET localhost:5000/api -d "{\"INDUS\":\"5.9\", \"RM\":\"4.7\", \"AGE\":\"80.5\", \"DIS\":\"3.7\", \"NOX\":\"0.7\", \"PTRATIO\":\"13.6\"}"

On Windows you can use waitress instead of gunicorn:
https://stackoverflow.com/questions/11087682/does-gunicorn-run-on-windows
But gunicorn will work in a docker container:
https://medium.com/p/ae6b144f74c8/responses/show

