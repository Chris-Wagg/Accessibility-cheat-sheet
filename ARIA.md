# ARIA

## Chrome dev tools

-   Chrome dev tools has the accessibility tree to check this stuff, use it!

## 5 rules of ARIA

### #1 Don't use ARIA

-   no ARIA is better than bad aria. use semantic HTML first

### #2 Don't add unnecessary ARIA

-   Again, use semantic HTML, most of the time it will do what you need it to without adding ARIA

### #3 Always support keyboard navigation

-   all interactive controls must be keyboard accessible. Use `tabindex='0'` to add it to the focus order. Avoid using positive integers with tabindex to stop any focus order issues

### #4 Don't hide focusable elements

-   dont add `role='presentation` or `aria-hidden=true` to elements that need focus. This will skip the elements and be bad for assistive tech

### #5 Use accessible names for interactive elements

-   make sure interactive elements have accessible names. eg buttons with inner text, labels are used correctly, images have good alt text etc...

## Aria labels

-   use aria labels with things like links so annouce to screen readers more about the link or if it might open a new tab. eg : `<a aria-label="Read more about some awesome article title">Read More</a>`
