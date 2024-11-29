# Radio groups

-   radio groups best practice is to have the contained within a fielset with a legend.
-   if you want only one radio to be selected out of a group, the name attribute of all the related radios must be the same

```
<div>
	<input
		required
		type='radio'
		name='rating'
		value='1'
		onChange={handleChange}
		/>
		<label htmlFor='rating-1'>
			1
		</label>
</div>
```

-   you can use an onchange to manage a state change such as changing the value of the state to the value of the selected radio
