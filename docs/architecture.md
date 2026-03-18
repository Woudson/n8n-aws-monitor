
# Project Architecture


# 1. Schedule Trigger (Node)

This node defines when the workflow is activated.
Set the execution time based on specific hours.

# 2. HTTP Request (Node)

* Method: **GET**
* Configure the request URL
* Authentication: **None**
* Response Options: Include **Response Headers** and **Status**

# 3. Edit Fields (Node)

* Use **JSON mode** to define parameters
* Convert URL-encoded data to JSON
* Add a **JavaScript code block**
* Set:

  * Mode: **Run Once for Each Item**
  * Language: **JavaScript**

This is where you write the code to define and process your parameters.

# 4. IF (Node)

* Configure the IF node using **JavaScript expressions**
* Evaluate conditions using **boolean** or **string** logic

# True Condition:

* Append a new row to the sheet

# False Condition:

* Add a **Code (JavaScript) node**

  * Mode: **Run Once for Each Item**
  * Language: **JavaScript**
* Write code to capture **staticData parameters**

Then:

* Append a row to the sheet to log the result

# 5. Gmail – Send a Message (Node)

* Log in with your credentials
* Configure the email details:

  * Recipient
  * Subject
  * Message content
