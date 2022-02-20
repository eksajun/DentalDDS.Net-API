# DentalDDS.Net-API
C# Net API layer
<h2>Dental DDS API application is online now...</h2>
<h4>Start Angular UI project from the DentalDDS-UI folder and run with the 'ng serve --o' command.</h4>
<h4>At login dialog, first register yourself and then login.</h4>

<br />
Alternatively, you may use API client to test the APIs endpoints below.
<k4></k4>
<h4>Simple Test</h4>
<ul>
    <li><b>[GET] https://localhost:44370/api/account/APITest</b></li>
</ul>

<h4>Register User</h4>
<ul>
    <li><b>[POST] https://localhost:44370/api/account/PostUserRegister</b></li>
    <li><p>{FirstName}, {LastName}, {MobileNumber}, {UserName}, {Password}, {ConfirmPassword} *Password must be 7 Char Aa1!</p></li>
</ul>

<h4>Login JW-Token</h4>
<ul>
    <li><b>[POST] https://localhost:44370/oauth/token</b></li>
    <li><p>{userName}, {password}, {grant_type}</p></li>
</ul>

<h4>Add Task</h4>(Secure endpoint, use token from above)
<ul>
    <li><b>[POST] https://localhost:44370/api/user/PostNewTask</b></li>
    <li><p>{TaskName}, {TaskDetail}, {TaskDateTime} {UserName }</p></li>
</ul>

<h4>Select A Task</h4>(Secure endpoint, use token from above)
<ul>
    <li><b>[GET] https://localhost:44370/api/user/GetSelectedTaskByID</b></li>
    <li><p>{TaskID:Number}</p></li>
</ul>

<h4>User TasksList</h4>(Secure endpoint, use token from above)
<ul>
    <li><b>[GET] https://localhost:44370/api/user/GetTasksListByUser</b></li>
    <li><p>{userName}</p></li>
</ul>


<h4>Edit A Task</h4>(Secure endpoint, use token from above)
<ul>
    <li><b>[PUT] https://localhost:44370/api/user/UpdateTasks</b></li>
    <li><p>{TasksID}, {TaskName}, {TaskDetail}, {TaskDateTime}, {UserName }</p></li>
</ul>

<h4>Delete A Task</h4>(Secure endpoint, use token from above)
<ul>
    <li><b>[DELETE] https://localhost:44370/api/user/DeleteSelectedTask</b></li>
    <li><p>{TaskID:Number}</p></li>
</ul>



