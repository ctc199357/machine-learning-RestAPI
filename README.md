# machine-learning-RestAPI
Create RestAPI for Car Price Prediction


# Project Goal:

Build an end to end regression ML model and use Backend RestAPI to serve this model and front end UI so people can interact and use it through web browser. 

## Question in my mind:

What is RestAPI 

What is the difference between RestAPI and FastAPI

How the RestAPI being developed to serve the model? 

How to use Streamlit to design the fount-end UI

What is data parsing?

![image](https://user-images.githubusercontent.com/53972816/208387033-c9414bd9-3a35-4ae5-9148-d4f5ff757a6c.png)


## Procedure (Machine Learning)
1. Collect dataset 
2. Create python conda environment 
3. Explore data 
4. data preprocessing 
5. model training 
6. model evaluation 
7. model saving


## Create Backend Restful API

There are 3 moduels: 

1. Fastapi (Create an API object) that can be run on Unicorn server 
2. Use pydantic (Basemodel) to specify the schema (Input data) 
3. Create the route (Home route “/” for health check) 
4. Create the predict route (Take the input data and convert it to an array so that it can be served by the model) 
5. Run the Unicorn (And specify the host and port)

![image](https://user-images.githubusercontent.com/53972816/208386964-7cda6473-dcac-4017-834c-09d673a47082.png)



## Create Front-end UI and make request to API 
**How to send request to API?**

The request modules allows you to send HTTP requests using Python. The HTTP request returns a response Object with all the response data.


To run the whole things 

1. Open the API Server 

```python
python api/main.py
```

2. Run the UI stremlit

```python
streamlit run ui/car_price.py
```


![image](https://user-images.githubusercontent.com/53972816/208386880-a7010d63-12da-4cb9-8e0a-9d693301c1ab.png)
