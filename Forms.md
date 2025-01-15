use native HTML controls and behaviour

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

## Form instructions

-   use aria-describedby to provide extra form instructions. This will read the extra information from the <p> after it has read the initial info about the element

```
<label for="username">Username</label>
<input type="text" id="username" name="username" aria-describedby="username-instructions" required>
<p id="username-instructions">Choose a unique username between 4 and 20 characters.</p>
```

## Autocomplete

-   Allow autocomplete. Most web browsers will recognise which info to autofill here based on the type and name of the input

-   If not, you can include `autocomplete='name'` for example to indicate the behaviour

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
