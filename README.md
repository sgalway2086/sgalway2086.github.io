# Milestone-1-Project

##UX

### Project Goals

The goal of the project is to provide a website, with a clean and easy to understand but still visually-appealing layout to a potential customer of the band. 
Providing the user with easy access to the media of the band, such as audio, video and social media links that are easy to find, as well as a contact page.
The target demographic is to be potential listeners, hence the importance of easily accessable media and potential bookers, necessitating a specialised contact page.

### User Goals

*Clearly laid out information
*Intuitively being able to figure out how to navigate the site
*Images and strong visual elements
*audio and video accessable for new visiters who are interested in the band

### Why the site meets this intended purpose

* Minimalist, but eye-pleasing layout with clearly labeled buttons
* A layout that follows the way a user will often use an unfamiliar website and is simply laid out
* A hero image and gallery section, with a minimalist color scheme surrounding to ensure they stand out
* Some form of video and audio content accessable from the index page

### A potential booker of the band

* Being able to easily book the band if they want
* Access to information to see if they will book, necessating a strong media presence.

### Why the site meets this intended purpose

* Specialised contact page in order to make access very obvious to a user within seconds
* Strong media presence on site
Multiple alternative contact routes, with social media links

## Developer and Business Goals

* Website to increase the amount of business the band recieves
* To increase traffic to social media and other online media from the band
* Creating a website with a strong layout, and good use of CSS for compatability and usability
* A project the developer can use for a portfolio

## User Stories

As a new user, who may never have heard of the band

1. To be able to learn about the members/who is the band
2. To have some reference to the music, either audio, video etc
3. Visual elements to get an idea of their performances
4. Intuitively knowing the websites purpose when arriving

As a potential booker of the band

1. To contact the band easily and be able to provide information for further contact
2. Getting an idea of what the band has made, with little issue with the layout
3. Seeing some past works, to see if the group is the right fit

## Design Choices

### Fonts
* Roboto from google is the font used in the project, as it is easy to read and has a rather clean look
### Icons
* There will be icons used for links, and will be easily understandable and represent where they lead
### Colours
* Colours will be relatively muted, with white, black, greys, in order to emphasise the images and visual elements of the page
### Styling
* The site will be styled with the idea of "rule of thirds" in the index for maximum usability and aesthetics
* Lots of contast between the text and backgrounds
### Backgrounds
* For the contact page, there will be a faded out picture of the band, with a largely white filter to ensure it does not intrude with the content
### Images
* Images of the band performing that are of high enough quality to look good on multiple screen sizes and represent the band well
### Video
* The video(s) on the site will be an "introduction" of sorts to a new potential listener and will be accessable and respresent the band well


## Wireframes

### Index Page

#### Large Index Page

![Large Index Page](/assets/wireframes/indexlargescreen.png "Large Index Page")

#### Medium Index Page

![Medium Index Page](/assets/wireframes/indexmediumscreen.png "Medium Index Page")

#### Small Index Page

![Small Index Page](/assets/wireframes/indexsmallscreen.png "Small Index Page")

### Gallery Page

#### Large Gallery Page

![Large Gallery Page](/assets/wireframes/gallerylargescreen.png "Large Gallery Page")

#### Medium Gallery Page

![Medium Gallery Page](/assets/wireframes/gallerymediumscreen.png "Medium Gallery Page")

#### Small Gallery Page

![Small Gallery Page](/assets/wireframes/gallerysmallscreen.png "Small Gallery Page")

### Contact Page

#### Large Contact Page

![Large Contact Page](/assets/wireframes/contactlargescreen.png "Large Contact Page")

#### Medium/Small Contact Page

![Small Contact Page](/assets/wireframes/contactsmallscreen.png "Small Contact Page")



## Bugs solved

### Header ordering issue
The header was loading the anchor links in the wrong order, so I reversed the order they were placed in.

Was previously
            <a class=" header-a-box large-resolution-header" href="index.html">Home</a>
            <a class=" header-a-box large-resolution-header" href="gallery.html">Gallery</a>
            <a class=" header-a-box large-resolution-header" href="contact.html">Contact us</a>

Is now
            <a class=" header-a-box large-resolution-header" href="contact.html">Contact us</a>
            <a class=" header-a-box large-resolution-header" href="gallery.html">Gallery</a>
            <a class=" header-a-box large-resolution-header" href="index.html">Home</a>

### Images not rendering issue
Images would fail to load without any indication of why (Correct file paths, correctly written names etc). The problem was the specifity of the file paths

Was previously
            background-image: url("/assets/images/heroimg");
            src="/assets/images/album-cover.jpg">

Is now

            background-image: url("../images/heroimg");
            src="./assets/images/album-cover.jpg">


## Credits

### Code

* Google Fonts "Roboto" font was used
* Varius FontAwesome logos were used in the project

### Media

#### Images
* All images are screenshots from NBC's "Parks and Recreation"
