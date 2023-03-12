<body>
    <table border="1">
        <tr>
            <th> Nama</th>
            <th>NIM</th>
            <th>Kelas</th>
        </tr>
        <tr>
            <td>Ahmad Syukron</td>
            <td>312110056</td>
            <td>TI.21.A.1</td>
        </tr>
    </table>
</body>

# Layout Sederhana

## Tugas Latihan
- <b>Soal</b><p>
![Gambar 00](Image/Tugas.png)<p>

- <b>index.html</b><p>
```bash
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>

    <!-- CSS -->
    <link rel="stylesheet" href="style.css" />
</head>
<body>
    <div id="container">
        <header>
            <h1>Layout Sederhana</h1>
        </header>
        <nav>
            <ul>
              <a href="index.html" class="active">Home</a>
              <a href="#article">Artikel</a>
              <a href="about">About</a>
              <a href="contact">Kontak</a>
            </ul>
          </nav>
      <section id="hero">
        <h1>Hello World!</h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum
          lorem elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin
          in leo fringilla, vestibulum mi porta, faucibus felis. Integer
          pharetra est nunc, nec pretium nunc pretium ac.
        </p>
        <a href="#"
          ><button class="button" style="vertical-align: middle">
            <span>Learn more </span>
          </button></a
        >
      </section>
      <section id="wrapper">
        <section id="main">
          <div class="row">
            <div class="box">
              <img
                src="https://dummyimage.com/120/db7d25/fff.png"
                alt=""
                class="image-circle"
              />
              <h3>Heading</h3>
              <p>
                Donec sed odio dui. Etiam porta sem malesuada magna mollis
                euismod.
              </p>
              <a href="#"
                ><button type="button" class="button-img">
                  View detail
                </button></a
              >
            </div>
            <div class="box">
              <img
                src="https://dummyimage.com/120/3e73e6/fff.png"
                alt=""
                class="image-circle"
              />
              <h3>Heading</h3>
              <p>
                Donec sed odio dui. Etiam porta sem malesuada magna mollis
                euismod.
              </p>
              <a href="#"
                ><button type="button" class="button-img">
                  View detail
                </button></a
              >
            </div>
            <div class="box">
              <img
                src="https://dummyimage.com/120/71e6d4/fff.png"
                alt=""
                class="image-circle"
              />
              <h3>Heading</h3>
              <p>
                Donec sed odio dui. Etiam porta sem malesuada magna mollis
                euismod.
              </p>
              <a href="#"
                ><button type="button" class="button-img">
                  View detail
                </button></a
              >
            </div>
          </div>

          <hr class="divider" />
          <article id="article" class="entry">
            <h2>First featurette heading.</h2>
            <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" />
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Vestibulum lorem elit, iaculis in nisl volutpat, malesuada
              tincidunt arcu. Proin in leo fringilla, vestibulum mi porta,
              faucibus felis. Integer pharetra est nunc, nec pretium nunc
              pretium ac.
            </p>
          </article>
          <hr class="divider" />
          <article class="entry">
            <h2>First featurette heading.</h2>
            <img
              src="https://dummyimage.com/150/7b8a70/fff.png"
              alt=""
              class="right-img"
            />
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Vestibulum lorem elit, iaculis in nisl volutpat, malesuada
              tincidunt arcu. Proin in leo fringilla, vestibulum mi porta,
              faucibus felis. Integer pharetra est nunc, nec pretium nunc
              pretium ac.
            </p>
          </article>
        </section>
        <aside id="sidebar">
          <div class="widget-box">
            <h3 class="title">Widget Header</h3>
            <ul>
              <li><a href="#">Widget Link</a></li>
              <li><a href="#">Widget Link</a></li>
              <li><a href="#">Widget Link</a></li>
              <li><a href="#">Widget Link</a></li>
              <li><a href="#">Widget Link</a></li>
            </ul>
          </div>
          <div class="widget-box">
            <h3 class="title">Widget Text</h3>
            <p>
              Vestibulum lorem elit, iaculis in nisl volutpat, malesuada
              tincidunt arcu. Proin in leo fringilla, vestibulum mi porta,
              faucibus felis. Integer pharetra est nunc, nec pretium nunc
              pretium ac.
            </p>
          </div>
        </aside>
      </section>
      <footer>
        <p>&copy; 2023 - Universitas Pelita Bangsa</p>
      </footer>
    </div>
  </body>
</html>
```


## Style

- <b>Style.css</b><p>

```bash
/* Import google font */
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');

@import url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');

/* Reset CSS */
* {
    margin: 0;
    padding: 0;
}

body {
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#5a5a5a;
}

#container {
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}

/* Header */
header {
    padding: 20px;  
}

header h1 {
    margin: 20px 10px;
    color: #b5b5b5;
}

/* Navigasi */
nav {
    display: block;
    background-color: #1f5faa;
}

nav a {
    padding: 15px 30px;
    display: inline-block;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
    font-weight: bold;
}

nav a.active,
nav a:hover {
    background-color: #2b83ea;
}

/* Hero Panel */
#hero {
    background-color: #e4e4e5;
    padding: 50px 20px;
    margin-bottom: 20px;
}
#hero h1 {
    margin-bottom: 20px;
    font-size: 35px;
    color: #0a0a0a;
}
#hero p {
    margin-bottom: 20px;
    font-size: 18px;
    line-height: 25px;
}

/* Main Content */
#wrapper {
    margin: 0;
}

#main {
    float: left;
    width: 640px;
    padding: 20px;
}

/* Sidebar Area */
#sidebar {
    float: left;
    width: 260px;
    padding: 20px;
}

/* Widget */
.widget-box {
    border:1px solid #eee;
    margin-bottom:20px;
}

.widget-box .title {
    padding:10px 16px;
    background-color:#428bca;
    color:#fff;
}

.widget-box ul {
    list-style-type:none;
}

.widget-box li {
    border-bottom:1px solid #eee;
}

.widget-box li a {
    padding:10px 16px;
    color:#333;
    display:block;
    text-decoration:none;
}

.widget-box li:hover a {
    background-color:#eee;
}

.widget-box p {
    padding:15px;
    line-height:25px;
}

/* Box */
.box {
    display:block;
    float:left;
    width:33.333333%;
    box-sizing:border-box;
    -moz-box-sizing:border-box;
    -webkit-box-sizing:border-box;
    padding:0 10px;
    text-align:center;
}

.box h3 {
    margin: 15px 0;
}

.box p {
    line-height: 20px;
    font-size: 14px;
    margin-bottom: 15px;
}

.box img {
    border: 0;
    vertical-align: middle;
}

.image-circle {
    border-radius: 50%;
}

.row {
    margin: 0 -10px;
    box-sizing: border-box;
    -moz-box-sizing: border-box;
    -webkit-box-sizing: border-box;
}

.row:after, .row:before,
.entry:after, .entry:before {
    content:'';
    display:table;
}

.row:after,
.entry:after {
    clear:both;
}

/* Article */
.divider {
    border:0;
    border-top:1px solid #eeeeee;
    margin:40px 0;
}

/* entry */
.entry {
    margin: 15px 0;
}

.entry h2 {
    margin-bottom: 20px;
}

.entry p {
    line-height: 25px;
}

.entry img {
    float: left;
    border-radius: 5px;
    margin-right: 15px;
}

.entry .right-img {
    float: right;
}

/* Footer */
footer {
  clear:both;
  background-color:#1d1d1d;
  padding:20px;
  color:#eee;
}

/* Button */

.button {
  display: inline-block;
  border-radius: 4px;
  background-color: #317CFF;
  border: none;
  color: #FFFFFF;
  text-align: center;
  font-size: 16px;
  padding: 10px;
  width: 140px;
  transition: all 0.5s;
  cursor: pointer;
  margin: 5px;
}

.button span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}

.button-img {
  padding: 5px;
}

.button span:after {
  content: '\00bb';
  position: absolute;
  opacity: 0;
  top: 0;
  right: -20px;
  transition: 0.5s;
}

.button:hover span {
  padding-right: 25px;
}

.button:hover span:after {
  opacity: 1;
  right: 0;
}

```

# END
![Gambar 04](Image/anime-love.gif)