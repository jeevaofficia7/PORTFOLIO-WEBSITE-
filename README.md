# PORTFOLIO-WEBSITE-
RESPONSIVE PORTFOLIO WEBSITE

<!DOCTYPE html>
<html lang="en">

<head>

    <!--style sheet-->
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: sans-serif;
            
        }

        body {
            background-color: rgb(0, 0, 90);
            color: white;
        }

        a {
            text-decoration: none;
        }

        #hamburger {
            display: flex;
            flex-direction: column;
            row-gap: 6px;
            display: none;
        }

        #hamburger .lines {
            height: 4px;
            width: 30px;
            background-color: white;
            margin-bottom: 4px;
        }

        /*style for header*/
        header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            background-color: red;
            padding: 20px 100px;
            margin-bottom: 100px;
        
        }

        /*stylew for navlinks */
        header #navlinks {
            list-style-type: none;
            display: flex;
            column-gap: 50px;
        
        }

        header #navlinks li a {
            color: white;
            font-weight: 600;
        }

        #navlinks i {
            color: orange;
        }

        #navlinks li a {
            padding: 12px;
        }

        #navlinks li a:hover {
            color: black;
        }

        /*style for logo*/
        #logo a {
            color: white;
            font-size: 20px;
            font-weight: 600;
            letter-spacing: 2px;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        }

        /*style for hero section..*/
        aside {
            display: flex;
            flex-direction: column;
            gap: 30px;
            align-items: center;
            text-align: center;
            margin: 30px;
        }

        aside p {
            text-align: center;
            padding: 10px;
            line-height: 1.6;
            font-size: 20px;

            width: 1000px;
        }

        aside button {
            padding: 20px 50px;
            background-color: red;
            border: none;
            color: white;
            border-radius: 50px;
        }

        aside #btns2 {
            display: flex;
            border: none;
            gap: 20px;
        }

        aside #btns2 button:hover {
            background-color: rgb(134, 8, 134);
        }

        i {
            margin-right: 10px;
        }

        main img {
            width: 400px;
            height: 400px;
            margin: 30px;
        }

        #projects {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            margin: 30px;
        }

        #projects img {
            width: 800px;
            height: 500px;
        }

        #projects p {
            padding: 10px;
            text-align: center;
            line-height: 1.6;
            width: 1200px;
        }

        #projects a {
            color: white;
            font-size: 60px;
            margin: 30px;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        }

        footer {
            display: flex;
            flex-direction: column;
            gap: 10px;
            align-items: center;
            background-color: #234;
            padding: 20px;
            width: 90%;
        }

        #footer a {
            text-decoration: none;
            color: white;
        }

        footer #footerlinks {
            list-style-type: none;
            display: flex;
            gap: 50px;
            justify-content: space-between;
            margin: 50px;
        }

        footer #footerlinks li a {
            color: white;
        }

        footer #social-link {
            list-style-type: none;
            display: flex;
            justify-content: space-between;
            gap: 50px;
            margin: 20px;
        }

        footer #social-link li a {
            text-decoration: none;
            color: white;
        }

        footer p {
            line-height: 1.6;
            padding: 10px 100px;
        }

        /*style for main*/
        section{
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 20px;
            margin: 40px;
            background-color: #222;
            padding: 50px;
            border: 1px solid white;
        
        }

        section article img{
            height: 300px;
            width: 500px;
            object-fit: cover;
        }

        section article{
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            gap: 30px;
        
        }

        section article p{
            font-size: 15px;
            width: 500px;
            text-align: center;
            line-height: 1.6;
        }

        section a{
            font-size: 20px;
            color: orange;
            font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
            font-weight: 600;
            letter-spacing: 2px;
        }

        section article button{
            padding: 12px;
            border-radius: 0;
        }

        .skill{
            font-size: 35px;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
            letter-spacing: 1px;
        }

        .change-color{
            background: black;
            color: white;
        }

        .change-color header{
            background-color: black;
        }

        /*------------Responsive design-------------------------*/

        @media screen and (max-width:1200px){
            
            header{
                display: flex;
                flex-direction: column;
                position: relative;
            }

            #navlinks{
                flex-direction: column;
                align-items: center;
                gap: 50px;
                margin: 50px;
                
            }

            #hamburger{
                display: block;
                position: absolute;
                right: 20px;
                top: 20px;

            }

            #togglebtns{
                position: absolute;
                left: 20px;
                top: 20px;
            }

            #navlinks li{
                width: 100%;
                padding: 10px 200px;
            
            }

            #navlinks li a{
                display: block;
                width: 100%;
            }

            #navlinks li:hover{
                background-color: orange;
                
            }

            img{
                height: 200px;
                width: 200px;
            }
            
            aside p{
                width: 600px;
                font-size: 15px;
            }

            #projects a{
                font-size: 30px;
            }

            #projects img{
                height: 300px;
                width: 300px;
                object-fit: cover;
            }

            #projects p{
                font-size: 12px;
                width: 700px;
                line-height: 2;
            }

            section{
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content:center ;
                gap: 20px;
            }

            footer{
                font-size: 15px;
            }

            #navlinks li{
                text-align: center;
            }

            #navlinks.active-class{
                display: none;
            }

            .change-color{
                background-color: black;
            }

            .change-color header{
                background-color: black;
            }
        }

        @media screen and (max-width:680px) {
            img{
                height: 200px;
                width: 200px;
            }

            

            #projects p{
                width: 600px;
                font-size: 12px
            }

            section{
                margin: 30px;
            }

            header{
                font-size: 15px;
                align-items: center;
                text-align: center;
            }

            header #navlinks li i{
                display: none;
            }
            

            footer #footerlinks{
                display: none;
            }
            
        }


        
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.1/css/all.min.css">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MY PORTFOLIO DEISGN</title>
    <link rel="icon" href="images/profile.png">
</head>

<body>
    <!--my project-->

    <!---header section-->
    <header>
        <!--hamburger menu-->
        <div id="hamburger">
            <div class="lines"></div>
            <div class="lines"></div>
            <div class="lines"></div>
        </div>
        <div id="logo">
            <a href="#">MY PORTFOLIO</a>
        </div>
        <!--NAVIGATION BAR-->
        <nav id="navigation">
            <ul id="navlinks">
                <li><a href="#"><i class="fas fa-house"></i>Home</a></li>
                <li><a href="#"><i class="fas fa-users"></i>Profile</a></li>
                <li><a href="#"><i class="fas fa-headset"></i>Support</a></li>
                <li><a href="#"><i class="fas fa-phone"></i>Contact</a></li>
                <li><a href="#"><i class="fas fa-lightbulb"></i>About</a></li>
            </ul>
        </nav>
        <div id="togglebtns">
            <i class="fas fa-sun" id="sun"></i>
        </div>
    </header>
    <!--hero section-->
    <aside>
        <img src="images/profile.png" height="300px" width="300px" alt="portfolio design">
        <h2>Iam Jeeva, This is My Portfolio Website</h2>
        <p>Iam a frontend Developer annd I have skills in HTML , CSS Javascript. I Enjoying creating Responsive web site
            using media queries and adding dynamic animation for enhnace user experience. Iam always ready to learn and
            improve my skills</p>
        <div id="btns2">
            <button>View deatils</button>
            <button>Contact</button>
            <button>Read More</button>
        </div>
        <main>
            
            <div id="projects">
                <h2>MY PROJECTS</h2>
                <a href="#"> RESPONSIVE RESTAURANT WEBSITE</a>
                <img src="images/street-cafe-terrace_1284-11404.jpg" height="300px" width="300px" alt="">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Autem sed eveniet odit doloremque ea culpa
                    iste, vel sequi rem placeat recusandae possimus cum saepe in, delectus rerum magni debitis ratione?
                    Commodi quod esse nesciunt deserunt eaque veritatis, ut tenetur ipsa nobis, pariatur nisi ipsam
                    suscipit placeat ducimus voluptatem. Voluptate, nam?</p>
                <a href="#">E COMMERCE WEBSITE</a>
                <img src="images/showing-cart-trolley-shopping-online-sign-graphic_53876-133967.avif" alt=""
                    height="300px" width="300px">
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Veniam commodi modi quo explicabo porro
                    consequatur nisi quasi dicta quod quisquam unde ea, eligendi nam accusamus. Earum commodi nihil
                    totam, cupiditate sed rerum expedita numquam neque reprehenderit delectus maxime autem natus optio
                    deleniti pariatur consectetur non possimus! Corrupti aliquid repellat necessitatibus!</p>
            </div>
        </main>
        <p class="skill">MY SKILLS <i class="fas fa-thumbs-up"></i></p>
        <section>
            <article>
                <a href="#">Programming skills <i class="fas fa-computer"></i></a>
                <img src="images/learn-programming-career-jpg.webp"  alt="">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. At eligendi illum sed explicabo dolore neque consequatur ullam magnam placeat. .</p>
                <button>CLICK HERE</button>
            </article>

            <!--article 2-->
            <article>
                <a href="#">Photography Skills <i class="fas fa-camera"></i></a>
                <img src="images/pho.webp"  alt="">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui omnis quidem similique dolorum possimus quod doloremque sint officia. </p>
                <button>CLICK HERE</button>
            </article>
            <!--article 3-->
            <article>
                <a href="#">Editing Works <i class="fas fa-computer"></i></a>
                <img src="images/course_10310_image.png"  alt="">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla corrupti dolor quam iste officiis. Consequatur, quisquam? Eius velit quo,.</p>
                <button>CLICK HERE</button>
            </article>
        </section>

        <footer>
            <nav id="footerlinks">
                <li><a href="#">Terms and conditions <i class="fas fa-tools"></i></a></li>
                <li><a href="#">Privacy policy</a></li>
                <li><a href="#">About us</a></li>
                <li><a href="#">Location <i class="fas fa-location"></i></a></li>
                <li><a href="#">Support and Enquries <i class="fas fa-headset"></i></a></li>
            </nav>
            <nav id="social-link">
                <li><a href="#"><i class="fab fa-google"></i></a></li>
                <li><a href="#"><i class="fab fa-facebook"></i></a></li>
                <li><a href="#"><i class="fab fa-whatsapp"></i></a></li>
                <li><a href="#"><i class="fab fa-instagram"></i></a></li>
            </nav>
            <p>
                JEEVA K <br>
                Rakkiyaplayam Kangayam Road Tiruppur.<br>
                Email:jeeva1293@gmail.com <br>
                Mobile:7550311563
            <p>
                <!--copyrights-->
            <p>&copy 2024 All rights reserved.</p>
        </footer>
</body>
<!--javacsript-->

<script>
    var hamburgerMenu = document.getElementById('hamburger');
    var navLinks = document.getElementById('navlinks');

    hamburgerMenu.addEventListener('click',()=>{
        navLinks.classList.toggle('active-class')
    })

    //for bgchange..

    var bgChange = document.getElementById('sun');

    bgChange.addEventListener('click',()=>{
        document.body.classList.toggle('change-color');
    })
</script>
</html>
