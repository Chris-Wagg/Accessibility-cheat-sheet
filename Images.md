# Images

## Purpose & context

-   Questions to ask first...

    -   Is it esential for context or understanding?
    -   What info is it conveying?
    -   Is it simple or complex?
    -   Does it elicit emotion or prompt action?
    -   It is just decorative?

-   Hide the images on a page and see if you can still understand everything. If you can then it's decoratve, if not then it probably serves some sort of purpose.

## Decorative images

-   Need to be hidden from AT's.
-   Can use empty alt texts, `use aria=none`, `aria-hidden=true` or add it as a background image with css.

    -   Be careful when using the aria methods, as it will remove the whole element and potential children. test it to make sure it works as intended.

## Informative images

-   When using something like an SVG, you might need to add `role=img` to make sure AT's pick up on them.
-   You can also add a `<title>` to an SVG to add a descriptive text sort of thing.

> [!NOTE]
> Some users still want to hear descriptions of images, if in doubt just add alt text and the user can skip it if they want

## Functional images

-   These are connected to actions, eg a logo that goes to a homepage, a magnifying glass search button, a social media logo/button.
-   These still need to include alt text or descriptions to inform what the action does.
    -   One way to do this is with text hidden via css.

`<div title="Navigate to the homepage">
<a href="/">
<img src=".../Ladybug_Logo.png" alt="Lovely Ladybugs for your Lawn"/>
</a>

</div>`

When read with a screen reader, both the title and alt will be read, informing the user of both the visual and action components.

## Complex images

-   Needs more information than any of the other image types. Will have both short and long alt texts.
-   You can use skip links to link to another part of the page with an explanation on it.
-   You can also use `aria-describedby` on the `img` element so you can link to a longer explanation. The description can also be visually shown or hidden, but it's probably best to keep it shown to support the most people.
-   You can also use `figure` and `figcaption`, it's similar to `aria-describedby`.
    [Check the link here for more info](https://web.dev/learn/accessibility/images#complex_images)

### Best practices

-   Alt texts should be as descriptive but succinct as possible.
-   Apparently 150 characters is the recommended max length of a good alt text?
-   If more info is needed then use one of the complex image patterns

Other good practices...

-   Avoid using words like "image of" or "photo of" in the description
-   When naming your images, be as consistent and accurate as possible. Image names are a fallback when the alternative text is missing or ignored.
-   Avoid using non-alpha characters and use dashes between words rather than underscores in your image names or alternative text.
-   Use proper punctuation whenever possible.
-   Write alternative text like a human and not a robot. Keyword stuffing does not benefit anyone—people using screen readers will be annoyed, and search engine algorithms will penalize you.
