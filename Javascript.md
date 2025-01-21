# Javascript

-   overuse of JS and injection of HTML or CSS through JS can lead to bad accessibility

## Trigger events

-   don't put onclick() on a div, only have things like that on elements that are meant to be interacted with, eg a button or anchor
-   if you add a trigger event to a non-semantic element then you need to add key down/up listiners etc which get messy

## Page titles

-   good page title are important
-   navigating to other pages should ideally change the title to annouce to users that they are somewhere different
-   `document.title` can be added manually or with helper packages, Announcing this change can mean more work but we have options

### Dynamic content

-   using a `querySelector` with `.innerHTML` can dynamically change an element on the webpage, be it adding text or changing a style eg: `document.querySelector("#banner").innerHTML = '<p>You are now signed in</p>';` or `document.querySelector("#banner").setAttribute("style", "border-color:#0000ff;");`

-   be sure to not misuse these features though eg...
    -   only use something like `.innertext` to insert small amounts of semantic text
    -   use a `setTimeout()` to make sure users hear the full message before something changes
    -   ideally all your CSS should be kept in the CSS sheet to avoid issues with conflicting inline additions. If you are going to dynamically change the CSS then toggle a class, not a specific style.

## Focus management

### Component level

-   It's important to know when to use a focus trap properly
-   When using a modal for example, a user should be trapped within the modal until they explicitly dismiss it

### Page level

-   Important to think about where the focus goes when the page changes (routes) or refreshes. Where to put the focus can be either context or action dependent.

    -   There are multiple techniques to achieve this:
        -   Place focus on the main container with an aria-live announcement.
        -   Put the focus back to a link to skip to the main content.
        -   Move the focus to the top-level heading of the new page.

## State management

### Component level

-   lots of different ways to announce changes to components - `aria-expanded` can be used when a component is open or closed to indicate which state it's in.

```
    <button id="toggle" aria-expanded="false">
    ...

```

You would when use JS to toggle this to true when the component is opened

-   you could also use something like `aria-pressed` yo indicate a toggle has happened. [See the documentation here](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-pressed)

-   be careful to not add to much aria though. no aria is better than bad aria. Think about the flow and critical info that should be conveyed to the user

### Page level

-   aria live regions can be used to announce changes for AT.
-   For the content to be properly read the live region must be in the DOM on load, then text can be dynamically added or changed
-   Amost all JS frameworks have accessible announcer packages

    React has...

    -   [React-aria-live](https://www.npmjs.com/package/react-aria-live)
    -   [React-a11y-announcer](https://github.com/thinkcompany/react-a11y-announcer)
