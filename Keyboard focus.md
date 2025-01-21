# keyboard focus

## Focus order

-   you can add tab index to include elements within the tab order that would normally not be in it

    -   using `tabindex='0'` will add it to the focus list
    -   using `tabindex='-1'` will remove it from the focus list
        -   javascript can be used to change a -1 tabindex to add it back into the focus list when needed

-   it's generally best to avoid adding positive tabindex to an element, this will mess with the focus order

## Skip links

-   sikp links will help keyboard users to skip to main content. Use an anchor tag for this ` <a href="#content" class="visually-hidden">Skip to main content</a>` you can target an ID of another tag

## Focus styling

-   best to leave the default styling for focus. Removing it is bad for AT. If you are going to chane default focus then make sure there is still visible focus.

eg: `a:focus {
  outline: auto 5px Highlight; /* for non-webkit browsers */
  outline: auto 5px -webkit-focus-ring-color; /* for webkit browsers */
}`
