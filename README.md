# Fylo Landing Page with Two Column Layout

<p align="left">
  <img src="https://img.shields.io/badge/Difficulty-Junior-brightgreen?style=for-the-badge" alt="Difficulty">
  <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/vanzasetia/fylo-landing-page-two-column-layout?style=for-the-badge">
  <a href="https://twitter.com/vanzasetia" target="_blank"><img src="https://img.shields.io/twitter/follow/vanzasetia?logo=twitter&style=for-the-badge" alt="Twitter followers." /></a>
  <img alt="Netlify" src="https://img.shields.io/netlify/?style=for-the-badge">
</p>
<p>
  <a href="http://jigsaw.w3.org/css-validator/check/referer">
    <img style="border:0;width:88px;height:31px"
        src="http://jigsaw.w3.org/css-validator/images/vcss-blue"
        alt="Valid CSS!" />
    </a>
</p>

## Feedback and Live Review
* [🌍 Live Review](https://fylocloudstorage.netlify.app/)
* [👉 Give feedback on Frontend Mentor platform]()
* [🐦 Give Feedback on Twitter]()

## Table of contents
- [Story](#the-story-when-doing-this-challenge)
  - [When I Build the Header](#header)
  - [When I Build the Hero Section](#hero)
  - [When I Build the Productive Section](#productive-section)
  - [When I Build the Testimonial Section](#testimonial-section)
  - [When I Build the CTA Section](#cta-section)
  - [When I Build the Footer](#footer)
- [What I Learned](#what-i-learned)
- [Technology that I used](#built-with)
- [Useful Resources](#useful-resources)
- [Continued Development](#continued-development)

## The Story When Doing This Challenge

### Header
This time, there was no active-states preview for the links on header. So, I created my own active-states.

### Hero
If you see the mobile design and compare it to the desktop design, you will see that the `.hero__title` has different font family 😂.

```html
<h1 class="hero__title">
  All your files in one secure location, accessible anywhere.
</h1>
```

I changed the color of bg-curve from `#F8F8FE` to `#f6f6fe`, so it has the same color as the background color of the next section.

### Productive Section
On mobile design, the `productive__description` has desaturated blue color, but on desktop design it has very dark blue. So, I chose to make it very dark blue color.

If you see the mobile design then you may notice that `See how Fylo works` link is on the center. But, for an unknown reason, the `productive__link` doesn't want to go to the center even though I already tried a couple things like using flexbox and `text-align: center`. 

I know that I can make it center by wrapping the link with `div`, then using absolute positioning on the link and make `top: 50%` and `left: 50%`, after that I add `transform: translate(50%, 50%)`. But, seriously?! It's too **overkill** in my opinion. So, I'm just leave as it is, since on the big screen it doesn't need to be in the center. It's also make the layout looks consistent.

### Testimonial Section
The original quotes icon `images/icon-quotes.svg` does not look similar as the design, so I downloaded another quotes icon from [Flaticon](https://www.flaticon.com/) which looks more similar to the design.

The `style-guide.md` said that you only need an **Open Sans** font family with 400 weights **only**. But when I see **Kyle Burton** text 😐, it needs **Open Sans** font family with **700 weights** 😫.

### CTA Section 
When I started building the mobile layout, I realized that the layout on mobile design wasn't consistent. This section had less width than the other section. So, I didn't follow the mobile design, I was just using the same `.container` as the other section had. That way, the layout is always consistent even in mobile devices 👍.

### FOOTER
For the footer, I use `grid` to make them three columns on desktop view.

## What I Learned
* Using `rel="preload"` and `font-display: optional` to prevent shifting layout on font family. But I used `font-display: swap` since if you import it using `link` tags, there this `&display=swap`.
* I learned that using `woff2` font format is better than using `ttf`. The reason for that is because `woff2` has smaller file size which is equal to better performance 🚀.
* I learned that `img` must have `width` and `height` attributes to prevent jumping layout.
* I also found out a link that explain, why you need `role="contentinfo"` on `footer`. The link in [Useful Resources section](#useful-resources).


## Built With
This project is created using **HTML5**, **CSS3**, and **Sass**. 

I used one of the form features from [Netlify which Forms Spam Filters](https://docs.netlify.com/forms/spam-filters/), using **Honeypot field**.

I also used [Mailgo](https://mailgo.dev/), which is a light JavaScript library for `mailto` and `tel`. It will give you a nice popup for every `mailto` and `tel` link. I really ❤️ love this library, since it is **easy** and **simple** to use.
<p align="left">
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg" alt="" width="auto" height="70px">
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg" alt="" width="auto" height="70px">
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/sass/sass-original.svg" alt="" width="auto" height="70px">
  <img src="./images/mailgo.png" alt="" width="auto" height="70px">
</p>

## Useful Resources
* [Optimize Cumulative Layout Shift](https://web.dev/optimize-cls/)
* [Form Validation UX in HTML and CSS](https://css-tricks.com/form-validation-ux-html-css/)
* [Preload web fonts to improve loading speed](https://web.dev/codelab-preload-web-fonts/)
* [Prevent layout shifting and flashes of invisible text (FOIT) by preloading optional fonts](https://web.dev/preload-optional-fonts/)
* [Font Converter from any format to any format that you want](https://www.fontconverter.io/en)
* [<footer> | MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/footer#accessibility_concerns)

## Continued development
I will take people feedback and improve this solution.