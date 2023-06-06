# EXP 01 - PORTFOLIO

## AIM:

To create a portfolio using HTML and CSS

## SOFTWARE:

Visual Studio Code.

## ALGORITHM:

1. Set up the basic structure of your HTML document.

2. Create a CSS file named "styles.css" and link it to your HTML document. This file will contain the CSS rules for styling your portfolio.

3. Design the layout of your portfolio using HTML elements such as < header >, < nav >, < section >, < article >, and < footer >. Use appropriate classes or IDs to style these elements later with CSS.

4. Add a header section to display your name or the title of your portfolio.

5. Add images or media to enhance your portfolio. You can use the <img> tag to display images and embed videos or other media using appropriate HTML tags.

6. Apply responsive design techniques to ensure your portfolio looks good on different devices and screen sizes. Use CSS media queries to adjust the layout and styling as needed.

7. Apply CSS styling to your portfolio elements by targeting their respective classes or IDs in the "styles.css" file. Customize the colors, fonts, spacing, and other visual properties to match your desired design.

## CODE:

### HTML CODE:

```java
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PERSONAL PORTFOLIO</title>
    <link rel="stylesheet" href="1.css">
</head>
<body>
    <nav class="navbar">
        <ul>
            <li><a herf="#home">HOME</a></li>
            <li><a herf="#about">ABOUT ME</a></li>
            <li><a herf="#education">EDUCATION</a></li>
            <li><a herf="#portfolio">PORTFOLIO</a></li>
            <li><a herf="#contact">CONTACT ME</a></li>
        </ul>
    </nav>

    <section id="home">
        <h1 class="heading"> HI, I AM</h1>
        <h1 class="heading"> MONISHA </h1>
        <br>
        
    </section>

    <section id="about">
        <h1 class="heading">ABOUT ME</h1>
        <br>
        <br>
        <div class="about">
            <img src="bg.jpg" alt="my pic">
            <div class="name">
                
                <br>
                <br>
                <p>AI/ML specialists work with a range of data types, including structured and unstructured data, and use various techniques such as neural networks, decision trees, and clustering to analyze and make predictions based on that data. They also work with large datasets, using tools like Hadoop, Spark, and SQL to extract, transform, and load data for analysis.In addition to technical skills, AI/ML specialists need to have a solid understanding of statistics, mathematics, and computer science. They should be able to communicate complex technical concepts to non-technical stakeholders and work collaboratively with teams to develop and implement AI/ML solutions that solve real-world business problems.<br>AI/ML specialists are in high demand across industries such as finance, healthcare, marketing, and e-commerce, as companies seek to leverage the power of AI to gain a competitive advantage. To become an AI/ML specialist, one typically needs to have a strong foundation in computer science, mathematics, and statistics, as well as experience working with AI/ML tools and technologies.</p>
            </div>
        </div>
     </section>

     <section id="education">
        <h1 class="heading">EDUCATION</h1>

        <div class="columns">
            <div class="box">
                <h2>BACHELORS IN AIML</h2>
                <p><I>Artificial Intelligence and Machine Learning which aims to develop a strong foundation by using the principles and technologies that consist of many facets of Artificial Intelligence including logic, knowledge representation, probabilistic models, and machine learning. This course is best suited for students seeking to build world-class expertise in Artificial Intelligence and Machine Learning</I></p>
            </div>
            <div class="box" >
                <h2>MASTERS IN AIML</h2>
                <p><I>The Master of Artificial Intelligence in Business is a unique 2-year full-time interdisciplinary program that will cover AI's foundations, principles, and techniques and business subjects such as economics, accounting, finance, and marketing. In addition to learning the theory, students will work on many projects that apply AI to practical problems in retail, manufacturing, finance, and many other businesses.</I></p>
            </div>
            <div class="box">
                <h2>P.H.D IN AIML</h2>
                <p><I>Earn a doctorate degree in Artificial Intelligence, help lead innovation in a growing industry. The PhD in Artificial Intelligence is centered upon how computers operate to match the human decision making process in the brain.</I></p>
            </div>
            <div class="box">
                <h2>RESEARCH IN AIML</h2>
                <p><I>A computer-generated simplification of something that exists in the real world, such as climate change, disease spread, or earthquakes. Machine learning systems develop models by analyzing patterns in large data sets. Models can be used to simulate natural processes and make predictions.</I></p>
            </div>
            
        </div>
     </section>

    <section id="portfolio">
        <h1 class="heading">PORTFOLIO</h1>
        <div class="gallery">
        <img src="img1.jpg" alt="">
        <img src="img2.jpg" alt="">
        <img src="img3.jpg" alt="">
    </div>
         </section>

         <section id="contact">
            <h1 class="heading">CONTACT ME</h1>
            <br>
            <form action="" class="form">
                <input type="text" name="name" class="input" placeholder="Enter Your name">
                <input type="text" name="email" class="input" placeholder="Enter Your Email">
                <textarea name="message" id="message" cols="70" rows="20" placeholder="Enter Your Message"></textarea>
                <input type="submit" value="submit" id="submit">
            </form>
         </section>
</body>
</html>
```

### CSS CODE:

```
*{
    margin: 0;
    padding: 0;
}
html{
    scroll-behavior: smooth;
}
.navbar{
    display : flex;
    justify-content: center;
    height: 50px;
    align-items: center;
    position: sticky;
    top: 0;
}
.navbar::before{
    content: "";
    position: absolute;
    background-color: rgba(0,0,0,0.5);
    height: 100%;
    width: 100%;
    z-index: -1;
}
.navbar ul{
    display : flex;
    list-style: none;
}
.navbar ul li{
    font-size: 1.1rem;
}
.navbar ul li a{
    padding: 5px 20px;
    text-decoration: none;
    color: rgb(255, 255, 255);
}
.navbar ul li a:hover{
    border-bottom: 2px solid yellow;
}
#home{
    display: flex;
    flex-direction: column;
    height: 1000px;
    justify-content: center;
    align-items: center;
    background-color: rgba(0,0,0,0.5);
    color: white;
    font-size: 25px;
}
#home::before{
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    background: url('bg1.jpg') no-repeat center center/cover;
    height: 1100px;
    width: 100%;
    z-index: -1;
    opacity: .7;
}
.heading{
    color: rgb(240, 243, 246);
    font-size: 3rem;
    font-family: Georgia, 'Times New Roman', Times, serif;
    text-align: center;
    transform: scale(1,1.3);
}
#portfolio{
    display: flex;
    flex-direction: column;
    background-color: #A29490;
}
#portfolio h1{
    margin: 60px;


    
}
.gallery{
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
}
.gallery img{
    width: 560px;
    height: 840px;
    padding: 10px;
    margin: 10px;
}
.gallery img:hover{
    background-color: white;
    cursor: pointer;
}

#education{
    display: flex;
    flex-direction: column;
    background-color: #A29490;
}
#education h1{
    margin: 60px;

}
.columns{
    display: grid;
    grid-template-columns: auto auto;
    padding-left: 50px;
}
.box{
    height: 250px;
    width: 600px;
    background-color: rgba(0,0,0,0.5);
    border-radius: 20px;
    margin: 80px;
    padding: 20px;
}
.box:hover {
    transition-duration: 0.1s;
    background-color: #7e645e;
}
.box h2{
    color: rgb(253, 253, 253);
    font-size: 2rem;
    margin-bottom: 40px;
}
.box p{
    color: white;
    font-size: 1.4rem;
}
#about{
    display: flex;
    flex-direction: column;
    height: 1000px;
    background-color:#A29490;
}
#about h1{
    color:white;
    margin: 55px;
}
#about h2{
    color: white;
    font-size: 2.5rem;

    
    padding-right: 200px;
}
#about p{
    color: white;
    font-size: 1.8rem;
}
.about{
    display: flex;
}
.about img{
    width: 600px;
    height: 600px;
    padding: 0px 60px;
}
.name{
    padding: 10px;
}
#contact{
    display: flex;
    flex-direction: column;
    background-color: #A29490;
    height: 800px;
    padding-top: 200px;
    
}
#contact h1{
    margin: 10px;
}
.form{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
.input{
    padding: 15px 20px;
    margin: 15px;
    width: 40%;
    border: none;
    outline: none;
    border-radius: 25px;
    background-color: rgba(0,0,0,0.5);
    color: #A29490;
    font-size: 1.2rem;
}
#message{
    margin: 20px;
    padding: 20px;
    border-radius: 20px;
    background-color: rgba(0,0,0,0.5);
    color: #A29490;
    height: 250px;
    width: 750px;
    font-size: 1.2rem;

}
#submit{
    padding: 15px 20px;
    margin: 30px;
    width: 15%;
    border-radius: 20px;
    background-color: rgba(0,0,0,0.5);
    color: #A29490;
    border: none;
    outline: none;
    font-size: 1.2rem;
}
#submit:hover{
    background-color: rgb(27, 181, 3);
    color: #ffffff;
    cursor: pointer;
}

```


## OUTPUT:

<img width="1262" alt="image" src="https://github.com/Monisha-11/EXP-01---MODERN-WEB/assets/93427240/e7b236ef-8187-4e58-b438-71b5efc2875a">

<img width="1265" alt="image" src="https://github.com/Monisha-11/EXP-01---MODERN-WEB/assets/93427240/71903d6c-2d13-45f8-bfac-e61ad2b21f4e">

<img width="1264" alt="image" src="https://github.com/Monisha-11/EXP-01---MODERN-WEB/assets/93427240/2a918907-fc64-4be8-8dbe-d18ccce3ce3c">

<img width="1262" alt="image" src="https://github.com/Monisha-11/EXP-01---MODERN-WEB/assets/93427240/fb5a68b1-942c-44b2-b984-544930f55d46">


## RESULT:

Thus, a Portfolio is created using HTML and CSS.
