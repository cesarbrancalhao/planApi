# To-do List
To-do List application with Java, Spring Boot, Maven, H2, Lombock, Docker and Render.

## Usage

### Deploy
-> https://todolist-ht01.onrender.com/ (API only)

### User

- Download API Dog at https://apidog.com/download/

- <p>In API Dog, create a new project/requisition.</p>
- <p>Select <b>New Request</b>, click <b>GET</b> and select <b>POST</b></p>
- <p>In the url, type "https://todolist-ht01.onrender.com/users/"</p>
- <p>Click <b>Body</b> and select <b>JSON</b></p>
- <p>Replace with your information and click <b>Send</b>:<br>

```json
{
    "username": "your_username",
    "name": "Your name",
    "password": "password_example"
}
```
<br />

### Tasks
- <p>Create a new <b>POST</b> request at https://todolist-ht01.onrender.com/tasks/</p>
- <p>Go to <b>Auth</b> and enter your username and password</p>
- <p>Go back to <b>Body</b>, select <b>JSON</b>, replace the following info and click <b>Send</b>:</p>

```json
{
    "description": "Task description",
    "title": "Name of the task",
    "startAt": "yyyy-mm-ddThh:mm:ss",
    "endAt": "yyyy-mm-ddThh:mm:ss",
    "priority": "Low"
}
```
<h4>Warning: the 'T' between the day and hour time must be maintained.</h4>

- <p>To see your tasks, create a <b>GET</b> request on /tasks/ and enter your username and password.</p>
- <p>To edit your tasks, create a <b>PUT</b> request, enter your username and password, copy the "id" of the task and paste it after /tasks/, edit the field you want to edit and click <b>Send</b></p>
  <h4>Example:</h4>
  <p>"<a href="">https://todolist-ht01.onrender.com/tasks/{taskid}</a>"</p>
  
  ```json
  {
      "title": "New title"
  }
  ```
