# 048-Responsive-Design-Media-Queries-templ

048 responsive design + media queries

Today’s goals:
    Learn about different approaches for responsive web design
    Begin learning about CSS media queries
 Today’s featured site:
    https://photos.icons8.com/creator – Create your own stock photos!
 Creating Responsive Webpages: Some Approaches

    Responsive web design is the act of making your webpage look good on a variety of screen sizes. There are many different ways to create a responsively designed webpage. We are going to learn a few particular methods and frameworks over the next few weeks. There are many tools and approaches to help create a responsively designed site, some of which you will learn.
        Use the auto value for width and height. What happens when we do this? What determines the width and height when the value is auto?
        Use percentages for margins and width/height values. Why would this approach be more responsive than using pixels (example- width: 50% vs width: 300px)?
        Media queries: changing CSS styles at certain screen widths. Things to consider: when does your design break? What CSS style changes can be made to adjust for certain screen widths? Common changes include the page layout, menu design, and background images.
        Frameworks: We will look at Skeleton and Bootstrap. What are these? Why do people use them?
        New: CSS grid layout and flexbox layout
    Mobile first: the approach of designing your site first for a small screen and scaling up.
    Website vs mobile apps: what is the major difference between websites and mobile apps?

 CSS Media Queries
           CSS media queries are used to change CSS styles when the screen (or view port) is a certain width. Screen/view port sizes are selected by determining when a design “breaks.” For example, in the Dallas Art Fair site we looked at, a video was used as a background for larger view ports, such as computer screens, and an image was used for smaller view ports. Media queries can be used to change a background image, page layout, or menu design (among many other things) when these things don’t look right at certain view ports (such as a video background image on a small screen such as a phone).
        What we are doing to our page: We are going to change up our original Zombies page by adding a header, footer, and sidebar menu. We are going to add new CSS for different media queries to change how our page looks on different screen sizes.
        header– located at top of page, width 100% for each screen
        footer– located at bottom of page, width 100% for each screen
        nav– contains the Major Keys and is the page menu. Nav is 100% width on the smallest screen and is a horizontal menu across the top below the header and above the section. Nav then becomes a sidebar for larger screens, so its width changes to a smaller percentage and it is floated to the left so it will be next to section. The nav’s menu items go from being horizontally displayed to vertically displayed on the larger screens.
        section– contains picture and text. Section is 100% width on the smallest screen and then floats to the right so the nav can fit next to it on the larger screens. 
Practice code: Download the broken practice code
    Open a new Notepad++ page, copy and paste the code, save it as 048_mediaqueries.html, and then launch it in the browser. What happens when you resize the browser window? What do the media queries do?
    Let’s open the page in Firefox and go into Responsive Design Mode. Let’s check out the page just before it hits 500px and 900px. What happens? Why?
    Why does the box still float to the left when the screen size hits 900px and above?
    Let’s add some more media queries. What should happen if we design for a smaller screen? What about a larger one? Specifically, what width should the box be?
    Can you add other CSS style properties to the separate media queries? Let’s try adding background colors to each media query.
    What would happen if we add more boxes to our page? Let’s try it.
    Let’s fix the ???? in our media query
        We have a media query for small screen sizes but 320px isn’t a good break point. Let’s launch the page in Firefox and open responsive design mode to determine what would be a better (higher) number to use based upon how our page looks. Let’s look at page on different devices.
        Let’s see how nav looks at 401px and up. How can we fix the text so it doesn’t wrap to two lines? Let’s create a new media query by copying and pasting the old one and fixing the code (and adding a new background-color to nav).
        Let’s see how the nav looks as the screen gets bigger. How can we fix it so the nav doesn’t seem too large for the text? Let’s create a new media query by copying and pasting the old one and fixing the code (and adding a new background-color to nav). Maybe instead of using percentage values, what value can we use that will “automatically” adjust to fit the content? Let’s also add some padding.
        What are the new break points (where the style changes happen?)
        Why does our page look the way it does between 441px and 534px? Where are the styles coming from?
