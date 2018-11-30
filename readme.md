## Laravel Task

Here is a small laravel task for you so that we can test your Laravel Skills. Refer to [Contribution Guide](https://github.com/zomeds/backend_internship_task/blob/master/Documentation/contributing.md) for understanding how to install this task.

**Task Description**
You've been provided with a _Laravel_ 5.1 installation. You've to contribute your code to this repo only.
These are the tasks that you've to complete : 
- User Module<br>
  Laravel comes with out of the box User model and corresponding migrations. You've to make some changes to that so that a user can register, login into the application. Here are some extra features that you've to include in your User Module :
  * Ensure that the user who is registering is a human.
  * Login using mobile number and email (both).
- Create Medicine Module<br>
  You've to create a view where a User can create medicines (medicine properties are listed below). Use laravel eloquent to implement relations between User and medicines created by them. 

**Medicine Attributes**
- name (String)
- company_name (String)
- mrp (Float)
- quantity (Int)
  
**Compulsory Views**

`Registration`<br>
`Login`<br>
`Create Medicine`<br>

**Optional Views** (It'll be impressive if you include these)<br>

`My Medicines` (Medicines created by current user)<br>
`My Profile` (Details about logged in user)<br>
