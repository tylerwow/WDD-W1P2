# Week 1 Practical 2 - Structuring Content with HTML

This practical is all about getting you to start writing your own HTML from scratch, while thinking carefully about the structure of your site and use of semantic elements. You will build a basic portfolio site over the next few practicals. Today you will focus on planning the structure of your site and writing the basic HTML.
The work for this practical has been broken down into 2 stages. 

## Stage 1: Planning and describing content with semantic HTML
Your task is to (eventually) build a basic portfolio website for yourself from scratch. If you already have a portfolio, scroll down to the sub-section titled, “I already have a portfolio site…”. 

The exact contents of your portfolio are up to you, but you should aim for the following pages and sections:
- **Home (or About)**. The Home / About page should include a paragraph or two about yourself and maybe an image.
- **Projects**. The Projects page will describe some of the projects you have worked. Include images and the skills you have learned. Consider adding additional detail pages if you want to describe your work in more detail.
- **CV**. Include sections for education, work / volunteer experience, and skills.

Creating a high quality portfolio website can take a long time so, for this session, focus on how you will structure the information on each page of your site and don’t worry too much about the content itself, or design details like the colour palette (we’ll get into styling next week).

Focusing on one page at a time, plan the semantic HTML structure of your portfolio. To make sure you actually write some HTML today, **spend no more than the first half hour of practical on this stage**. You are not being marked, you do not have to make the site public unless you want to, and you can always come back and make changes in future so don’t get bogged down in the details! 

You will probably find it helpful to look at some [example developer portfolio sites](https://github.com/emmabostian/developer-portfolios) for inspiration. 

Some tips:
- At a minimum, you should plan for a `<header>`, which will contain your site title and a `<nav>` with links to each page on your site, and a `<main>` area that will contain the main contents of each page. The `<header>` section may be the same on each page.
- Some pages may benefit from `<section>` and/or `<article>` areas.
- All text should be in the appropriate semantic text tags (i.e. `<h1> … <h6>, <p>, <a>`).
- A `<footer>` section can be a good place to put things like the last update date, contact information, or links to social media.

If you are not sure what the elements mentioned above are for and how they should be used check the W3Schools Reference list of Elements and revise the lecture on structuring content with HTML.

**_I already have a portfolio site…_**
Did you write your portfolio site yourself from scratch using HTML (i.e. without using blog services or site builders like Wordpress or Wix.com)? 
- If the answer is yes, look carefully at your HTML code and make sure you have used proper semantic HTML everywhere you can. If you are unsure, show your code to the course staff.
- If the answer is no, take this opportunity to try to replicate your existing portfolio site using semantic HTML.
- Alternatively, plan a professional website for your favourite fictional character.

## Stage 2: Writing semantic HTML
After completing stage 1, you should have an outline of your portfolio marked up using HTML elements.

Next, create a folder for your website and open it in Visual Studio Code. From inside VS Code, create HTML files for each page of your site. Follow these guidelines:
- The entry point of your site (your home page) must be a file named **index.html**. When a user types in the URL of a website without a specific file name, the browser looks for a file name index.html. Naming your entry point index.html ensures your site will be found.
- You may name the other files of your site whatever you like but filenames should not contain spaces or special characters other than _ or –
- Use the boilerplate code provided in Lecture 2 (see the code below) for every HTML file. Make sure you update the `<title>` tag of each page! Reminder: don’t copy-paste code directly from the slides as you will likely encounter bugs due to character encoding.

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8"/>
    <title>CHANGE ME!!!</title>
  </head>
  <body>
  </body>
</html>
```

Begin filling in each page with the semantic HTML you planned in stage 1. Don’t worry about putting “real” text content and images in the pages just yet (unless you’re ready). You can use [lorem ipsum as filler text](https://www.lipsum.com/feed/html) and you can download placeholder images from [pixabay](https://pixabay.com/) or [pexels](https://www.pexels.com/). 

Aim to get at least one page mocked up in HTML by the end of practical. If you have more than one page ready, make sure there’s a way to navigate between them. A widely used convention for creating a menu on a website is to use an unordered list. By default, unordered lists appear as a list of bullet points, which probably isn’t how you want your navigation to look. We will use CSS to style the list appropriately next week. For now, the code for your site navigation should look something like this:
```
<nav>
    <ul>
        <li><a href=”index.html”>Home</a></li>
        <li><a href=”yourProjectsPage.html”>Projects</a></li>
        <li><a href=”yourCV.html”>CV</a></li>
    </ul>
</nav>
```
Take a close look at the href attributes in the links above. Assuming all of your pages are in the same folder, the value of the attribute should be just the name of the file you want to link to; there is no need to add a full path. These are _**relative**_ file paths, meaning you provide the file location relative to the current file. For more detail on relative paths, see the section titled, “A quick primer on URLs and file paths”, in the [MDN tutorial on creating hyperlinks](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks). 

Finally, make sure your work is valid by using the W3C validation extension installed last time **and** putting the code through [the W3C Validator](https://validator.w3.org/).

Make sure you push and commit this code on GitHub, as we will be using it in future practicals.
