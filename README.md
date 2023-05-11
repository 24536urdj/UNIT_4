# UNIT_4
![Screen Shot 2023-04-13 at 8 58 44](https://user-images.githubusercontent.com/112072887/231611426-48d1189e-0f13-4a74-ae50-c36b0177bd73.png)

# Criteria A planning

### Problem definition
My client (who is currently a student in an ib school )has expressed  their worries about the amount of notes they need in order to revise and  understand the curriculum of all their subjects in order to pass successfully  the upcoming exams for both g11 and g12 , especially that they do not have time and sometimes the courage to ask other students to send them a lot of notes , therefore they requested a solution where different g11 and g12 from isak only and not other schools  can share their notes that will be categorized based on the subjects they take ,and can be accessed rapidly through filtering  which is why they eliminated facebook groups and other social network groups as a possible solution since it will be very hard to find the notes you need for their  own subjects and their  own level quickly, moreover taking into consideration that changement that happens to do curriculum and changement  of teachers,the client requested a way to keep the website updated regularly.
### Proposed solution 
Considering the requirements for the idea, an adequate solution is creating a social network website for  G11 isak students and G12 where the users can create an account and  share their notes in form of posts while also having the ability to view other users posts that will be organized in categories based on the subject and also ordered in a chronological way so that the user can access it easily and quickly. 
The social network  website  will be created  using  python , html and css because firstly python is  a multi-functionality language having capabilities to operate in multiple ways, that does not need a license and also easily understandable and usable  for the programmer.for html and css,as Both HTML and CSS are frequently used languages for web development  , also HTML uses a tag-based structure which is easy to understand even without any prior technical experience, and CSS uses a simplistic structure as well making the learning curve for mastery relatively easy; therefore it is more adequate for the developer of the website who is more comfortable with these languages than others like java scripts and in order to keep it organized and fulfill the success criteria , I will use sql to associate a database to the website because it's portability makes it a convenient option for users, as they can transfer it from one device to another with no issues. It processes queries quickly. No matter how large data might be, SQL can retrieve it quickly and efficiently.[^3] so that the  client will be able to add, withdraw and edit the notes shared.
### Design statement
Taking into consideration the client's requirements and need , I will design this notes sharing  website using python, html, css , javascript , sqlite and flask , therefore it will take  me 4 weeks to develop it .
At the end ,The effectiveness of the website will be evaluated using the success criterias below.

### Success Criteria 
1. [issue tackled : enable only isak students to access the website ]: The solution needs to have a login and a registration system.
2. [issue tackled :  having access to other students posts ]The solution needs to be able to classify updated notes into directories based on their subjects.
3. [issue tackled :  rapid access to notes]The solution needs to be able to keep  the notes posts  organized and easily to follow by classifying them in categories based on their subjects.
4. [issue tackled : notes sharing between isak students ]The solution needs to enable the client to add new posts 
5. [issue tackled : update the notes so that it harmonizes with the curriculum of the year]The solution needs to enable the client to delete unwanted posts.
6.[issue tackled :  organization of the posts ] The solution needs to have a menu where notes are categorized into subjects such as category for english lang-lit , History and Computer sciene.



# Criteria B 
## System diagram

![Screen Shot 2023-05-10 at 20 50 12](https://github.com/24536urdj/UNIT_4/assets/112072887/50d90601-ea5a-4e1e-a991-711a20dbf4b5)

fig_: 
the system diagram  visually illlustrates the components of the programmes and the relations they hold with each others.
The program is created using pycharm and python, moreover. all the data issued will be stored in an sqlite database.finally the website will get some inputs from the user and send them back to the program which will help in outputting new data and display on the website. 
## Wireframe diagram 
![Screen Shot 2023-05-10 at 21 43 54](https://github.com/24536urdj/UNIT_4/assets/112072887/0238fd30-11e7-48de-9735-af2a79ee60cd)

## ER diagram 
![Screen Shot 2023-05-11 at 16 30 52](https://github.com/24536urdj/UNIT_4/assets/112072887/8a00a3e7-ee46-43e0-b337-e4e03785b3da)
fig_:  
As it seen I have only created one database table called USERS in which I stored the user's registration and login information.
The USERS data table contains id which automatically added as it is a primary key integer,name column in which the name of the user is stored,email column which  also stores the user's email address. Furthermore i have also added the password column where the passowrd of the user is stored , therefore it ensures the security of the login system.


## Flow chart 

https://drive.google.com/file/d/1hwkE0FZ1w6jCV-ABtu-T_lTO2caMC96m/view?usp=share_link
fig_:
since the client wants the notes to be organized in categories based on their subject,i have created a code for it that is represented by  the following flow chart which shows in plain english  the code used to get all the files in a directory by just entering its path in pycharm project "flaskProject" this will enable to insert the files in a database and therefore display it on the website just as the client wanted.
## UML Diagram : 
![Screen Shot 2023-05-09 at 16 01 44](https://user-images.githubusercontent.com/112072887/237019586-e0c3efa1-16b8-49bf-8954-fde620ba5da5.png)

This Unified Modeling Language diagram shows the class used in programing the website, the class is called database_worker and it is responsible to manage as an example executing the queries , and closing the database along with many other  different databse interactions that they handle.

## Test Plan
| Description                 | Type             | Inputs                                                                                                                                              | Outputs                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|-----------------------------|------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| login system         | Unit test        | 1. Run the python file app.py 2.open the webiste . Click login button on the login_page 3. Input information in each textfield following the hint text 4. Click login | If the username is wrong:an error hint_text  will say the username is wrong. If password is wrong :an error hint_text will appear saying the password is wrong don't match: the message will say that password doesn't match. If entering the right password and username : successfully it will take you to the main page.                                                                                                                                                                                                                          |
|  Add new file       | Unit test        | 1. run the python file app.py 2. login  3. press file button create a post on the main_page  4.click the button choose file  5.select a file that conatins the notes you want to share  6.enter in the text field next to the button the subject of the note (as an example English) 7.press the button submit 8. go back to the pycharm and select flask project 9. go to directory Englis 10. see if the file you choose was added there                                              | the file name need to be correct and exist in the directory of the subject chosen 
| login system     | Unit test        | 1. run the python file app.py 2. open the website . clik signup button. sign up. then go to the sql databse called social.db in pycharm.select the table called USERS. check if the registration information exists in the table                     |the information need to be in the appropriate row and also identical to what the user entered 


## Task Record 

| | Planned Action                 | Planned outcome            | time estimate                                                                                                                                             | target completion date|              Criterion                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|-----|-----------------------------|------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------|
| 1  | Code the about_me page    : development                         | programming the about_me page using  python and pycharm,              | 60 minutes    | 4 april        | C       |
| 2  | add the post function :  development                           | add a function that will allow the user to post their notes .                                                |   30 minutes    | 5 april         | C        |
| 3  |Create a database for the user and their posts   : development                          | create using sql a database called social_networok that conatins two tables one for users and one for posts  |5 minutes        | 7 april           | C       |
| 4  | Write down the problem definition           : planning                    | state a detailed version of the problem                       |  40 minutes    | 13 april         | A        |
| 5  | Write down the proposed solution with justification of tools implied : planning | Reasearch and evaluation of solutions to choose an adequate one                                       | 30 min     | 17 april        | A        |
| 6 | Write down the success criterias : planning  | Choosing important feature of the website that will show how successful or unsuccessful the website is                                      | 30 min     | 17 april        | A        |
| 7 | Rewrite the problem definition : planning  | Add more details to the problem definition in order to stte clearly the main issue                                | 20 min     | 19 april        | A        |
| 8 | Code the main page : development  |     programming the main page using  python and pycharm                              | 30 min     | 21 april        | C      |
| 9 | Code the posts page : development  |     programming the posts page using  python and pycharm                              | 30 min     | 21 april        | C      |
| 10 |  menu bar: development   | use the header attribute to add a menu bar so that students can naviagte the website easily                                 | 5 min     | 21 april        | C      |
| 11 |  Login and registration page: development   | use transition method in  javascript html and css in order to create a login and registration page                                |      45 min     | 24 april        | C      |
| 12 |  the post creation page : development   | programming a page where the client can add their own notes as posts                                 | 45 min     | 26 april        | C      |
| 13|  flowcharts  : design  | create the first flow chart that shows  the code that classifies    files into categories                            | 20 min     | 07 May       | B     |
| 14|  UML diagram  : design | create the UML diagram that shows visually the classes contained in the code                            |  10 min     | 09 May       | B     |
| 15| Database table : development   | create a database table to insert the English subject  files uploaded by the client                             | 5 min     | 09 May       | C     |
| 16| Database table : development   | delete the database table used to insert the English subject  files uploaded by the client                             | 5 min     | 09 May       | C     |
| 17|Subject posts : development  | create a web page for each subject and upload the files shared in it                            | 5 min     | 10  May       | C     |
| 18| Wireframe diagram : design   | create a wireframe diagram to show a general view to the client of how would the website look like                         | 30 min     | 10 May       | C     |
| 19| flow chart : design   | create the second  flow chart that shows  the code with which i connect to sql database                            | 20 min     | 10 May       | C     |
| 20| explain code  : development    | add other parts of the code and explain the way it was developed                        | 20 min     | 10 May       | C     |
| 21| draw the ER diagram : design    | draw an entity relation diagram that shows the databases used in the process and the relationship they have with each others      | 20 min     | 10 May       | C     |
| 22| draw the ER diagram : design    | draw an entity relation diagram that shows the databases used in the process and the relationship they have with each others      | 20 min     | 10 May       | C     |
















# Criteria C: Developement 
## List of Techniques 
1.  Python 
2.  Html along with Java script inside some html files 
3.  CSS 
5.  Flask library
6.  SQlite 
7.  If statement 
8.  Functions 
9.  OS module
10. Werkzeug library
11. my_lib library 
12. Variables



## success criteria (3): posts need to be organized based on the subject
```.py 
@app.route('/index', methods=['GET', 'POST'])
def index():
    if request.method == 'POST':
      
        f = request.files['file']
     
        
        subject = request.form['subject']

       
        if subject == "English":


            f.save(f"English/{f.filename}")
        else :
            if subject == "Computer science":
                f.save(f"Computer science/{f.filename}")
            else:
                if subject == "Global politics":
                    f.save(f"Global politics/{f.filename}")
                else :
                    if subject == "Biology":
                        f.save(f"Biology/{f.filename}")
                    else:
                        if subject == "History":
                            f.save(f"History/{f.filename}")
                        else :
                            f.save(f"files/{f.filename}")


    return render_template("index.html")
    return render_template("acknowledgement.html")
```
Fig_:
In order to ensure that the posts are keeping organized and rapidly accessible, I created a python code that classifies the notes based on their subjects.
As shown above , firstly I have used flask route in order to create the url that takes the user to the website while specifying the methods allowed . I have also used if statement firstly to get the file that contains the note and also its subject, afterwards I have also created an if statement and the save function so that the files are classified  and saved in pycharm directories based on the subject they belong too , otherwise if they do not belong to any of the subjects available then they will be saved in a general directories called files, as an example if the subject is English then the file chosen will be saved in the directory called English 
## connect to sql database 
```.py 
class database_worker:
    def __init__(self,name):
        self.connection = sqlite3.connect(name)
        self.cursor = self.connection.cursor()
    def search(self,query):
        result= self.cursor.execute(query).fetchall()
        return result

    def run_save(self,query):
        self.cursor.execute(query)
        self.connection.commit()

    def close(self):
        self.connection.close()

```
fig_: 
the python code enables to connect to an sql database throught as seen firstly creating a class called database_worker 
where we define two functions the __init__ function which allows the class databse_worker to initialize the attributes of the class.
the function search allows  to see if your information provided in the self-query order form matches information in the database
moreover the run_save function allows to run the sql query and save the data.
the close function allow us to close the database after the query was executed 

## 
```.py
<!DOCTYPE html>
<head lang="en">
        <meta charset="UTF-8">
        <link rel="stylesheet"href="/static/my_style.css">
</head>
<body>
<div class="navbar">
    <a href="#home">Home</a>
    <a href="#news">News</a>
    <div class="dropdown">
        <button class="dropbtn">Subjects
            <i class="fa fa-caret-down"></i>
        </button>
        <div class="dropdown-content">
            <a href="/login_page">English A&B</a>
            <a href="#">History HL&SL</a>
            <a href="econ">Economics</a>
            <a href="#">Global politics</a>
            <a href="/biology_page">Biology</a>

        </div>
        </div>
```
fig_:
this an html code used to create a menu bar and also a drop down navigation bar which allows the user to serach directly for the sun¥bject they would like to take notes of.
the code was built as follow: create a section in the html document then inside it I added another section with a class called dropdown , inside it I have also added button tag which  defines a clickable button, afterwards I have a added inside it class "fa fa-caret-down" so that once the user clicks the button subject the list of subjects will drop down. furthermore I have added another section that shows the drop down content  then    the <a> tag which defines a hyperlink, that is used to link from one page to another. as an example if the client click on the economic button  then it will take you to the web page called econ which displays notes for ib economics.
















### Work cited 
[^3]: https://www.businessnewsdaily.com/5804-what-is-sql.html#:~:text=Its%20portability%20makes%20it%20a,retrieve%20it%20quickly%20and%20efficiently.

