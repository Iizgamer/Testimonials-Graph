# CTI-110 Final Project - Testimonials Grid by Nicholas Foles

## Table of contents

- [CTI-110 Final Project - Testimonials Grid by Nicholas Foles](#cti-110-final-project---testimonials-grid-by-Nicholas-Foles)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [The challenge](#the-challenge)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Continued development](#continued-development)
    - [Useful resources](#useful-resources)
  - [Author](#author)
  - [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size

### Screenshot

./desktop-view.png

./mobile-view.png

### Links

- Repository URL: https://github.com/Iizgamer/Testimonials-Graph.git
- Live Site URL: https://iizgamer.github.io/Testimonials-Graph/index.html

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Hopes, dreams, and duct tape

### What I learned

I learned that making a website 1 to 1 to a design is quite hard. I had previously done it once before, but that desing was quite bare bones, contrasting to this website, which had several difficult areas. One of those specific areas were the quotation marks behind the text in Daniel Clifford's review box. I solved it through the use of divs and the position CSS variable.

'''css
#overlapcontainerdaniel {
    position: relative;
    background-color: hsl(263, 55%, 52%);
}

#quote-img {
    background-color: hsl(263, 55%, 52%);
    margin-top: -67px;
    margin-left: 390px;
    position: absolute;
}

#bigtextclifford {
    font-weight: bold;
    font-size: 20px;
    margin-top: 10px;
    margin-bottom: 0px;
    border-radius: 0px;
    position: relative;
    background-color: transparent;
}
'''

After figuring out Daniel Clifford's box, it was quite easy to solve the rest, as I had a sort of template to go off of now. However, after that, I did struggle with making it mobile-accessible. The way I solved this was through the use of the @media (max-width) variables in CSS.

'''css
@media (max-width: 900px) {
    body {
        margin: 0px;
        margin-left: 60px;
        margin-top: 20px;
    }

    #danielcliffordbox {
        width: 300px;
        float: left;
        margin-right: 20px;
        box-shadow: 10px 20px 10px 0px rgba(186, 186, 186);
        margin-bottom: 20px;
    }

    #quote-img {
        display:none;
    }

    #waltersbox {
        width: 300px;
    }

    #harmonbox {
        width: 300px;
    }

    #abramsbox {
        width: 300px;
        margin-top: 20px;
        margin-left: 0px;
        height: 350px;
    }

    #whittlebox {
        width: 300px;
        margin-left: 0px;
        margin-top: 20px;
        height: 430px;
    }

    #whittleimg {
        margin-top: 10px;
    }

    #whittlesubtitle {
        margin-left: 0px;
        padding-left: 0px;
    }

    .attribution {
        margin-left: 50px;
        margin-right: 90px;
    }
}
'''

### Continued development

One area that I think would be very beneficial to learn would be the ability to make my CSS and HTML be automatically adjustable to screens using only a few lines of code, as opposed to me having to manually adjust everything. In fact, it would be beneficial for me to learn how to make everything automatic, instead of using negative margins.

### Useful resources

- https://pavellaptev.medium.com/css-weekly-2-an-image-on-the-left-text-on-the-left-a5e59b2acdb5 - This helped me learn how to align an image on the left, whilst keeping the text on the right. This specifically helped me with the image then the name and title in the cards.
- https://stackoverflow.com/questions/49243420/how-to-move-element-in-css-up-so-that-elements-underneath-will-follow - This helped me understand how margins, borders, and paddings worked. It also made me use a negative margin, though, so...

- https://www.w3schools.com/css/tryit.asp?filename=trycss_zindex3 - This helped me understand how to overlap elements over others.

## Author

- Website - Nicholas Foles: https://github.com/Iizgamer

## Acknowledgments

Sami: Helped me throughout this entire project. Especially in the mobile layout section.