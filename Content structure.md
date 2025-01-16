# Content Structure

-   if using `<section>`, check to see if you need to add a label to imporove assistive tech. eg: `<section aria-label="Introduction to stamp collecting">`. This should annouce the purpose of the section navigation

-   use heading levels correctly

## Page titles

-   use descriptive and front loaded info for the title. Use a description of the current age followed by other info. eg: `<title>Season 3 | Outrageous Pumpkins | The Food Channel</title>`
    -   Search engines typically display only the first 55–60 characters of a page title, so be sure to limit your total page title characters.

## Page language

-   use the 2 letter language codes for the AT coverage. There can only be one lang per html so use the primary language

-   you can use separate languages within html elements. eg: `<p> this is an english paragraph with estonian in the middle <span lang='et'>"Kas sa räägid inglise keelt?"</span> and some english at the end </p>`
    -   this is will help with correct accent and cadence for AT
