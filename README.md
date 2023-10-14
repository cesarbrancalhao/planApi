# To-do List
To-do List application with Java, Spring Boot, Maven, H2, Lombock, Docker and Render.



### Deploy
https://todolist-ht01.onrender.com/

### Test
Download API Dog at https://apidog.com/download/

<p>In API Dog, create a new project.</p>
<p>Select <b>New Request</b> click <b>GET</b> and select <b>POST</b></p>
<p>In the url, enter https://todolist-ht01.onrender.com/users/</p>
<p>Click <b>Body</b> and select <b>json</b></p>
<p>Enter your information and press Send<br>
  
```json
{
    "username": "your_username",
    "name": "Your name",
    "password": "password_example"
}
```
<hr>
<p>Create a new POST request at https://todolist-ht01.onrender.com/tasks/</p>
<p>Go to <b>Auth</b> and enter your username and password</p>
<p>Go back to body, select the same options, enter the following informations and press Send</p>

```json
{
    "description": "Task description",
    "title": "Name of the task",
    "startAt": "yyyy-mm-ddThh:mm:ss",
    "endAt": "yyyy-mm-ddThh:mm:ss",
    "priority": "Low"
}
```
<h5>Warning: the 'T' between the day and hour should be keeped.</h5>

<p>To see your tasks create a <b>GET</b> request and enter your <b>Auth</b></p>
<p>To edit your tasks, create a <b>PUT</b> request, enter your <b>Auth</b> copy the "id" of the task, paste it after /tasks/, enter the field you want to edit and press Send</p>
<p>"<a href="">https://todolist-ht01.onrender.com/tasks/{taskid}</a>"</p>

```json
{
    "title": "New title"
}
```
