# REATE A TODO WITH FORM DATA

### DESCRIPTION
This plugin allows the users of the application to create todos (which are like tasks). These todos can be created in an organization where it would be public and users can be assigned to it or be created for private use.

### END-POINT
<details>
  <summary> POST/todo </summary>

http://todo.zuri.chat/todo
 </details>
 

### METHOD 
POST


### PARAMETERS
| Name               | Data type | Description                                         |
| -------------------| --------- | --------------------------------------------------- |
| Organisation_id    | string    | ID of the organisation in which the todo is created |
| Plugin_id          | string    | This is the ID of the todo                          |
| User_id            | string    | The ID of the user creating the task                |
| Title              | string    | The refers to the name of the task                  |
| Description        | string    | A line of text explaining the purpose of the task   |

### Responses  
 - 200 (Successful Operation) <br>
   Response body:  
     
     ```sh
      {
        "type": "string",
        "user_id": "string",
        "title": "string",
        "status": "string",
    }
    ```
  - 400 (Invalid Input)
