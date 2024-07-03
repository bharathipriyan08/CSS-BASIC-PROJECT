# CSS-BASIC-PROJECT
# Program:
```
 Index Code:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BP Coaching Centre</Center></title>
    <style type="text/css">
        * {
            margin: 0;
            padding: 0;
            font-family: Arial, Helvetica, sans-serif;
        }
        .banner {
            width: 100%;
            height: 95vh;
            background-image: linear-gradient(
                rgba(0, 0, 0, 0.75),
                rgba(0, 0, 0, 0.75)
            ),
            url('/static/background.jpg');
            background-size: cover;
            background-position: center;
            color: #fff; 
        }
        .navbar {
            width: 85%;
            margin: auto;
            padding: 35px 0;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }
        .logo {
            color: #fb0b1b;
            font-size: 40px;
            font-weight: 700;
            letter-spacing: 3px;
        }
        span {
            color: white;
        }
        form {
            width: 300px;
            height: 40px;
            display: flex;
            background: rgba(255, 255, 255, 0.2);
            padding: 1px 1px;
            font-size: 15px;
            border-radius: 10px;
            backdrop-filter: blur(4px) saturate(180%);
        }
        form input {
            background: transparent;
            flex: 1;
            border: 0;
            outline: none;
            padding: 12px 20px;
            font-size: 15px;
            color: white;
        }
        ::placeholder {
            color: white;
        }
        form button {
            border: 0;
            outline: none;
            padding: 5px 20px;
            color: white;
            border-radius: 10px;
            background: rgb(255, 133, 92);
            cursor: pointer;
        }
        #search.hover {
            border: 1px;
            padding: 10px;

            transition: 0.5s;
            cursor: pointer;
            border-radius: 30px;
            background:rgb(255, 133, 92);
            color: #081b29;
            box-shadow: 0 0 20px rgb(231, 160, 128);
        }
        .navbar li {
            list-style: none;
            display: inline-block;
            margin: 0 20px;
            position: relative;
        }
        .navbar li a {
            text-decoration: none;
            color: white;
            text-transform: uppercase;
        }
        .navbar li:hover {
            border: 1px;
            padding: 10px;

            transition: 0.5s;
            cursor: pointer;
            border-radius: 30px;
            background: rgb(255, 133, 92);
            color: #081b29;
            box-shadow: 0 0 20px rgb(252, 129, 129);
        }
        .content {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
        }
        .text h2 {
            color: #fb0be3;
            font-weight: 800;
            font-size: 40px; 
            letter-spacing: 3px;
        }
        .text p {
            color: white;
            text-transform: capitalize;
            font-size: 15px;
            margin-bottom: 30px;
            word-spacing: 2px;
            letter-spacing: 1px;
        }
        .login {
            margin: 0px 10px;
            border: 2px solid #161717;
            padding: 13px 35px;
            letter-spacing: 1px;
            color: white;
            border-radius: 30px;
            background-color: #0f1010;
            text-decoration: none;
        }
        .login:hover {
            border: 2px solid #151515;
            color: #191a1a;
            background-color: white;
            transition: 0.5s;
            cursor: pointer;
        }
        .signup {
            margin: 0px 10px;
            border: 2px solid #0e0e0e;
            padding: 13px 35px;
            letter-spacing: 1px;
            color: white;
            border-radius: 30px;
            background-color: #1b1c1d;
            text-decoration: none;
        }
        .signup:hover {
            border: 2px solid #f60b0b;
            color: #1b1c1c;
            background-color: white;
            transition: 0.5s;
            cursor: pointer;
        }
        footer {
            border: 1px;
            padding: 10px;

            transition: 0.5s;
            cursor: pointer;
            border-radius: 30px;
            background: rgb(255, 133, 92);
            color: #081b29;
            box-shadow: 0 0 20px rgb(17, 17, 17);
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
<div class="banner">
    <br />
    <div class="navbar">
        <h1 class="logo">BP<span>C</span>oaching<span>Centre</span></h1>
        <ul>
            <li><a href="{% url 'home' %}">Home</a></li>
          <li><a href="{% url 'products' %}">Products</a></li>
          <li><a href="{% url 'people' %}">People</a></li>
          <li><a href="{% url 'contact' %}"> Contact </a></li>
        </ul>
        <form action="" method="get">
            <input type="text" placeholder="Enter to Search" />
            <button id="search" type="submit">Search</button>
        </form>
    </div>
    <div class="content">
        <div class="text">
            <h2>
                Keep going. Everything you need will come to you at the perfect time.
            </h2>
            <br />

            <br />
            <div>
                <a href="#" class="login"> Log In </a>
                <a href="#" class="signup"> Sign Up </a>
            </div>
        </div>
    </div>
</div>
<footer>
    <center>Created by BHARATHI PRIYAN T</center>
</footer>
</body>
</html>

Product code:
    <html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Product Page</title>
    <style type="text/css">
      * {
        margin: 0;
        padding: 0;
        font-family: Arial, Helvetica, sans-serif;
      }
      .banner {
        width: 100%;
        height: 95vh;
        background-image: linear-gradient(
            rgba(0, 0, 0, 0.75),
            rgba(0, 0, 0, 0.75)
          ),
          url('/static/background.jpg');
        background-size: cover;
        background-position: center;
      }
      .navbar {
        width: 85%;
        margin: auto;
        padding: 35px 0;
        display: flex;
        align-items: center;
        justify-content: space-between;
      }
      .bg-product {
        border: 1px;
        padding: 10px;
        color: white;
        background-color: rgb(255, 133, 92);
        border-radius: 30px;
      }
      .logo {
        color: #3b0bfb;
        font-size: 40px;
        font-weight: 700;
        letter-spacing: 3px;
      }
      span {
        color: white;
      }
      form {
        width: 300px;
        height: 40px;
        display: flex;
        background: rgba(255, 255, 255, 0.2);
        padding: 1px 1px;
        font-size: 15px;
        border-radius: 10px;
        backdrop-filter: blur(4px) saturate(180%);
      }
      form input {
        background: transparent;
        flex: 1;
        border: 0;
        outline: none;
        padding: 12px 20px;
        font-size: 15px;
        color: white;
      }
      ::placeholder {
        color: white;
      }
      form button {
        border: 0;
        outline: none;
        padding: 5px 20px;
        color: white;
        border-radius: 10px;
        background: rgb(255, 133, 92);
        cursor: pointer;
      }
      .navbar li {
        list-style: none;
        display: inline-block;
        margin: 0 20px;
        position: relative;
      }
      .navbar li a {
        text-decoration: none;
        color: white;
        text-transform: uppercase;
      }
      .navbar li:hover {
        border: 1px;
        padding: 10px;

        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgb(255, 133, 92);
        color: #081b29;
        box-shadow: 0 0 20px rgb(255, 133, 92);
      }
      .container {
        background: transparent;
        padding: 10px 5%;
        padding-bottom: 100px;
      }
      .container .box-container {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(170px, 1fr));
        gap: 100px;
      }
      .container .box-container .box {
        color: white;
        box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
        border-radius: 20px;
        background: transparent;
        border: 1px solid white;
        padding: 30px 20px;
      }
      .container .box-container .box img {
        height: 70px;
        border-radius: 20px;
      }
      .container .box-container .box h3 {
        color: rgb(255, 133, 92);
        font-size: large;
        padding: 20px 0;
      }
      .container .box-container .box p {
        color: white;
        font-size: small;
        line-height: 1.5;
      }
      footer {
        border: 1px;
        padding: 10px;

        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgb(255, 133, 92);
        color: #081b29;
        box-shadow: 0 0 20px rgb(34, 36, 36);
      }
    </style>
  </head>
  <body>
    <div class="banner">
      <br />
      <div class="navbar">
        <h1 class="logo">BP<span>C</span>oaching<span>Centre</span></h1>
        <ul>
          <li><a href="{% url 'home' %}">Home</a></li>
          <li><a href="{% url 'products' %}"  class="bg-product">Products</a></li>
          <li><a href="{% url 'people' %}">People</a></li>
          <li><a href="{% url 'contact' %}"> Contact </a></li>
        </ul>
        <form action="" method="get">
          <input type="text" placeholder="Enter to Search" />
          <button type="submit">Search</button>
        </form>
      </div>
      <div class="container">
        <div class="box-container">
          <div class="box">
            <h3>Programming Languages</h3>
            <p>
              Front end and back end programming languages such as Java, Python, PHP, CSS, JavaScript. </p>
          </div>
          <div class="box">
            <h3>GATE,CAT Preparation</h3>
            <p>
              Coaching to face competitive exams like GATE,CAT,NEET.</p>
          </div>
          <div class="box">
            <h3>Engineering Mathematics</h3>
            <p>
              Engineering Mathematics subjects such as discrete mathematics,graphs,combinatorics.
            </p>
          </div>
          <div class="box">
            <h3>Computational Algorithms and Data Structures</h3>
            <p>
               Basic algorithms used for computation such as dynamic programming,time and space complexity.           </p>
          </div>
          <div class="box">
            <h3>Aerospace Engineering</h3>
            <p>
              Aerospace engineering is the primary field of engineering concerned with the development of aircraft and spacecraft.            </p>
          </div>
          <div class="box">
            <h3>Biomedical Engineering</h3>
            <p>
              Biomedical engineering (BME) focuses on the advances that improve human health and health care at all levels and is the application of the principles and problem-solving techniques of engineering to biology and medicine.            </p>
          </div>
          <div class="box">
            <h3>Chemical Engineering</h3>
            <p>
              Chemical engineering is a multi-disciplinary branch of engineering that combines natural and experimental sciences  along with life sciences to design, develop, produce, transform, transport, operate and manage the industrial processes that turn raw materials into valuable products.            </p>
          </div>
          <div class="box">
            <h3>Biotechnology</h3>
            <p>
              Biotechnology is technology that utilizes biological systems, living organisms or parts of this to develop or create different products.            </p>
          </div>
          <div class="box">
            <h3>Electronics and Communication Engineering</h3>
            <p>
              Electronics and Communications Engineering (ECE) course is a branch of engineering that covers the study, design, development, and application of electrical circuits, electronics, and communication systems.            </p>
          </div>
          <div class="box">
            <h3>Electrical Engineering</h3>
            <p>
              Electrical engineering is an engineering discipline concerned with the study, design, and application of equipment, devices, and systems which use electricity, electronics, and electromagnetism.            </p>
          </div>
        </div>
      </div>
    </div>
    <footer>
      <center>Created by BHARATHI PRIYAN T</center>
    </footer>
  </body>
</html>


People Code:
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>people page</title>
    <style type="text/css">
      * {
        margin: 0;
        padding: 0;
        font-family: Arial, Helvetica, sans-serif;
      }
      .banner {
        width: 100%;
        height: 95vh;
        background-image: linear-gradient(
            rgba(0, 0, 0, 0.75),
            rgba(0, 0, 0, 0.75)
          ),
          url('/static/background.jpg');
        background-size: cover;
        background-position: center;
      }
      .navbar {
        width: 85%;
        margin: auto;
        padding: 35px 0;
        display: flex;
        align-items: center;
        justify-content: space-between;
      }
      .bg-people {
        border: 1px;
        padding: 10px;
        color: white;
        background-color: rgb(255, 133, 92);
        border-radius: 30px;
      }
      .logo {
        color: #0b13fb;
        font-size: 40px;
        font-weight: 700;
        letter-spacing: 3px;
      }
      span {
        color: white;
      }
      form {
        width: 300px;
        height: 40px;
        display: flex;
        background: rgba(255, 255, 255, 0.2);
        padding: 1px 1px;
        font-size: 15px;
        border-radius: 10px;
        backdrop-filter: blur(4px) saturate(180%);
      }
      form input {
        background: transparent;
        flex: 1;
        border: 0;
        outline: none;
        padding: 12px 20px;
        font-size: 15px;
        color: white;
      }
      ::placeholder {
        color: white;
      }
      form button {
        border: 0;
        outline: none;
        padding: 5px 20px;
        color: white;
        border-radius: 10px;
        background: rgb(255, 133, 92);
        cursor: pointer;
      }
      .navbar li {
        list-style: none;
        display: inline-block;
        margin: 0 20px;
        position: relative;
      }
      .navbar li a {
        text-decoration: none;
        color: white;
        text-transform: uppercase;
      }
      .navbar li:hover {
        border: 1px;
        padding: 10px;

        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgb(255, 133, 92);
        color: #081b29;
        box-shadow: 0 0 20px #0ef;
      }
      .image {
        position: relative;
        border: 0;
        top: 150px;

        background: transparent;
      }
      .image table {
        border: 0;
        color: white;
        position: relative;
        left: 200px;
      }
      .image table img {
        height: 140px;
        width: 140px;
        border: 2px solid white;
        padding: 5px;
        border-radius: 50%;
      }
      .image table td {
        color: #111111;
      }
      footer {
        border: 1px;
        padding: 10px;

        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgb(255, 133, 92);
        color: #081b29;
        box-shadow: 0 0 20px rgb(230, 134, 99);
      }
    </style>
  </head>
  <body>
    <div class="banner">
      <br />
      <div class="navbar">
        <h1 class="logo">BP<span>C</span>oaching<span>Centre</span></h1>
        <ul>
          <li><a href="{% url 'home' %}">Home</a></li>
          <li><a href="{% url 'products' %}">Products</a></li>
          <li><a href="{% url 'people' %}"  class="bg-people">People</a></li>
          <li><a href="{% url 'contact' %}"> Contact </a></li>
        </ul>
        <form action="" method="get">
          <input type="text" placeholder="Enter to Search" />
          <button type="submit">Search</button>
        </form>
      </div>
      <div class="image">
        <table cellspacing="20">
          <tr align="center">
            <td><img src="https://www.pinclipart.com/picdir/middle/11-110067_emoji-faces-free-printables-paper-trail-design-emojis.png" /></td>
            <td><img src="https://cdn.dribbble.com/users/2454973/screenshots/7139551/media/d7ec746931c88d5f957a348245e013f9.jpg" /></td>
            <td><img src="https://www.kindpng.com/picc/m/115-1151460_transparent-smile-emoji-png-big-smiley-face-png.png" /></td>
            <td><img src="https://img.elo7.com.br/product/zoom/D55ED5/emoji-20x20cm-emoji.jpg" /></td>
            <td><img src="https://content.assets.pressassociation.io/2021/02/16174655/65db9fea-5ad3-4d1c-95da-5219f213b70c.png" /></td>
            <td><img src="http://www.pngmart.com/files/8/Crying-Emoji-PNG-Image-Free-Download.png" /></td>
          </tr>
          <tr align="center">
            <th>Bharathi priyan  T</th>
            <th>Prakash</th>
            <th>Vijay</th>
            <th>Akash</th>
            <th>Srivarshan</th>
            <th>kumar</th>
          </tr>
          <tr align="center">
            <td>Director</td>
            <td>Managing Director</td>
            <td>Coaching Head</td>
            <td>Admistrator</td>
            <td>Teaching Department Head</td>
            <td>Campus Head</td>
          </tr>
        </table>
      </div>
    </div>
    <footer>
      <center>Created by BHARATHI PRIYAN T</center>
    </footer>
  </body>
</html>


Contact code:
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Contact Us Page</title>
    <style type="text/css">
      * {
        margin: 0;
        padding: 0;
        font-family: Arial, Helvetica, sans-serif;
      }
      .banner {
        width: 100%;
        height: 95vh;
        background-image: linear-gradient(
            rgba(0, 0, 0, 0.75),
            rgba(0, 0, 0, 0.75)
          ),
          url('/static/background.jpg');
        background-size: cover;
        background-position: center;
      }
      .navbar {
        width: 85%;
        margin: auto;
        padding: 35px 0;
        display: flex;
        align-items: center;
        justify-content: space-between;
      }
      .bg-contact {
        border: 1px;
        padding: 10px;
        color: white;
        background-color: rgb(255, 133, 92);
        border-radius: 30px;
      }
      .logo {
        color: #3b0bfb;
        font-size: 40px;
        font-weight: 700;
        letter-spacing: 3px;
      }
      span {
        color: white;
      }
      .navbar form {
        width: 300px;
        height: 40px;
        display: flex;
        background: rgba(255, 255, 255, 0.2);
        padding: 1px 1px;
        font-size: 15px;
        border-radius: 10px;
        backdrop-filter: blur(4px) saturate(180%);
      }
      .navbar form input {
        background: transparent;
        flex: 1;
        border: 0;
        outline: none;
        padding: 12px 20px;
        font-size: 15px;
        color: white;
      }
      ::placeholder {
        color: white;
      }
      .navbar form button {
        border: 0;
        outline: none;
        padding: 5px 20px;
        color: white;
        border-radius: 10px;
        background: rgb(255, 133, 92);;
        cursor: pointer;
      }
      .navbar li {
        list-style: none;
        display: inline-block;
        margin: 0 20px;
        position: relative;
      }
      .navbar li a {
        text-decoration: none;
        color: white;
        text-transform: uppercase;
      }
      .navbar li:hover {
        border: 1px;
        padding: 10px;

        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgb(255, 133, 92);
        color: #081b29;
        box-shadow: 0 0 20px #0ef;
      }
      .box {
        display: flex;
        column-gap: 40px;
        background: transparent;
        position: relative;
        top: 50px;
      }
      .box-1 {
        height: 400px;
        width: 400px;
        border: 3px solid white;
        border-radius: 20px;
        background: transparent;
        position: relative;
        left: 250px;
      }
      .box-2 {
        height: 400px;
        width: 400px;
        border: 3px solid #ee1f1f;
        border-radius: 20px;
        background: transparent;
        position: relative;
        left: 300px;
      }
      .box-1 form {
        display: flex;
        color: white;
        background: transparent;
        padding: 10px;
        font-size: 15px;
        position: relative;
        top: 15px;
      }
      .box-1 form input {
        background: transparent;
        display: flex;
        border: 1px solid white;
        border-radius: 10px;
        padding: 15px 30px;
        font-size: 15px;
        color: white;
        position: relative;
        top: 30px;
      }
      .box-1 form textarea {
        background: transparent;
        color: white;
        padding: 15px 10px;
        position: relative;
        top: 30px;
        left: 20px;
        border: 1px solid white;
        border-radius: 10px;
        width: 300px;
      }
      .box-1 form button {
        border: 0;
        outline: none;
        padding: 10px 20px;
        color: white;
        border-radius: 30px;
        background:rgb(255, 133, 92);
        cursor: pointer;
        position: relative;
        top: 50px;
      }
      .box-2 h2 {
        color: white;
        position: relative;
        top: 25px;
        left: 50px;
        font-size: 30px;
      }
      .box-2 p {
        color: white;
        position: relative;
        top: 50px;
        padding: 10px 80px;
      }
      .box-2 span {
        color: rgb(255, 133, 92);
        font-size: 20px;
      }
      footer {
        border: 1px;
        padding: 10px;

        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgb(255, 133, 92);
        color: #081b29;
        box-shadow: 0 0 20px rgb(217, 34, 43);
      }
    </style>
  </head>
  <body>
    <div class="banner">
      <br />
      <div class="navbar">
        <h1 class="logo">BP<span>C</span>oaching<span>Center</span></h1>
        <ul>
          <li><a href="{% url 'home' %}">Home</a></li>
          <li><a href="{% url 'products' %}">Products</a></li>
          <li><a href="{% url 'people' %}">People</a></li>
          <li><a href="{% url 'contact' %}" class="bg-contact"> Contact </a></li>
        </ul>
        <form action="" method="get">
          <input type="text" placeholder="Enter to Search" />
          <button type="submit">Search</button>
        </form>
      </div>
      <div class="box">
        <div class="box-1">
          <form>
            <center>
              <h1>Contact Us</h1>
              <input type="text" placeholder="Your Name" />
              <br />
              <input type="email" placeholder="Your Email" />
              <br />
              <textarea rows="4" cols="40" placeholder="Your Message">
              </textarea>
              <br />
              <button type="submit">Submit</button>
            </center>
          </form>
        </div>
        <div class="box-2">
          <h2>Contact Information</h2>
          <p>
            <span>Address</span> : No 8,Top building,East Cost Road,Chennai, India
          </p>
          <p><span>Email</span> : bpcoachingcentre@gmail.com</p>
          <p><span>Follow us On Facebook</span> : https://www.facebook.com/bp_coachingcentre</p>
        </div>
      </div>
    </div>
    <footer>
      <center>Created by BHARATHI PRIYAN T</center>
    </footer>
  </body>
</html>

```
# OUTPUT

