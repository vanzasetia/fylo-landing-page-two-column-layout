# Fylo Landing Page with Two Column Layout

## Disclaimer

This project is solely for learning purposes. I take no any responsibility or liability for the accuracy, completeness, or usefulness of any information provided in this project. You should not use it as a reference for creating your project.

I am currently no longer working on this project.

## Links

- [Live Review](https://fylocloudstorage.netlify.app/)
- [Give feedback on Frontend Mentor platform](https://www.frontendmentor.io/solutions/fylo-two-columns-layout-landing-page-html5-css3-sass-mailgo-eB98lZ5w1)

## The Story When Doing This Challenge

### Header

This time, there was no active-states preview for the links on header. So, I created my own active-states.

### Hero

If you see the mobile design and compare it to the desktop design, you will see that the `.hero__title` has different font family.

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

The `style-guide.md` said that you only need an **Open Sans** font family with 400 weights **only**. But when I see **Kyle Burton** text, it needs **Open Sans** font family with **700 weights**.

### CTA Section

When I started building the mobile layout, I realized that the layout on mobile design wasn't consistent. This section had less width than the other section. So, I didn't follow the mobile design, I was just using the same `.container` as the other section had. That way, the layout is always consistent even in mobile devices 👍.

### Footer

For the footer, I use `grid` to make them three columns on desktop view. I also make the social media circle bigger than the design. It's also an accessibility, to make sure that they are easy to click by the user.

## What I Learned

- Using `rel="preload"` and `font-display: optional` to prevent shifting layout on font family. But I used `font-display: swap` since if you import it using `link` tags, there is this `&display=swap`.
- I learned that using `woff2` font format is better than using `ttf`. The reason for that is because `woff2` has smaller file size which is equal to better performance.
- I learned that `img` must have `width` and `height` attributes to prevent jumping layout.
- I also found out a link that explain, why you need `role="contentinfo"` on `footer`. The link in [Useful Resources section](#useful-resources).


## Built With

This project is created using **HTML5**, **CSS3**, and **Sass**. 

I used one of the form features from [Netlify which Forms Spam Filters](https://docs.netlify.com/forms/spam-filters/), using **Honeypot field**.

I also used [Mailgo](https://mailgo.dev/), which is a light JavaScript library for `mailto` and `tel`. It will give you a nice popup for every `mailto` and `tel` link.

## Useful Resources

- [Optimize Cumulative Layout Shift](https://web.dev/optimize-cls/)
- [Form Validation UX in HTML and CSS](https://css-tricks.com/form-validation-ux-html-css/)
- [Preload web fonts to improve loading speed](https://web.dev/codelab-preload-web-fonts/)
- [Prevent layout shifting and flashes of invisible text (FOIT) by preloading optional fonts](https://web.dev/preload-optional-fonts/)
- [Font Converter from any format to any format that you want](https://www.fontconverter.io/en)
- [ Footer Tag | MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/footer#accessibility_concerns)

## License

[MIT](./LICENSE)
