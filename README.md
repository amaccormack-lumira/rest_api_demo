rest_api_demo
=============

This is a sample RESTful API technical test.

## Software Test Engineer - Tech Test

### Instructions

Your team has been tasked with building a simple back-end for a blog. They have built a RESTful API to implement CRUD operations on this data. The endpoints are:

* GET /blog/categories/ - Returns list of blog categories
* POST /blog/categories/ - Creates a new blog category
* DELETE /blog/categories/{id} - Deletes blog category
* GET /blog/categories/{id} - Returns a category with a list of posts
* PUT /blog/categories/{id} - Updates a blog category

##### Additional endpoints
The following endpoints also exist to help you test the category endpoints above, but you do not need to provide tests to cover these

* GET /blog/posts/ - Returns list of blog posts
* POST /blog/posts/ - Creates a new blog post
* GET /blog/posts/archive/{year}/ - Returns list of blog posts from a specified year
* GET /blog/posts/archive/{year}/{month}/ - Returns list of blog posts from a specified month
* GET /blog/posts/archive/{year}/{month}/{day}/ - Returns list of blog posts from a specified day
* DELETE /blog/posts/{id} - Deletes blog post
* GET /blog/posts/{id} - Returns a blog post
* PUT /blog/posts/{id} - Updates a blog post

There is also a Swagger document which describes the API.

#### Testing report
The software engineers have now finished their initial development and the application is ready to be tested. Your task is to take the project, run it and test it. Use any testing tools that you think are appropriate for validating this black-box system. You will be evaluated on test coverage, readability and organisation of tests, and suggesting any improvements which could be made to the API.

#### Bug report(s)

So that the team can review any bugs found in their application, a simple bug report should be produced as a result of the testing process. This can be in any format you feel is appropriate.

#### Automation

If you are applying as an automation tester, please give an example of automating the running of some tests. You can use python or any other language or tool you are familiar with. If we need to install something to run your tests, please provide instructions as part of your submission.

### Install/setup of the app to test
In order to run the application, you need a copy of Python 3. Unfortuantely, it seems the latest version 3.10 has broken this app, so please use a slightly older version. This can be downloaded from:

https://www.python.org/downloads/release/python-399/

Linux installs may well already have a python 3 install. Some issues have been seen with this test on Ubuntu, where sqllite has not been set up OK, please contact us if you have these issues, or try another platform.

##### It is recommended that you select the "Add python to path" option in the python installer

A download for the project can be found at:

https://github.com/amaccormack-lumira/rest_api_demo/archive/refs/tags/techtest1.3.zip

Once downloaded, extract the zip file, and use a Command Prompt to open the extracted directory. Navigate into the appropriate folder. The API can then be run using the following commands:

```
cd path_to_workspace
cd rest_api_demo-techtest1.3
pip install virtualenv
```
(if you get errors, try using pip3 instead)

* On Windows (if you have both python 2 and python 3 installed, you may need to tell virtualenv the path to python3 install with -p option):
```
virtualenv venv
venv\Scripts\activate
```

* On Linux/MacOS: 
```
virtualenv -p `which python3` venv
source venv/bin/activate
```
Then, on all systems:
```
(venv) pip install -r requirements.txt
(venv) python setup.py develop
(venv) python rest_api_demo/app.py
```
(if you get errors, try using pip3 and python3 instead)

## And get testing...

You will then be able to open the swagger endpoints  to allow you access to the API documentation which can also be used for manual testing:

* http://localhost:8888/api/
* https://localhost:8889/api/

