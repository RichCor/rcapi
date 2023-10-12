Richmond A. Corpuz 4-B

# JSON POST with Database Integration

This API endpoint, designed for JSON POST requests, facilitates the transmission of structured data from clients to a server, enabling the creation or updating of records. The JSON data contained in the request body enhances its adaptability and user-friendliness. Subsequently, the server responds by providing an HTTP status code and the requisite JSON data post-processing. This API can be effectively employed for purposes such as user registration, data updates, and custom workflows, all while ensuring a high level of security through authentication measures. It is imperative to consult the relevant documentation for a comprehensive understanding of the endpoint's prerequisites and procedures for managing errors.
## API Description

The API optimizes processes by providing a seamless mechanism for data administration, real-time communication, and secure incorporation of third-party services. It features robust authentication, a scalable architecture, and extensive documentation, enabling developers to design versatile and efficient applications. This results in improved functionality and heightened user engagement when using the API.

Purpose:
The API is meticulously designed to simplify intricate processes and augment the performance of your software applications. Whether you are engaged in the development of a website, mobile application, or any other form of software, our API provides a comprehensive array of tools aimed at optimizing operations, enhancing the user experience, and increasing overall productivity.


## API Endpoints

Endpoint: http://127.0.0.1/api/public/postName

Function: This endpoint is specifically designed for the addition of new information to the database.
Mandatory Parameters: The mandatory parameters for this operation are the First name (fname) and Last name (lname).
Endpoint: http://127.0.0.1/api/public/postUpdate

Function: This endpoint is employed for the purpose of modifying pre-existing data within the database.
Mandatory Parameters: The operation necessitates the inclusion of the ID, First name (fname), and Last name (lname) as obligatory parameters.
Endpoint: http://127.0.0.1/api/public/postPrint

Function: The primary role of this endpoint is to display the data that is stored in the database.
Mandatory Parameters: Notably, there are no mandatory parameters required for this operation.
Endpoint: http://127.0.0.1/api/public/postDelete

Function: This endpoint is responsible for the removal of specific data from the database.
Mandatory Parameters: The sole required parameter for this function is the ID.



## Request Payload

## JSON Payload postName:

- Request payload:
{
  "lname":"hortizuela",
   "fname":"manny"
}

This payload is used for creating a new name entry. It requires both the last name ("lname") and first name ("fname") of the person being added.

## JSON Payload printName:
 
- Request payload:

This payload does not contain any specific fields. It might be used for retrieving or printing a name from the system, but the payload itself does not specify any required or optional fields.

## JSON Payload updateName:

- Request payload:
{
  "id":1,
  "lname":"wick",
   "fname":"john"
}

This payload is used for updating an existing name entry identified by the specified "id". It requires the updated last name ("lname") and first name ("fname") of the person.

## JSON Payload deleteName:

- Request payload:
{
  "id":1
}

This payload is used for deleting a name entry based on the specified "id". It only requires the unique identifier of the name entry to be deleted.

## Response

## JSON Payload postName:

- Response payload:
{
         "status":"success","data":null
}



## JSON Payload printName:

- Response payload:
{
         "status":"success","data":["lname":"hortizuela","fname":"manny","lname":"licayan","fname":"arnold"]
}




## JSON Payload updateName:

- Response payload:
{
         "status":"success","data":null
}




## JSON Payload deleteName:

- Response payload:
{
         "status":"success","data":null
}





## Usage

Follow these steps to manipulate database information using Postman and the API endpoints:

1.Initialize Postman:

Ensure that Postman is both installed and operational on your system.
2. Dispatch a POST Request to Insert Data:

For the purpose of inserting data into the database via the /api/public/postName endpoint:
Select the HTTP method as POST.
Specify the URL as http://127.0.0.1/api/public/postName.
Within the request body, define the parameters fname and lname, and input the desired values for insertion.
Click the "Send" button to initiate the request.
3. Issue a POST Request to Update Data:

To effect updates on existing database entries using the /api/public/postUpdate endpoint:
Choose the HTTP method as POST.
Input the URL as http://127.0.0.1/api/public/postUpdate.
Within the request body, provide the parameters id, fname, and lname, and include the updated values.
Click "Send" to submit the request.
4. Transmit a POST Request to Retrieve Data:

For the purpose of displaying database data through the /api/public/postPrint endpoint:
Opt for the HTTP method as POST.
Specify the URL as http://127.0.0.1/api/public/postPrint.
Maintain an empty request body since no additional parameters are necessary.
Click "Send" to transmit the request.
5. Dispatch a POST Request to Erase Data:

To eradicate data from the database through the /api/public/postDelete endpoint, you should:

Select the HTTP method as POST.
Specify the URL as http://127.0.0.1/api/public/postDelete.
Within the request body, incorporate the parameter id and assign it the ID of the data you intend to delete.

Click "Send" to initiate the request.
 

## License

No License 


## Contributors

Sir Manny Hortizuela
provided:

- some codes
- database structure
- payloads
- etc.


## Contact
Include contact
information for inquiries or support.

Richmond A. Corpuz
- richmond.corpuz@student.dmmmsu.edu.ph
- 09501113950

