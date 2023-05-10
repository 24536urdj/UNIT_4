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
2. [issue tackled :  having access to other students posts ]The solution needs to contain a page where client can see all posts 
3. [issue tackled :  rapid access to notes]The solution needs to be able to keep  the notes posts  organized and easily to follow by classifying them in categories based on their subjects.
4. [issue tackled : notes sharing between isak students ]The solution needs to enable the client to add new posts 
5. [issue tackled : update the notes so that it harmonizes with the curriculum of the year]The solution needs to enable the client to delete unwanted posts.
6.[issue tackled :  organization of the posts ] The solution needs to have a menu where notes are categorized into subjects such as category for english lang-lit , History and Computer sciene.



# Criteria B 
## System diagram

![Uploading Screen Shot 2023-05-10 at 20.50.12.png…]()

## Flow chart 

https://drive.google.com/file/d/1hwkE0FZ1w6jCV-ABtu-T_lTO2caMC96m/view?usp=share_link
## UML Diagram : 
![Screen Shot 2023-05-09 at 16 01 44](https://user-images.githubusercontent.com/112072887/237019586-e0c3efa1-16b8-49bf-8954-fde620ba5da5.png)



## Test Plan
| Description                 | Type             | Inputs                                                                                                                                              | Outputs                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|-----------------------------|------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| login system         | Unit test        | 1. Run the python file app.py 2. Click login button on the login_page 3. Input information in each textfield following the hint text 4. Click login | If the username is wrong:an error hint_text  will say the username is wrong. If password is wrong :an error hint_text will appear saying the password is wrong don't match: the message will say that password doesn't match. If entering the right password and username : successfully it will take you to the main page.                                                                                                                                                                                                                          |
|  Add new file       | Unit test        | 1. run the python file app.py 2. login  3. press file button create a post on the main_page  4.click the button choose file  5.select a file that conatins the notes you want to share  6.enter in the text field next to the button the subject of the note (as an example English) 7.press the button submit 8. go back to the pycharm and select flask project 9. go to directory Englis 10. see if the file you choose was added there                                              | the file name need to be correct and exist in the directory of the subject chosen 


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



















### Work cited 
[^3]: https://www.businessnewsdaily.com/5804-what-is-sql.html#:~:text=Its%20portability%20makes%20it%20a,retrieve%20it%20quickly%20and%20efficiently.

