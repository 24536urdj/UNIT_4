# UNIT_4
![Screen Shot 2023-04-13 at 8 58 44](https://user-images.githubusercontent.com/112072887/231611426-48d1189e-0f13-4a74-ae50-c36b0177bd73.png)

# Criteria A planning

### Problem definition
My client (who is currently a student in an ib school )has expressed  their worries about the amount of notes they need in order to revise and  understand the curriculum of all their subjects in order to pass successfully  the upcoming exams for both g11 and g12 , especially that they do not have time and sometimes the courage to ask other students to send them a lot of notes , therefore they requested a solution where different g11 and g12 from isak only and not other schools  can share their notes that will be categorized based on the subjects they take ,and can be accessed rapidly through filtering  which is why they eliminated facebook groups and other social network groups as a possible solution since it will be very hard to find the notes you need for their  own subjects and their  own level quickly, moreover taking into consideration that changement that happens to do curriculum and changement  of teachers,the client requested a way to keep the website updated regularly.
### Proposed solution 
Considering the requirements for the idea, an adequate solution is creating a social network website for  G11 isak students and G12 where the users can create an account and  share their notes in form of posts while also having the ability to view other users posts that will be organized in categories based on the subject and also ordered in a chronological way so that the user can access it easily and quickly. 
The social network  website  will be created  using  python , html and css because firstly python is  a multi-functionality language having capabilities to operate in multiple ways, that does not need a license and also easily understandable and usable  for the programmer.for html and css,as Both HTML and CSS are frequently used languages for web development  , also HTML uses a tag-based structure which is easy to understand even without any prior technical experience, and CSS uses a simplistic structure as well making the learning curve for mastery relatively easy; therefore it is more adequate for the developer of the website who is more comfortable with these languages than others like java scripts and in order to keep it organized and fulfill the success criteria , I will use sql to associate a database to the website because it's portability makes it a convenient option for users, as they can transfer it from one device to another with no issues. It processes queries quickly. No matter how large data might be, SQL can retrieve it quickly and efficiently.[^3] so that the  client will be able to add, withdraw and edit the notes shared.
### Success Criteria 
1. [issue tackled : enable only isak students to access the website ]: The solution needs to have a login and a registration system.
2. [issue tackled :  having access to other students posts ]The solution needs to contain a page where client can see all posts 
3. [issue tackled :  rapid access to notes]The solution needs to be able to keep  the notes posts  organized and easily to follow by providing a filtering button 
4. [issue tackled : notes sharing between isak students ]The solution needs to enable the client to add new posts 
5. [issue tackled : update the notes so that it harmonizes with the curriculum of the year]The solution needs to enable the client to delete unwanted posts.
6.[issue tackled :  organization of the posts ] The solution needs to have a menu where notes are categorized into subjects such as category for english lang-lit , History and Computer sciene.

## Task Record 

|    | Planned Action                                        | Planned Outcome                                                                            | Design Cycle   | Time Estimate | Target Completion | Criteria |
|----|-------------------------------------------------------|--------------------------------------------------------------------------------------------|----------------|---------------|-------------------|----------|
| 1  | Code the about_me page                            | programming the about_me page using  python and pycharm,              | Development       | 60 minutes    | 4 april        | C       |
| 2  | add the post function                           | add a function that will allow the user to post their notes .                                                | Development      | 30 minutes    | 5 april         | C        |
| 3  |Create a database for the user and their posts                            | create using sql a database called social_networok that conatins two tables one for users and one for posts  |Development       | 5 minutes        | 7 april           | C       |
| 4  | Write down the problem definition                              | state a detailed version of the problem                       | Planning       | 40 minutes    | 13 april         | A        |
| 5  | Write down the proposed solution with justification of tools implied | Reasearch and evaluation of solutions to choose an adequate one                                   | Planning       | 30 min     | 17 april        | A        |
| 6 | Write down the success criterias  | Choosing important feature of the website that will show how successful or unsuccessful the website is                                   | Planning       | 30 min     | 17 april        | A        |
| 7 | Rewrite the problem definition  | Add more details to the problem definition in order to stte clearly the main issue                                | Planning       | 20 min     | 19 april        | A        |
| 8 | Code the main page  |     programming the main page using  python and pycharm                              | Development        | 30 min     | 21 april        | C      |
| 9 | Code the posts page  |     programming the posts page using  python and pycharm                              | Development        | 30 min     | 21 april        | C      |
| 10 |  menu bar  | use the header attribute to add a menu bar so that students can naviagte the website easily                                 | Development        | 15 min     | 21 april        | C      |
| 11 |  Login and registration page  | use transition method in  javascript html and css in order to create a login and registration page                                | Development        | 45 min     | 24 april        | C      |
| 12 |  the post creation page   | programming a page where the client can add their own notes as posts                                 | Development        | 45 min     | 26 april        | C      |



# Criteria C: Developement 

## success criteria (2): posts page html code 
```.py 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    {% if title %}
    <title>{{ title }}</title>
    {% else %}
    <title> Welcome </title>
    {%  endif%}
    <link rel="stylesheet"href="/static/my_css.css">
</head>
<body>
<div class="container cta-100 ">
    <div class="container">
        <div class="row blog">
            <div class="col-md-12">
                <div id="blogCarousel" class="carousel slide container-blog" data-ride="carousel">
                    <ol class="carousel-indicators">
                        <li data-target="#blogCarousel" data-slide-to="0" class="active"></li>
                        <li data-target="#blogCarousel" data-slide-to="1"></li>
                    </ol>
                    <!-- Carousel items -->
                    <div class="carousel-inner">
                        <div class="carousel-item active">
                            <div class="row">
                                <div class="col-md-4" >
                                    <div class="item-box-blog">
                                        <div class="item-box-blog-image">
                                            <!--Date-->
                                            <div class="item-box-blog-date bg-blue-ui white"> <span class="mon">Augu 01</span> </div>
                                            <!--Image-->
                                            <figure> <img alt="" src="https://pixabay.com/get/g9fecae00b48af6ad3638a7c7a96aba1aff5a92fe390044699ed53d8a48e5ff99bdc2cb3e8ac8f552db2e8926f8003afd_1280.jpg"> </figure>
                                        </div>
                                        <div class="item-box-blog-body">
                                            <!--Heading-->
                                            <div class="item-box-blog-heading">
                                                <a href="#" tabindex="0">
                                                    <h5>News Title</h5>
                                                </a>
                                            </div>
                                            <!--Data-->
                                            <div class="item-box-blog-data" style= background-color:lightcyan;">
                                                <p><i class="fa fa-user-o"></i> Admin, <i class="fa fa-comments-o"></i> Comments(3)</p>
                                            </div>
                                            <!--Text-->
                                            <div class="item-box-blog-text">
                                                <p>Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, consectetuer adipiscing. Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, consectetuer adipiscing. Lorem ipsum dolor.</p>
                                            </div>
                                            <div class="mt"> <a href="#" tabindex="0" class="btn bg-blue-ui white read">read more</a> </div>
                                            <!--Read More Button-->
                                        </div>
                                    </div>
                                </div>
                                <div class="col-md-4" >
                                    <div class="item-box-blog">
                                        <div class="item-box-blog-image">
                                            <!--Date-->
                                            <div class="item-box-blog-date bg-blue-ui white"> <span class="mon">Augu 01</span> </div>
                                            <!--Image-->
                                            <figure> <img alt="" src="guten.png"> </figure>
                                        </div>
                                        <div class="item-box-blog-body">
                                            <!--Heading-->
                                            <div class="item-box-blog-heading">
                                                <a href="#" tabindex="0">
                                                    <h5>News Title</h5>
                                                </a>
                                            </div>
                                            <!--Data-->
                                            <div class="item-box-blog-data" style="background-color: lightcyan;">
                                                <p><i class="fa fa-user-o"></i> Admin, <i class="fa fa-comments-o"></i> Comments(3)</p>
                                            </div>
                                            <!--Text-->
                                            <div class="item-box-blog-text">
                                                <p>Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, consectetuer adipiscing. Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, consectetuer adipiscing. Lorem ipsum dolor.</p>
                                            </div>
                                            <div class="mt"> <a href="#" tabindex="0" class="btn bg-blue-ui white read">read more</a> </div>
                                            <!--Read More Button-->
                                        </div>
                                    </div>
                                </div>
                                <div class="col-md-4" >
                                    <div class="item-box-blog">
                                        <div class="item-box-blog-image">
                                            <!--Date-->
                                            <div class="item-box-blog-date bg-blue-ui white"> <span class="mon">Augu 01</span> </div>
                                            <!--Image-->
                                            <figure> <img alt="" src="guten.png"> </figure>
                                        </div>
                                        <div class="item-box-blog-body">
                                            <!--Heading-->
                                            <div class="item-box-blog-heading">
                                                <a href="#" tabindex="0">
                                                    <h5>News Title</h5>
                                                </a>
                                            </div>
                                            <!--Data-->
                                            <div class="item-box-blog-data" style="background-color: lightcyan;">
                                                <p><i class="fa fa-user-o"></i> Admin, <i class="fa fa-comments-o"></i> Comments(3)</p>
                                            </div>
                                            <!--Text-->
                                            <div class="item-box-blog-text">
                                                <p>Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, consectetuer adipiscing. Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, consectetuer adipiscing. Lorem ipsum dolor.</p>
                                            </div>
                                            <div class="mt"> <a href="#" tabindex="0" class="btn bg-blue-ui white read">read more</a> </div>
                                            <!--Read More Button-->
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <!--.row-->
                        </div>
                        <!--.item-->
                        <div class="carousel-item ">
                            <div class="row">
                                <div class="col-md-4" >
                                    <div class="item-box-blog">
                                        <div class="item-box-blog-image">
                                            <!--Date-->
                                            <div class="item-box-blog-date bg-blue-ui white"> <span class="mon">Augu 01</span> </div>
                                            <!--Image-->
                                            <figure> <img alt="" src="guten.png"> </figure>
                                        </div>
                                        <div class="item-box-blog-body">
                                            <!--Heading-->
                                            <div class="item-box-blog-heading">
                                                <a href="#" tabindex="0">
                                                    <h5>News Title</h5>
                                                </a>
                                            </div>
                                            <!--Data-->
                                            <div class="item-box-blog-data" style="background-color: lightcyan;">
                                                <p><i class="fa fa-user-o"></i> Admin, <i class="fa fa-comments-o"></i> Comments(3)</p>
                                            </div>
                                            <!--Text-->
                                            <div class="item-box-blog-text">
                                                <p>Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, consectetuer adipiscing. Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, consectetuer adipiscing. Lorem ipsum dolor.</p>
                                            </div>
                                            <div class="mt"> <a href="#" tabindex="0" class="btn bg-blue-ui white read">read more</a> </div>
                                            <!--Read More Button-->
                                        </div>
                                    </div>
                                </div>
                                <div class="col-md-4" >
                                    <div class="item-box-blog">
                                        <div class="item-box-blog-image">
                                            <!--Date-->
                                            <div class="item-box-blog-date bg-blue-ui white"> <span class="mon">Augu 01</span> </div>
                                            <!--Image-->
                                            <figure> <img alt="" src="guten.png"> </figure>
                                        </div>
                                        <div class="item-box-blog-body">
                                            <!--Heading-->
                                            <div class="item-box-blog-heading">
                                                <a href="#" tabindex="0">
                                                    <h5>News Title</h5>
                                                </a>
                                            </div>
                                            <!--Data-->
                                            <div class="item-box-blog-data" style="background-color: lightcyan">
                                                <p><i class="fa fa-user-o"></i> Admin, <i class="fa fa-comments-o"></i> Comments(3)</p>
                                            </div>
                                            <!--Text-->
                                            <div class="item-box-blog-text">
                                                <p>Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, consectetuer adipiscing. Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, consectetuer adipiscing. Lorem ipsum dolor.</p>
                                            </div>
                                            <div class="mt"> <a href="#" tabindex="0" class="btn bg-blue-ui white read">read more</a> </div>
                                            <!--Read More Button-->
                                        </div>
                                    </div>
                                </div>
                                <div class="col-md-4" >
                                    <div class="item-box-blog">
                                        <div class="item-box-blog-image">
                                            <!--Date-->
                                            <div class="item-box-blog-date bg-blue-ui white"> <span class="mon">Augu 01</span> </div>
                                            <!--Image-->
                                            <figure> <img alt="" src="guten.png"> </figure>
                                        </div>
                                        <div class="item-box-blog-body">
                                            <!--Heading-->
                                            <div class="item-box-blog-heading">
                                                <a href="#" tabindex="0">
                                                    <h5>News Title</h5>
                                                </a>
                                            </div>
                                            <!--Data-->
                                            <div class="item-box-blog-data" style="background-color: lightcyan;">
                                                <p><i class="fa fa-user-o"></i> Admin, <i class="fa fa-comments-o"></i> Comments(3)</p>
                                            </div>
                                            <!--Text-->
                                            <div class="item-box-blog-text">
                                                <p>Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, consectetuer adipiscing. Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, adipiscing. Lorem ipsum dolor sit amet, consectetuer adipiscing. Lorem ipsum dolor.</p>
                                            </div>
                                            <div class="mt"> <a href="#" tabindex="0" class="btn bg-blue-ui white read">read more</a> </div>
                                            <!--Read More Button-->
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <!--.row-->
                        </div>
                        <!--.item-->
                    </div>
                    <!--.carousel-inner-->
                </div>
                <!--.Carousel-->
            </div>
        </div>
    </div>
</div>


```
## Css code for the posts page 
```.py 
* {
  box-sizing: border-box;
}

body {
  font-family: Arial;
  padding: 20px;
  background: #f1f1f1;
}

/* Header/Blog Title */
.header {
  padding: 100px;
  font-size: 40px;
  text-align: center;
  background: white;
  background-image: url("MOI.png");
  background-repeat: repeat;
  background-size: 700px;
}

/* Create two unequal columns that floats next to each other */
/* Left column */
.leftcolumn {
  float: left;
  width: 75%;
}

/* Right column */
.rightcolumn {
  float: left;
  width: 25%;
  padding-left: 20px;
}

/* Fake image */
.fakeimg {
  background-color: #aaa;
  width: 100%;
  padding: 20px;

}
.fakeimga {
  background-image: url("mira.png");
  background-repeat: no-repeat;
  height: 30px;
  width: 300px;
  padding: 50px;

}



/* Add a card effect for articles */
.card {
  background-color: white;
  padding: 20px;
  margin-top: 20px;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Footer */
.footer {
  padding: 10px;
  text-align: center;
  background: black;
  margin-top: 10px;
  -webkit-text-fill-color: white;
}

/* Responsive layout - when the screen is less than 800px wide, make the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 800px) {
  .leftcolumn, .rightcolumn {
    width: 100%;
    padding: 0;
  }
}
/* Add a black background color to the top navigation */
.topnav {
  background-color: #333;
  overflow: hidden;
}

/* Style the links inside the navigation bar */
.topnav a {
  float: left;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

/* Change the color of links on hover */
.topnav a:hover {
  background-color: #ddd;
  color: black;
}

/* Add a color to the active/current link */
.topnav a.active {
  background-color: black;
  color: white;
}
```

The code above shows the way in which the posts page was developed using html and css.
In the html file: 
In the Css file : 


##Success criteria  Menu bar html and Css code :
 Html code : 
 ```.py 
 <!DOCTYPE html>
<head lang="en">
    <div class="topnav">
        <a class="active" href="#home">Home</a>
        <a href="#Posts">Posts</a>
        <a href="#contact">Contact</a>
        <a href="#Register"> Register </a>
    </div>
    <head>
        <meta charset="UTF-8">
        <link rel="stylesheet"href="/static/my_style.css">
    </head>
 ```
 Css code : 
 ```.py 
 .topnav {
  background-color: #333;
  overflow: hidden;
}

/* Style the links inside the navigation bar */
.topnav a {
  float: left;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

/* Change the color of links on hover */
.topnav a:hover {
  background-color: #ddd;
  color: black;
}

/* Add a color to the active/current link */
.topnav a.active {
  background-color: black;
  color: white;
}
 ```




















### Work cited 
[^3]: https://www.businessnewsdaily.com/5804-what-is-sql.html#:~:text=Its%20portability%20makes%20it%20a,retrieve%20it%20quickly%20and%20efficiently.

