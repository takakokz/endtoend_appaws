# Built AWS App to calculate longtitude/latitude 
![Long_Lat_AWS](https://github.com/takakokz/endtoend_appaws/assets/13964231/3cead01c-d37b-46d9-9fcd-b9284a7302f7)

## Objective and Method
Input longtitude and latitude of 2 locations into input parameters then calculate distance between 2 by clicking "Caulculate"  
Original  
![1](https://github.com/takakokz/endtoend_appaws/assets/13964231/f7ace4d0-7058-4ec8-9eff-f50a55f7f535)  

Input  
Access From here https://dev.d34vlivsdltjdj.amplifyapp.com/
Starbucks headquarters in Seattle, WA  
47.5975024  
-122.3492781  

Times Square in New York City, NY  
40.7579787  
-73.9900326  

Result  
![2](https://github.com/takakokz/endtoend_appaws/assets/13964231/6040a3f7-dbd5-4c85-a264-d597b877de9d)  


In order to achieve it, I have created...
1. AWS Amplify to host a webpage  
2. AWS Lambda to calculate distance between 2 points
3. API to invoke Lambda function created  
4. AWS Dynamo DB then grant permission to Lambda to store/return math result into it   
5. Add API URL to code on Amplify, so Website can send Post API to calculate a value

## Process  

Upload Index.html to Amplify  
![3](https://github.com/takakokz/endtoend_appaws/assets/13964231/5cd0dc05-aefa-4a2a-93a2-f446d9fe08b3)  

Create Lambda function and set trigger by API Post   
![5](https://github.com/takakokz/endtoend_appaws/assets/13964231/9eda8052-857d-4896-a8e1-b02814d4ad6d)  
![4](https://github.com/takakokz/endtoend_appaws/assets/13964231/4972a1c2-495b-4e32-9fc1-eeae2636543a)  

Create Dynamo DB then crate IAM policy to grant pamission for Lambda to write result into the table
![6](https://github.com/takakokz/endtoend_appaws/assets/13964231/548cbc2c-6faf-4cc9-8e6e-357d00107945)

Update index file to call the API created  
![7](https://github.com/takakokz/endtoend_appaws/assets/13964231/47968de5-03bb-4dbd-9733-766370ba2450)  


