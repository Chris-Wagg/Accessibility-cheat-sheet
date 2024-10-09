# Screen reader basics

[A11Y-Checklist](https://www.a11yproject.com/checklist/)

## where to start...

-   HTML mark-up: Does your website use semantic HTML mark-up for elements like headings, paragraphs, lists, tables and forms?

-   Alternative text: Does your website use descriptive alternative text for images, icons and non-text content? (only for informative images, decorative images will have null alts)

-   Keyboard compatibility: Is your site navigable using keyboard-only commands?

-   Visually-led content: Is your web content understandable without visual cues? For example, is link text descriptive? Do instructions require a visual cue, e.g. click on the red box to download?

-   Dynamic content: With content becoming increasingly complex and dynamic, moving and changing elements on a screen can be an obstacle to comprehension. Disabling automatic carousels and autoplay on multimedia content helps put the user in control of their site experience.

-   Accessibility overlays: Websites with an accessibility overlay can actually make it trickier for screen reader users to read content. They sometimes disrupt screen readers from interpreting the page correctly and pose an obstacle to effective navigation. If your website has an accessibility overlay installed, it’s very important to check that it works properly with screen reader testing, or you could be excluding the very people you’re trying to include.

## Checklsit

-   Check for missing/improper headings on your pages

-   Think about if you need hidden headings or not

-   Check for presence of ‘skip to main content’ and ‘skip navigation’ links (use anchor links for this)

-   Check the lang attribute is correct

-   Complete a fill form – are the labels and prompts working as expected?

-   Interact with call-to-action buttons

-   Interact with data tables – they should only be used for tabular data if present

-   Check image alt text for descriptiveness

-   Check link text for descriptiveness

-   Check button text for descriptiveness. Inner text is best, aria-label is also good

-   Should it be a button or a link?

-   should it be a link or a heading?

-   groups of inline elements (eg: links) should be grouped in lists
-   -   this is important for popouts/ dialogues

-   Check common problematic elements, like CAPTCHA, accessibility overlays, unexpected screen changes and Flash content

-   Check that the search functionality is present and functional

-   check colour contrasts on text etc...

-   Check that automatic carousels and autoplay are disabled if needed
