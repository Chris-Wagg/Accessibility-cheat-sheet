# Custom Errors

-   ideally it is best to leave default errors for things, these will not mess with screen readers

-   if using a custom error, attach the error to the input using `aria-describedby` and an `ID` attached to the message. Use `role='alert` and `aria-live` to make sure the error is announced by the screen reader

eg:

```
<input
	aria-required
	required
	type='text'
    ...
	aria-describedby='email-error'
/>

		<div
			id='error'
			role='alert'
			aria-live='polite'
			>
			*ERROR MESSAGE IS HERE*
		</div>

```
