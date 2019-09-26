# django-interview-questions
Django interview question that I've been asked.
##Django - Interview Questions


Q#1. What do you like about django? Or the same question can be re-phrased as what are the features of django?

Answer: Django is secure, fast and rapid application development(RAD) framework.. It offers/features are:

●	Admin Interface (CRUD)
●	Templating
●	Form handling
●	Internationalization
●	Session, user management, role-based permissions, messages
●	Object-relational mapping (ORM)

Q#2. What architecture does Django follow? Or Is Django an MVC framework?
Answer: Django follows MTV pattern/architecture. MTV stands for Model, Template, View.

Q#3. How to write views in django?
Answer. There are 2 primary methods to write views in django. First is the django function based views and second is django’s class based views. Function based views are simple and are better option to go for if you know that you have to create less than 8-10 views.

Q#4. What’s the current version of Django? Or (What django version are you currently working with)?
Answer. Django 2.2

Q#5. How to create a model in Django? Or Can you name some model fields that you’ve created before during your projects? 
Answer. Models in django inherit from the models class. The class offers multiple fields to work with. Fields that I’ve used and are used extensively in any project are:
1.	CharField(max_length=128)(tell the interviewer that max_length parameter is not optional)
2.	ImageField() - tell them that the ImageField inherits from FileField()
3.	BooleanField() - tell them it’s best practise to use default value for boolean field.
4.	IntegerField() - Also mention the PositiveIntegerField()
5.	DateTimeField() - Tell them that you can pass auto_now_add=True as a parameter to get current timestamp saved into datetimefield()

Q#6. How would you check your django version?
Answer. Python -m django –version

Q#7. Can you use MySQL with Django?
Answer. Yes, you can. You can use, mysql, sqlite, oracle, postgresql etc

Q#9. What does makemigrations command do?
Answer. It creates migrations for the models that you define in models.py file.

Q#10. What popular websites use django? Can you name some?
Answer. Disqus, Instagram, Mozilla, NASA, The Washington Post etc.

Q#11. So you said, django follows MTV pattern. You mean django doesn’t follow MVC right?
Answer. MTV closely resembles MVC. Because, the framework handles the controller part itself so most things happen only in models, views and templates.

Q#13. Think of this scenario. You’re a django developer here. A big company, take Tesla as example, wants us to make them a website where the website handles all the feedback from the clients that are currently using tesla as their primary vehicle of transport. How would you make that type of website, sometimes, you might get 1000 reviews/feedbacks in an hour. How would you design the database too. Also tell about the security. If you know about front-end, what front-end technology would you prefer?

Anwer. Start by asking further questions and remove any doubt or question you have. Tell them how you would make it. When it comes to database design, explain all the fields that you are going to use. If the feedback is coming from unregistered clients than you might not know their location. In that case, you will determine the location using ip-location services and store the ip-address in GenericIPAddressField() field. Continue with more explanation and if you know any front-end technology than explain why would you prefer that particular technology instead of certain other technologies available in the market
