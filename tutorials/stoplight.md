---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: "test"
permalink: /tutorials/stoplight
---


<html>
<head>

<link rel="shortcut icon" type="image/x-icon" href="/favicon.ico?">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="google-site-verification" content="oDxukBkdlE7rzN-YU0phS7LTeVIG1ZGbeS62fjbs3q8" />

<meta property="og:title" content="Site Title" />
<meta property="og:type" content="website" />
<meta property="og:url" content="http://my.site.com" />
<meta property="og:image" content="https://raw.githubusercontent.com/codeoffun2/codeoffun/gh-pages/favicon.ico" />
<meta property="og:description" content="Site description" />
<meta name="theme-color" content="#FF0000">
<!-- Include this to make the og:image larger -->
<meta name="twitter:card" content="summary_large_image">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<body style="background-color:#FFFFFF;">


<html>
<head>
<style>
body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
}

.topnav {
  overflow: hidden;
  background-color: #333;
}

.topnav a {
  float: left;
  color: #81D8D0;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

.topnav a:hover {
  background-color: #81D8D0;
  color: white;
}

.topnav a.active {
  background-color: #81D8D0;
  color: white;
}
.dropdown {
  float: left;
  overflow: hidden;
}

.dropdown .dropbtn {
  font-size: 16px;  
  border: none;
  outline: none;
  color: white;
  padding: 14px 16px;
  background-color: #333;
  font-family: inherit;
  margin: 0;
}

.navbar a:hover, .dropdown:hover .dropbtn {
  background-color: red;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
  right: 0;
}

.dropdown-content a {
  float: none;
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
  text-align: left;
}

.dropdown-content a:hover {
  background-color: #ddd;
}

.dropdown:hover .dropdown-content {
  display: block;
}
.mobileShow {display: none;} 

  /* Smartphone Portrait and Landscape */ 

}
  #content-desktop {display: block;}
#content-mobile {display: none;}

@media screen and (max-width: 600px) {

#content-desktop {display: none;}
#content-mobile {display: block;}

}
  code {
  font-family: Consolas,"courier new";
  color: crimson;
  background-color: #f1f1f1;
  padding: 2px;
  font-size: 105%;
}
</style>
</head>
<body>

<div class="topnav">
<div id="content-desktop">
  <a href="https://codeoffun.ddns.net">Home</a>
  <a href="https://codeoffun.ddns.net/projects">Projects</a>
  <a class="active" href="https://codeoffun.ddns.net/tutorials">Tutorials</a>
    <a href="https://codeoffun.ddns.net/contact">Contact</a>
  <a href="https://codeoffun.ddns.net/about">About</a>
  <a  href="https://codeoffun.ddns.net/blog">Blog</a>  
  </div>
<div id="content-mobile">
 <div style="float:left" >

     <a  href="https://codeoffun.ddns.net">Codeoffun</a> 
    </div>

 <div style="float:right" >

<div class="dropdown">

    <button class="dropbtn">
      <i class="fa fa-bars"></i>
    </button>
    <div class="dropdown-content">
      <a href="https://codeoffun.ddns.net/projects">Projects</a>
      <a href="https://codeoffun.ddns.net/tutorials">Tutorials</a>
        <a href="https://codeoffun.ddns.net/contact">Contact</a>
      <a href="https://codeoffun.ddns.net/about">About</a>   
        <a href="https://codeoffun.ddns.net/blog">Blog</a>
  </div> 
    </div>
  </div>
</div>
  </div>
  <div>


<!-- end of button code -->

    <p style="font-family: Helvetica"> <p> <h2> How to make an arduino stoplight </h2> </p>
  <p> This tutorial will teach you how to make a stoplight with an arduino.
    <br> This project can be done within 5-10 minutes.
    <br> Level: Beginners </p>
  <p> <h2> Materials: </h2>
    <br> Arduino
    <br> 3 leds (red, green and yellow)
  </p>
  <h2> Code: </h2>
  <br>
  <p> <code> /* Led stoplight<br>
<br>
  Wiring:<br>
  -----------------------------<br>
  |Arduino pin |Leds          |<br>
  |------------|---------------<br>
  |     2      |green led  (+)|<br>
  |     3      |yellow led (+)|<br>
  |     4      |red led    (+)|<br>
  |    gnd     |all 3 leds (-)|<br>
  -----------------------------<br>
*/<br>
int green = 2;<br>
int yellow = 3;<br>
int red = 4;<br>
void setup() {<br>
  // initialize digital pins as an output.<br>
  pinMode(green, OUTPUT);<br>
  pinMode(yellow, OUTPUT);<br>
  pinMode(red, OUTPUT);<br>
}<br>
<br>
// the loop function runs over and over again forever<br>
void loop() {<br>
  digitalWrite(green, HIGH);  //turn on the green led<br>
  delay(5000);                //delays 5 seconds<br>
  digitalWrite(green, LOW);   //turns the led off<br>
  digitalWrite(yellow, HIGH); //turns the yellow led on<br>
  delay(5000);                //delays 5 seconds<br>
  digitalWrite(yellow, LOW);  //turns the led off<br>
  digitalWrite(red, HIGH);    //turns the red led on<br>
  delay(5000);                //delays 5 seconds<br>
  digitalWrite(red, LOW);     //turns the led off<br>
}<br> </code>
  </p>
  <br> Wiring: 
  <br>
  <img src="Screenshot 2022-03-05 171055.png" alt="wiring">
