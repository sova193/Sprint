This is an API for a mobile application that tourists can use.

When tourists reach a mountain pass, they can take pictures and use a mobile app to send information.

The result of sending is a status and status message: { "status": 200, "message": "OK"}.

### **Models**
#### **Users**

User model contains information about the user: email, password, first name, last name and patronymic.

#### **Pereval**

Model of passes, contains information about the passes: name, beautiful name, coordinates, images, status, date of addition, ID of the user who added the pass.

#### **Coords**

Coordinate model, contains information about the coordinates of passes: latitude, longitude and altitude.

#### **Images**

Pass image model, contains information about the image and its name.

#### **Level**

Pass image model, contains information about the image and its name.



### **API methods:**

#### GET /submitData/ method

Returns a list of all mountain passes.

#### **POST /submitData/ method**

Allows you to create a record of one mountain pass.

#### **GET /submitData/{id}**

Retrieves data for a specific mountain pass.

#### **PATCH /submitData/{id}**

Allows you to change the attribute values of a mountain pass entry.

The result will be a message containing:

state:

Status: 1 for successful update and 0 for unsuccessful update.

message: explains why the change failed.

#### **GET/submit Data/?user__email=< email>**

Returns a list of data about all objects that a user with a given email sent to the server.
You can try using the API methods at  http://127.0.0.1:8000/swagger-ui/
