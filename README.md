# Built AWS App to calculate longtitude/latitude 
![Long_Lat_AWS](https://github.com/takakokz/endtoend_appaws/assets/13964231/3cead01c-d37b-46d9-9fcd-b9284a7302f7)

## Objective and Method
Input longtitude and latitude of 2 locations into input parameters then calculate distance between 2 by clicking "Caulculate"  
Original  
![Website_NoValue](https://github.com/takakokz/endtoend_appaws/assets/13964231/f47cad50-a46a-4c11-98fc-9c378d8a49b9)  

Result  
![Website_Result](https://github.com/takakokz/endtoend_appaws/assets/13964231/183e5ad5-bcf1-4d2c-b209-39e905e761b9)  

In order to achieve it, I have created...
1. AWS Amplify to host a webpage  
2. AWS Lambda to calculate distance between 2 points
3. API to invoke Lambda function created  
4. AWS Dynamo DB then grant permission to Lambda to store/return math result into it   
5. Add API URL to code on Amplify, so Website can send Post API to calculate a value
