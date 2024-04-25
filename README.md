# Handledelete
API Gateway: [Customers](https://us-west-1.console.aws.amazon.com/apigateway/main/apis/i9ry743iq0/resources?api=i9ry743iq0&region=us-west-1)

## Route: 
/customers/{id}

## Input: 
ID of the record to be deleted (##).

## Output: 
Empty Oject

## Function Mapping:
Lambda Function: 
[handleDelete](https://us-west-1.console.aws.amazon.com/lambda/home?region=us-west-1#/functions/handleDelete)

## Data Flow:
1. Client sends a DELETE request to {root_url}/customers/{id}.
2. Amazon API Gateway triggers the handleDelete Lambda function.
3. Lambda function deletes the record with the specified ID from the database.
4. Lambda function returns an empty object as the response.
5. Amazon API Gateway sends the response back to the client.
