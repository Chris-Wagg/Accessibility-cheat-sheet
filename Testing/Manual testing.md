# Manual Testing

**_Pros_**

-   Straightfoward and quick to run
-   Catches more issues then automated testing
-   Fewer tools and expertise needed

**_Cons_**

-   More complex and time consuming
-   Difficult to repeat at scale
-   Sometimes requires greater expertise to run test and interpret results

### Can be automated

-   Color contrast of text on solid backgrounds
-   Image alternative text exists
-   Headings, lists, and landmarks exist
-   ARIA is present
-   Identifying keyboard-focusable elements
-   iFrame title detection
-   Video element is present

### Can't be automated

-   Color contrast of text on gradients/images
-   Image alternative text is accurate and is properly assigned
-   Headings, lists, and landmarks are correctly marked-up and all elements are accounted for
-   ARIA is being used appropriately and applied to the correct element(s)
-   Which elements are missing keyboard focus, the focus order makes logical sense, and the focus indicator is visible
-   iFrame, the focus order makes logical sense, and the focus indicator is visible
-   Video element has appropriate alternative media present (such as captions and transcripts)

## Types of manual testing

-   3 big focuses
    1. keyboard functionality
    2. visually-focused reviews
    3. general content checks

[Check out the IBM accessibility manual for a checklist to start testing](https://www.ibm.com/able/toolkit/verify/manual/)

### Keyboard checks

-   Answers questions such as...
    -   Does the web page or feature require a mouse to function?
    -   Is the tabbing order logical and intuitive?
    -   Is the keyboard focus indicator always visible?
    -   Can you get stuck in an element that shouldn't trap focus?
    -   Can you navigate behind or around an element that should be trapping focus?
    -   When closing an element that received focus, did the focus indicator return to a logical place?

### Visual checks

-   Make sue to check zoom/ magnification levels

Visual check can tell us...

-   Are there color contrast issues that an automated tool couldn't pick up, such as text on top of a gradient or image?
-   Are there any elements that look like headings, lists, and other structural elements but are not coded as such?
-   Are navigation links and form inputs consistent throughout the website or app?
-   Is there any flashing, strobing, or animation that exceeds the recommendations?
-   Does the content have proper spacing? For letters, words, lines, and paragraphs?
-   Can you see all the content using a screen magnifier or browser zoom?

### Content checks

-   Make sure to actually check the content of the page to make sure it is logical and makes sense

Content checks can tell us...

-   Are page titles, headings, and form labels clear and descriptive?
-   Are image alternatives concise, accurate, and useful?
-   Is color alone used as the only way of conveying meaning or information?
-   Are links descriptive or do you use generic text such as "read more" or "click here"?
-   Are there any changes to the language within a page?
-   Is plain language used and are all acronyms spelled out when first referenced?
