# Colour and contrast

-   Regular text and images of text must have a minimum contrast of `4.5 : 1` to pass WCAG requirements
-   Large text and essential icons must be minimum `3 : 1`

    -   Large text is anything at least 18pt / 24px or 14pt / 18.5px bolded
    -   Logos and decorations don't need to follow these

    -   Lots of tools available to check this stuff for you

-   Don't use colour alone to convery meaning or information

## Media queries

-   You can use media queries to create new/ different colour or contrat themes to help with visual sensitivity.

    -   `@prefers-color-scheme` could be used to make a dark theme

              `@media (prefers-color-scheme: dark) {

        body {
        background: #282828;
        }
        }`

    -   `@prefers-contrast` could be used to make a high or low contrast build

                  `@media (prefers-contrast: more) {

        body {
        background: #333333;
        }
        }`
