# Horiseon Refactor

## Description 

This project is a code refactoring of a single web page aimed at making the website's images more accesible and the websites code cleaner and semantic. 

The acceptance requirements were:

>GIVEN a webpage meets accessibility standards  
WHEN I view the source code  
THEN I find semantic HTML elements  
WHEN I view the structure of the HTML elements  
THEN I find that the elements follow a logical structure independent of styling and positioning  
WHEN I view the icon and image elements  
THEN I find accessible alt attributes  
WHEN I view the heading attributes  
THEN they fall in sequential order  
WHEN I view the title element  
THEN I find a concise, descriptive title  

The webpage itself is live and can be [found here](https://corasinth.github.io/horiseon-refactor/). 

If the link above is inaccesible for any reason, a screenshot of the page is below. 
![Screenshot](./assets/images/horiseon_screenshot.png)

Below is a brief summary of the kinds of changes made. Changes were made entirely in HTML and CSS using VSCode and GitHub.  

## Table of Contents

* [Semantic Changes](#semantic-changes)
* [CSS Consolidation](#css-consolidation)
* [Image Accessibility](#image-accessibility)
* [Corrections](#corrections)  
* [Credits](#credits)
* [License](#license)

## Semantic Changes

These changes consisted primarily of replacing `<div>` containers with more appropriate ones, such as `<header>`, `<footer>`, and `<section>`. 

It also involved revising the CSS code so that various rules were still in effect given the changes to container names. Introducing some classes and cutting some out was also effective to maintain the CSS effects. 

Lastly, I cleaned up the code so that it was logically consistent with its new semantic labels, introducing spaces between sections and labeling areas with comments for future accessibility. 

## CSS Consolidation 

The CSS starter code was redundant in several areas, and I consolidated and cleaned up the selectors where I could. 

I also reorganized the CSS flow so that the page loads more evenly and proceeds from the top of the page to the bottom. Comments along general areas of CSS code corresponding to sections of HTML were used for ease of future revisions. 

## Image Accessibility

All images were given alt attributes for screen reader accesibility. With the exception of a single image, the images were purely deocrative and provided no information to describe. Blank alt attributes, as `alt=""` were provided for these so that screenreaders would not read the name of the image file. 

## Corrections

A few corrections to the code were required. 

One of the section links was broken; the section in question was missing the appropriate `id`, which was provided.

Additionally, [this image](./assets/images/digital-marketing-meeting.jpg) was inserted into the webpage using `background-image` in CSS. I removed this image and replaced it using HTML for consistency. This change is of course easily reversible should anyone wish to utilize CSS sprites for the image or have some other reason for removing it from the HTML code.  

## Credits
Jerome Chennette provided the starter code for refactoring. 

[This guide](https://accessible360.com/accessible360-blog/2020-11-10-the-art-of-alt-attributes/) was used to make accesibility decisions.

## [License](./LICENSE)