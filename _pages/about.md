---
permalink: /
title: "About"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
scripts:
  - src: "https://cdn.jsdelivr.net/npm/darkmode-js@1.5.7/lib/darkmode-js.min.js"
  - inline: |
      function addDarkmodeWidget() {
        new Darkmode().showWidget();
      }
      window.addEventListener('load', addDarkmodeWidget);
---
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>{{ page.title }}</title>
    <!-- Include the dark mode script tags here -->
    {% if page.scripts %}
        {% for script in page.scripts %}
            <script src="{{ script.src | relative_url }}"></script>
            {% if script.inline %}
                <script>{{ script.inline | strip_newlines }}</script>
            {% endif %}
        {% endfor %}
    {% endif %}
    <!-- Link to favicon -->
    <link rel="icon" type="image/png" href="https://raw.githubusercontent.com/senanindya/senanindya.github.io/main/favicon.ico">
</head>
<body>

Hello!<br />
I am **Anindya Sen**. I have completed B.Tech. in Computer Science and Engineering from <a href="https://vit.ac.in/">Vellore Institute of Technology (VIT),Vellore</a>, Tamil Nadu, India.
My primary research interest lies in Machine Learning Applications, Computer Vision, and Image Processing.<br /><br />
 
I am open to any Research Collaborations in the field of *Large Language Models*, *Medical Imaging* and *Chat bots*. Please reach out if you have anything to discuss or want to work together.<a href="mailto:senanindya5@gmail.com"><i class="fas fa-envelope"></i></a> <br />  

<!---
-----------

# Activities 
* <span style="color:Blue"> [March 3, 2021] </span> - One paper won the [<span style ="color:Red">**3rd Best Paper Award**</span>](https://tonmoy-hossain.github.io/files/ICCIT-Best-Paper.pdf) at [ICCIT 2020](http://iccit.org.bd/2020/).

<script type="text/javascript" src="//rf.revolvermaps.com/0/0/8.js?i=52vxgbx02tg&amp;m=0&amp;c=ff0000&amp;cr1=ffffff&amp;f=arial&amp;l=33" async="async"></script>
-----------
-->


Skills
======
* **Programming Languages/Platforms:** Python, C++, MATLAB, LaTeX, Arduino
* **Machine Learning Libraries/Platforms:** Tensorflow, PyTorch, Keras, OpenCV, Numpy, Scikit-learn, Weka
* **Web Languages/Platforms/Frameworks:** HTML, CSS, Javascript, React, jQuery, Bootstrap, Django, Wordpress, Kajabi, Shopify, Clickfunnels

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

