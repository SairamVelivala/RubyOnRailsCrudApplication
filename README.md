I have created a simple information security blog for users to post the latest trends in information security. 
The architecture used in this project is as follows: 

User --- Browser --- Rails Router ---- controller -- Views --- Model --- Database

Controller -- Data flows to Model and Views. 

User – Sends a request to the browser – that is sent to the rails router – that is further sent to the controller – then the request goes to the – Model – from the model it goes to the – Database – from the database – Model – form the model – to controller – views – back to the browser. 
When the user types the url this request hits the rails router(router.rb).  It maps the url to the controller. The action requests the response and asks for the the model and then fetches the data from the database and sends to the model and then to the controller and then to the views renders html and it is send to the controller and browser. 
Here we use the MVC framework. 
The model would hold the raw data and hold essential components of the blog. It will describe the post title and post content. 
View is made up of functions used by the user.
Controller acts an ambassador between model and view. It is the brain of the process. 
Pattern used in rails is the Active records pattern: 
It deals with the object and behavior. It is derived and described by ORM. It represents models and data and relationship between models. Validation of models before persisted. Database base operations in object oriented fashion. Active records allow easy migration of the database. 

The home page of the blog would show all the posts that have been posted by all the users. On the top right side of the navigation bar we can see the “Home” , “New Post”  and “contact” links. 
Further we can also see the read posts link below every post

