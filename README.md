Node Js session for student at code center. This is a practical example of building an Express API. This APIs will be use fro front end development in the classes to come.

### Task for the Week.
Build APIs for an E-commerce app. The user of the app should be able to sign up, login, go to home page and be greeted will a welcome message, get email notification when they register. User should be able to log out, post images, update their profile, delete an image and any other functionality you can think of.

### Available Endpoints
* **"/"** : Method **GET**. This is the home endpoint.
* **"/signup"**: Method **POST**. This is the endpoint for user to register.
	* **Request Object**:
		* firstName : Type(String)
		* lastName : Type(String)
		* username : Type(String)
		* password : Type(String)
		* bio : Type(String)
		* email : Type(String)
		* gender : Type(String)
		* phoneNumber : Type(Number)
		* address : Type(String)
		* state : Type(String)

	* **Response Object**:
		* firstName : Type(String)
		* lastName : Type(String)
		* username : Type(String)
		* password : Type(String)
		* bio : Type(String)
		* email : Type(String)
		* gender : Type(String)
		* phoneNumber : Type(Number)
		* address : Type(String)
		* state : Type(String)


* **"/login"**: Method **POST**. This is the endpoint for login into the app.
	* **Request Object**:
		* username
		* password
	* **Response Object**:
		* username
		* password

* **"/task"**: Method **POST**. This is the endpoint for user to add task.
	* **Request Object**:
		* taskName : Type(String)
		* time : Type(String)
		* description: Type(String)
		* isCompleted : Type(Boolean)
		* reminderTime : Type(Number)

	* **Response Object**:
		* taskName : Type(String)
		* time : Type(String)
		* description: Type(String)
		* isCompleted : Type(Boolean)
		* reminderTime : Type(Number)

* **"/update/:taskId"**:  **PATCH** Method. This is the endpoint to update task by its database unique id.
	 * **Request Object**:
		* taskName : Type(String)
		* time : Type(String)
		* description: Type(String)
		* isCompleted : Type(Boolean)
		* reminderTime : Type(Number)

	* **Response Object**:
		* taskName : Type(String)
		* time : Type(String)
		* description: Type(String)
		* isCompleted : Type(Boolean)
		* reminderTime : Type(Number)

* **"/delete/:taskId"**: **DELETE** Method. This is the endpoint to delete a task by it's unique ID.
	* **Response** : "task deleted."
*  **"'/logout"**: **GET** Method. This is the endpoint to logout.
	* **Response** : "Log out successful."