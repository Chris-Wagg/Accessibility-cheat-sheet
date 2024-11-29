# Visually hidden elements

```
clip: rect(1px, 1px, 1px, 1px);
	clip-path: inset(50%);
	height: 1px;
	width: 1px;
	margin: -1px;
	overflow: hidden;
	padding: 0;
	position: absolute;
```

-   this is the most modern way to hide content

-   using `visibility: hidden` or `display:none` will remove the element from the DOM tree and hide it from screen readers
-   using `opacity:0` is also not best practice
