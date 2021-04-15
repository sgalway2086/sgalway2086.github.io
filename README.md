# Milestone-1-Project

## UX

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

![Large Index Page](/documentation/wireframes/indexlargescreen.png "Large Index Page")

#### Medium Index Page

![Medium Index Page](/documentation/wireframes/indexmediumscreen.png "Medium Index Page")

#### Small Index Page

![Small Index Page](/documentation/wireframes/indexsmallscreen.png "Small Index Page")

### Gallery Page

#### Large Gallery Page

![Large Gallery Page](/documentation/wireframes/gallerylargescreen.png "Large Gallery Page")

#### Medium Gallery Page

![Medium Gallery Page](/documentation/wireframes/gallerymediumscreen.png "Medium Gallery Page")

#### Small Gallery Page

![Small Gallery Page](/documentation/wireframes/gallerysmallscreen.png "Small Gallery Page")

### Contact Page

#### Large Contact Page

![Large Contact Page](/documentation/wireframes/contactlargescreen.png "Large Contact Page")

#### Medium/Small Contact Page

![Small Contact Page](/documentation/wireframes/contactsmallscreen.png "Small Contact Page")



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

### Page shortness on contact page 
The page was slightly too short on a specific screen size (ipad pro vertical) **updated to be general rule**

Added 
        @media screen and (max-width: 800px) and (min-height: 977px){
            #contact-wrap{
                padding: 60px 0;
            }
        }

### Error with i element formatting on drop bar
The two icons appeared seperately but it was a small formatting error

was 

            <i class="fas fa-bars header-fa"></i>
            <i class="fas fa-caret-down header-fa"></i>

Is now

        <i class="fas fa-bars header-fa"></i><i class="fas fa-caret-down header-fa"></i>

### Error with padding sizes on contact page
The padding was often too small to fill the screen and would leave a white portion at the botton under the header. A height increase fixed the problem

from
        padding: 30px 0;

To
        padding: 60px 0;

### Gallery distortion error
When the gallery section was divided in 2 columns, it was compressed into the left quarter of the screen without any explanation. 
However, it turned out the large scale nav bar, despite not being visible, was pushing the two columns to the left so a media query was
placed to set it to take up no space when invisible.

        nav-header{
            height: 0;
            width: 0;
        }

## Testing

### Site Function Testing

#### Header and Footer
The header and footer were tested first, on all three of the html pages, ensuring the transition effect and the links all functioned correctly 
on each of the pages.

#### Index Page
The index page was tested first by checking the call to action on the hero image was functional and lead to the information section as
well as creating an underline effect when hovered over. After successfully going to the div, I checked all the external links on the page, 
ensuring that the links to spotify and apple music had functional links that opened seperate tabs.For the mobile friendly versions of the site 
it was important to ensure that all the divs moved as intended, and I checked they changed position without issue and correctly to prevent any 
sort of distortions within the page. The hover function on the music links functioned well.

![Index Test](/documentation/tests/heroimage.PNG "Index Test")

![Index Bio Test](/documentation/tests/index.PNG "Index Bio Test")

##### Smaller screen

![Index Small Bio Test](/documentation/tests/indexsmall.PNG "Index Small Bio Test")

#### Gallery
The gallery page was tested primarily by changing the size of the display size to ensure the columns worked. Ensuring correct scrolling and 
movement of the images within the columns was crucial to an ideal user experience. The 4 sizes for various resolutions all functioned very
satisfactorily 

![Gallery test](/documentation/tests/gallery1.PNG "Gallery test")

##### Smaller screen

![Gallery small test](/documentation/tests/gallery2.PNG "Gallery small test")

#### Contact Page
The contact page was tested, as with the previous two, by adjusting the screen size to ensure the layout would be suitable on all resolutions.
The forms functions (the inputs and submit button) all functioned as intended. The hover function on the submit form worked as intended.

![Contact test](/documentation/tests/contact.PNG "Contact test")

##### Smaller screen

![Contact small test](/documentation/tests/contact2.PNG "Contact small test")

### HTML/CSS Validating
After testing the site thoroughly to ensure ideal function, the HTML and CSS was in need of testing. After some mild adjustments, all pages 
passed validation without issue

### Drop bar
The drop bar functioned very well, and changed to fit when the media query activates. It switched seemlessly from the large contact bar to the 
drop bar.

#### Index Page validation

![Index Validation](/documentation/tests/indexpagecheck.PNG "Index Validation")

#### Gallery Page validation

![Gallery Validation](/documentation/tests/indexpagecheck.PNG "Gallery Validation")


#### Contact Page validation

![Contact Validation](/documentation/tests/contactpagecheck.PNG "Contact Validation")


#### CSS validation

![CSS Validation](/documentation/tests/csscheck.PNG "CSS Validation")



### Lighthouse Testing

#### Index Page (desktop)

![Index Desktop Lighthouse Check](/documentation/tests/indexdesktoplighthouse.PNG "Index Desktop Validation")

#### Index Page (mobile)

![Index Mobile Lighthouse Check](/documentation/tests/indexmobilelighthouse.PNG "Index Mobile Lighthouse Check")

#### Gallery Page (desktop)

![Gallery Desktop Lighthouse Check](/documentation/tests/gallerydesktoplighthouse.PNG "Gallery Desktop Lighthouse Check")

#### Gallery Page (mobile)

![Gallery Mobile Lighthouse Check](/documentation/tests/gallerymobilelighthouse.PNG "Gallery Mobile Lighthouse Check")

#### Contact Page (desktop)

![Contact Desktop Lighthouse Check](/documentation/tests/contactdesktoplighthouse.PNG "Contact Desktop Lighthouse Check")

#### Contact Page (mobile)

![Contact Mobile Lighthouse Check](/documentation/tests/contactmobilelighthouse.PNG "Contact Mobile Lighthouse Check")

## Credits

### Code

* Google Fonts "Roboto" font was used
* Varius FontAwesome logos were used in the project

### Media

#### Images
* All images are screenshots from NBC's "Parks and Recreation"
