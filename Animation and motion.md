# Animation and motion

-   Over 30% of aldunts have experienced vestibular issues.

## Flashing and moving content

https://www.w3.org/TR/WCAG22/#three-flashes-or-below-threshold

-   Any flashing should not occur more than 3 times in 1 second.
-   All flashing and animations should be able to be disabled unless it is essential to the functionality or information of the page.
-   Any flashes should also be below the [red and green flash threshold.](https://www.w3.org/TR/WCAG22/#dfn-general-flash-and-red-flash-thresholds)

-   Consider not having any movement (even micro movement) at all unless it is essential to the function of the page.
-   If you think the movement is essential, follow the [WCAG guidelines on motion](https://www.w3.org/WAI/WCAG21/Understanding/pause-stop-hide.html)

## Pause/ Stop/ Hide movement

-   You can use a button to toggle animations on the page so stop them.
-   You can use media-queries with `@prefers-reduced-motion` which will automatically toggle the movements off if they have the setting active through the OS

-   Any animation should be used cautiously. Ideally a user hsould be able ot control the animation with a pause and play button. Generally better to not have animations if possible

**some OS' require opt in while some require opt out, be careful relying only on @prefers-reduced-motion**

-   You can se multiple medai queries to give more choices, eg: `@prefers-color-scheme`, `@prefers-contrast`, and `@prefers-reduced-motion`
