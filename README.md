# User Experience (UX)

## User Stories

As a new user, who may never have heard of the band

1. Know the purpose of the site
2. To be able to learn about the members/who is the band
3. To have some reference to the music, either audio, video etc
4. Visual elements to get an idea of their performances

As a returning user

1. Provide information (such as tour dates) that they would like to know
2. To ensure the information they may be searching for always remains simple to find

As a potential booker of the band

1. To contact the band easily and be able to provide information for further contact
2. Getting an idea of what the band has made, with little issue with the layout
3. Seeing some past works, to see if the group is the right fit

# Design

## Fonts
* Roboto from google is the font used in the project, as it is easy to read and has a rather clean look. Sans-serif is the backup font 
for if Roboto does not load.
## Icons
* There will be icons used for links, and will be easily understandable and represent where they lead
## Colours
* Colours will be relatively muted, with white, black, greys, in order to emphasise the images and visual elements of the page
## Styling
* The site will be styled with the idea of "rule of thirds" in the index for maximum usability and aesthetics
* Lots of contast between the text and backgrounds
## Backgrounds
* For the contact page, there will be a faded out picture of the band, with a largely white filter to ensure it does not intrude with the content
## Images
* Images of the band performing that are of high enough quality to look good on multiple screen sizes and represent the band well
## Video
* The video(s) on the site will be an "introduction" of sorts to a new potential listener and will be accessable and respresent the band well

# Wireframes

## Index Page

### Large Index Page

![Large Index Page](/documentation/wireframes/indexlargescreen.png "Large Index Page")

### Medium Index Page

![Medium Index Page](/documentation/wireframes/indexmediumscreen.png "Medium Index Page")

### Small Index Page

![Small Index Page](/documentation/wireframes/indexsmallscreen.png "Small Index Page")

## Gallery Page

### Large Gallery Page

![Large Gallery Page](/documentation/wireframes/gallerylargescreen.png "Large Gallery Page")

### Medium Gallery Page

![Medium Gallery Page](/documentation/wireframes/gallerymediumscreen.png "Medium Gallery Page")

### Small Gallery Page

![Small Gallery Page](/documentation/wireframes/gallerysmallscreen.png "Small Gallery Page")

## Contact Page

### Large Contact Page

![Large Contact Page](/documentation/wireframes/contactlargescreen.png "Large Contact Page")

### Medium/Small Contact Page

![Small Contact Page](/documentation/wireframes/contactsmallscreen.png "Small Contact Page")

# Features
* Works well on all device sizes without any compromises on content
* Strongly interactive for a User
* Links to many forms of media

# Technology used

## Google Fonts
* Google Fonts "Roboto" font was used

## FontAwesome
* Varius FontAwesome logos were used in the project

## Git
* The version control on Gitpod was used to create commits and version control the project

## Github
* Github was used to store all versions commited from Gitpod

## Balsamiq
* Balsamiq was used to create various wireframes of different sizes of the site

# Testing

## Index Page validation

![Index Validation](/documentation/tests/indexpagecheck.PNG "Index Validation")

## Gallery Page validation

![Gallery Validation](/documentation/tests/indexpagecheck.PNG "Gallery Validation")

## Contact Page validation

![Contact Validation](/documentation/tests/contactpagecheck.PNG "Contact Validation")

## CSS validation

![CSS Validation](/documentation/tests/csscheck.PNG "CSS Validation")

# Lighthouse Testing

## Index Page (desktop)

![Index Desktop Lighthouse Check](/documentation/tests/indexdesktoplighthouse.PNG "Index Desktop Validation")

## Index Page (mobile)

![Index Mobile Lighthouse Check](/documentation/tests/indexmobilelighthouse.PNG "Index Mobile Lighthouse Check")

## Gallery Page (desktop)

![Gallery Desktop Lighthouse Check](/documentation/tests/gallerydesktoplighthouse.PNG "Gallery Desktop Lighthouse Check")

## Gallery Page (mobile)

![Gallery Mobile Lighthouse Check](/documentation/tests/gallerymobilelighthouse.PNG "Gallery Mobile Lighthouse Check")

## Contact Page (desktop)

![Contact Desktop Lighthouse Check](/documentation/tests/contactdesktoplighthouse.PNG "Contact Desktop Lighthouse Check")

## Contact Page (mobile)

![Contact Mobile Lighthouse Check](/documentation/tests/contactmobilelighthouse.PNG "Contact Mobile Lighthouse Check")

# Testing User Stories

## New User

1. As a first time user, it is important to understand the sites purpose and learn more
* This is accomplished with a large hero image displayed upon entering the site. There is a large 
call to action present in the middle of the page with a "learn moore" anchor element that brings 
the user to the information part of the site, ensuring they understand easily the purpose of the site.
The user also has the option to scroll down to lead to the same information.
* The nav bar gives easy and fluid navigation all around the site, and the footer leading to the bands 
social media ensures that a user can gain a strong interactivity with the website.

2. Understanding the band (who is in it, information about shows and some media reference)
* This is accomplished by having a link to a bio, streamable music and a music video all on the same 
page, in order to provide a variety of choices and provide the new user with all the information and media 
that they could possible need to decide on if this band will be a good choice for them.

3. Having visual reference
* Visual reference is provided by an easy to find Gallery button in the nav bar, that can give the new user 
a complete idea about the types of performance this band would usually do, and provide them with an impression 
of the way the band appears performing. This is easy to find and will more than likely be the part of the site 
they explore after they have read the bio and seen the other media on the index page. The gallery is simplictically 
laid out for this purpose, and is eye catching when opened.

## Returning User

1. A returning user often is familiar with the sites purpose and media, and so will be more than likely looking for updates
* This is accounted for by the bio in the index page that is very easy to access the second the user enters the site. This contains 
the type of information that would be more regularly updated, such as tour dates, and the latest music video and it makes accessing this 
information very simple for the returning user.

2. The returning user could potentially be back to book the band
* This necessitated having the contact page be easy to find and not obstructed with any other information.

## Potential Booker

1. A booker of the band will want a complete idea of what the band is like
* having a wide array of information for them to see (music links, video, and images) will give them a rather complete impression of the band 
and what they are like. Navigating these must be simple, especially for a booker, and having music links, video and a bio on the index page then 
the gallery only one click away makes this a trivial task that can be accomplished rather quickly, with no frusteration.

2. A booker will want an easy way to contact the band
* The contact page is given its own html page, thus to make sure it does not get lost within any other information present on the website. 
This also gives incentive to book them, as having the option present at all times could potentially give the idea to the booker if they 
are impressed with the other media on the website.


# Further testing

* site tested on various desktop sizes and on google chrome, opera and 

# Deployment






# Bugs solved

## Header ordering issue
The header was loading the anchor links in the wrong order, so I reversed the order they were placed in.

Was previously
            <a class=" header-a-box large-resolution-header" href="index.html">Home</a>
            <a class=" header-a-box large-resolution-header" href="gallery.html">Gallery</a>
            <a class=" header-a-box large-resolution-header" href="contact.html">Contact us</a>

Is now
            <a class=" header-a-box large-resolution-header" href="contact.html">Contact us</a>
            <a class=" header-a-box large-resolution-header" href="gallery.html">Gallery</a>
            <a class=" header-a-box large-resolution-header" href="index.html">Home</a>

## Images not rendering issue
Images would fail to load without any indication of why (Correct file paths, correctly written names etc). The problem was the specifity of the file paths

Was previously
            background-image: url("/assets/images/heroimg");
            src="/assets/images/album-cover.jpg">

Is now

            background-image: url("../images/heroimg");
            src="./assets/images/album-cover.jpg">

## Page shortness on contact page 
The page was slightly too short on a specific screen size (ipad pro vertical) **updated to be general rule**

Added 
        @media screen and (max-width: 800px) and (min-height: 977px){
            #contact-wrap{
                padding: 60px 0;
            }
        }

## Error with i element formatting on drop bar
The two icons appeared seperately but it was a small formatting error

was 

            <i class="fas fa-bars header-fa"></i>
            <i class="fas fa-caret-down header-fa"></i>

Is now

        <i class="fas fa-bars header-fa"></i><i class="fas fa-caret-down header-fa"></i>

## Error with padding sizes on contact page
The padding was often too small to fill the screen and would leave a white portion at the botton under the header. A height increase fixed the problem

from
        padding: 30px 0;

To
        padding: 60px 0;

## Gallery distortion error
When the gallery section was divided in 2 columns, it was compressed into the left quarter of the screen without any explanation. 
However, it turned out the large scale nav bar, despite not being visible, was pushing the two columns to the left so a media query was
placed to set it to take up no space when invisible.

        nav-header{
            height: 0;
            width: 0;
        }

# Credits

## Media

### Images
* All images are screenshots from NBC's "Parks and Recreation"
