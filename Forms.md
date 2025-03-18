# Forms

-   All the previous factors such as content structure, keyboard focus, colour contrast etc apply to forms.

## Fields

-   Use native HTML controls and behaviour, this is easier than building cutom aria into things.

-   Forms should not auto-submit on field changes or when they gain focus

## Labels

-   Must be present and visible at all times
-   relationship between form and field should be clear and accurate

## Descriptions

-   field descriptions are not required for accessibility if labels or form instructions are descriptive enough
-   Good to add field descriptions in some cases to avoid errors in the form. Eg explaining the input order for a date YYYY/MM/DD
-   One of the best methods for descriptions in to add `aria-labelledby` as well as a `<label>`, screen readers will read both
-   If you add the aria-labelledby attribute to your element, the attribute value overrides the text within your `<label>`. As always, be sure to test the final code with all of the ATs you plan to support.

## Errors

-   Make errors known, clearly identify which field has the error and make sure the error is described to the user in text

-   Different ways to include errors

    -   A modal, inline near where the error occured
    -   A collection of errors, grouped in a larger message at the top of the page
    -   [check here for more](https://webaim.org/techniques/formvalidation/#error)

-   Pay attention to keyboard focus and live regions when announcing errors
-   Offer details to fix the erro where possible

    -   Use `required` attribute on the field, but the error will be generic
    -   `aria-required` can share custom error messages to AT's. Only the AT's will get the message though, you will need to add more custom code to show these errors to other users

    -   Make sure users get another try at submitting the fixed form and provide feedback. Error messages say if updates need to be made, success messages confirms everything is all good.

## Inputs and grouped inputs

-   Always pair an input with a label

```
<label for="email">Email</label>
<input type="email" id="email" name="email">
```

-   Placeholders should be used to show examples of what the input expecets, not used as a label

-   Wrap multiple inputs in a fieldset with a legend

```
<fieldset>
  <legend>Choose your favorite color</legend>
  <input type="radio" id="red" name="color" value="red">
  <label for="red">Red</label>
  <input type="radio" id="blue" name="color" value="blue">
  <label for="blue">Blue</label>
  <input type="radio" id="green" name="color" value="green">
  <label for="green">Green</label>
</fieldset>
```

-   Related form fields should be grouped programmatically and visually, use field sets to do this

## Form instructions

-   use aria-describedby to provide extra form instructions. This will read the extra information from the `<p>` after it has read the initial info about the element

```
<label for="username">Username</label>
<input type="text" id="username" name="username" aria-describedby="username-instructions" required>
<p id="username-instructions">Choose a unique username between 4 and 20 characters.</p>
```

## Autocomplete

-   Allow autocomplete. Most web browsers will recognise which info to autofill here based on the type and name of the input
-   If not, you can include `autocomplete='name'` for example to indicate the behaviour
-   Autocomplete should be inculded where possible to help with definition or identification of pourpose of the form to AT's

## Focus

-   Most browsers will have default focuses for elements, try not to mess with these.
-   If anything you can try to enhance them (eg: make boarders bolder) but it's bad practice to remove them

## Required fields

-   use the required attribute in the input tag
-   to indicate to users use something like an asterisk or put required in the label

```
<label for="email">Email (required)</label>
<input type="email" id="email" name="email" required>
```
