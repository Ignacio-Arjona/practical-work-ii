# Design Detailed Document

### Description of my work

This project consists of the development of a software, a  website. The website is composed of seven main pages, each one with its own quirks and characteristics:
1) index.html: This page serves as a hub to all the other pages, and it includes a link to every one of them, as well as a brief description.

2) topic.html: This page is dedicated to a personal topic, the critique of social injustice and oppresion shown in One Piece, and its relation to real-life events. Although it is a very specific topic, it should be comprehensible without having any previous knowledge on the series, as almost all relevant names or events are either self-descriptive ("World Government") or explained briefly ("Five Elders (the head of the World Government)").

3) degree.html: In this page I delve deeped into the degree I'm studying on the UFV. It includes a general section for some information related to the degree (Overview, Purpose and Structure), as well as a section for each of the five degree years, each one featuring it's own subjects. It also features a link to fce.html, allowing visitors to easily nagivate between pages.

4) fce.html: This page is focused on the subject of "Fundamentals of Computer Engineering". It is divided into three main sections; Content (related to the structure and the content covered in the program), Objectives (self-descriptive) and Learning Outcomes (self-descriptive). 
5) net.html: This page serves as a hub to the index.html of my partners, allowing the visitors to easily navigate through our websites.

6) about.html: In this page I give some extra information about myself. It includes a "Description" section, where I delve into my career and personal interests, adding some photos featuring myself. It also includes my curriculum vitae, where I showcase my profesional experience, certifications, skills, and much more. Lastly, it includes a section with links to some social media profiles, such as Instagram, X, Threads, Facebook and Twich.

7) contact.html: This page consists purely on a contact form. It is designed without any scripting elements that send the information, and it has the basic input boxes for a typical contact form (Name, Email, Phone Number, Message...) 

### Problems during the development

This project was filled to the brim with problems: 
1) To start off, I had from the start a clear idea in my mind, to include an expandable menu in the left of the screen. I could've used the "hover" pseudo-class to give an easy solution to this, but I wanted to make it switch between two different stages, and stay in the current stage until something was triggered again, not until the hovering was over. The first problem actually was finding a way to do this kind of menu. Because of this, I researched about buttons and the "checked" pseudo-class, which solved my issue. This feature was also used in future pages such as degree.html for the expandable elements.

2) In second place, another issue I had recursively during the development process was the measures and its units. I wanted to make a webpage that worked properly in most devices. Because of this, I adopted through all the webpages relative units. These are vh and vw, where 100vh is the total height of any device the website is being visited on, and 100vw is the width of the device. Of course, this didn't solve anything, because some elements, such as square-shaped photos required to be modified in both the height and width simultaneously. Using the min() function solved this issue. 

3) The third main problem I found during the development of the webpage was the left side menu height. During the first pages I designed (index.html and contact.html) the content wasn't enough to surpass the document height. Because of this, I was surprised to see that for the next page (degree.html), where the information actually overfloaded the website, the side menu actually was cut out at 100vh (the height of the device). In order to solve this, I created a button for each of the page where this issue happened, and configured it so that, when the button wasn't checked, the height of the side menu is the size I wanted. As the button wasn't able to be checked by anything (due to display:none), the page was constantly on the perfect sizing.

4) The fourth problem is closely related to the third. When I chose a height for the side menu, it worked just fine until I tried to resize the screen proportions. I haven't been able to find a solution for this, but I've found a semi-solution and implemented it. Thanks to this solution, the height of the side menu will be **At Least** the content height. This causes some extra space to be left on the bottom of the page but, besides aesthetics, there isn't any problem with that.

5) The fifth and last mayor problem I found during this development was that, when the content surpassed the document height (waht happened in errors 3 and 4), a scroll bar was added to the document for the visitor to scroll down in order to see all the contents. As a scroll bar is created on the right border, and all measures were made so that the total width of the webpage was 100% of the device width, the content overflowed in the width. Because of this, another scroll bar was created in the bottom in order to see al the contents. This was not only visually unappealing, but caused some errors with the interactions between divs. I solved this issue by completely removing sidebars in all the pages.

### Conclusions

