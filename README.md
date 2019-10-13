# HScroll CSS

A dead simple CSS file to create INFINITE HORIZONTAL TEXT SCROLLING 🤙

## Example

_(You have access to examples in this repo)_

## Requirements

For the **wrapper** you need to specify a fixed **width** in CSS and an overflow **hidden**

```html
<div class="hscroll-wrapper"></div>
```

For the inner text you need to create two instances with the same content like this :

```html
<div class="hscroll-wrapper">
	<div class="hscroll">HSCROLL - HSCROLL - HSCROLL -&nbsp;</div>
	<div class="hscroll">HSCROLL - HSCROLL - HSCROLL -&nbsp;</div>
</div>
```

The minimal require CSS code :

_Note that the animation property need to be linear and infinite 👍_

```css
.hscroll-wrapper {
	height: fit-content;
	width: 100vw;
	overflow: hidden;
	white-space: nowrap;
}
.hscroll {
	display: inline-block;
	font-size: 200px;
	font-weight: 900;
	animation: hscrollTranslate 10s linear infinite;
	border: 1px solid green;
}

@keyframes hscrollTranslate {
	100% {
		transform: translateX(-100%);
	}
}
```

> ## **TO-DO FUTURE UPDATES :**

- [ ] JS Version
