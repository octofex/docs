## HTML Styling

This also applies to:

- JSX
- Any HTML Embed language
- Vue
- Angular
- Blade (Laravel)
- ...

### Starting HTML Files

Every html file should have the following HTML Template:

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8">
		<meta http-equiv="X-UA-Compatible" content="IE=edge">
		<meta name="viewport" content="width=device-width, initial-scale=1.0">

		<title>TITLE_OF_THE_PAGE</title>
	</head>
	<body>

	</body>
</html>
```

Yes, this is the Emmet starting template. We strongly recommend everyone to use Emmet extension to edit HTML and it's variants.

The organizing of the head element is important it should be like:

```html
<head>
	<meta charset="UTF-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	
	<meta name="description" content="Lorem ipsum dolor, sit amet consectetur.">
	<meta name="keywords" content="lorem, ipsumi dolor, sit">
	<meta name="author" content="Octofex">

	<link rel="icon" href="favicon.ico">

	<link rel="stylesheet" href="style1.css">
	<link rel="stylesheet" href="style2.css">
	
	<title>TITLE_OF_THE_PAGE</title>
</head>
```
Order:
- Meta Tags
- Meta SEO Tags
- Favicon
- Stylesheets
- Titles

If scripts are used in the file it can be added at the end of the file, before `html <body> `.

### Class Names

Class names is a very easy topic to understand. Basically, spaces should be replaced with dashes and all text should be lowercase.

#### Examples:
```html
<p class="text-center color-red error-text"> This service is currently unavailable </p>
```

### Id's

Id's and names are a little bit different from class names. They should be named with camel case format. The only exception is multiple id's under the same logic should have a tagname.

#### Examples:
```html
<input id="thisIsAInput" type="text">

<div id="menuDiv">
	<button id="menuTrigger"></button>
</div>
```

### Names

Name attribute should be in camel case. There is no extra exceptions.


### Naming Elements and Attributes
	
Every tag and attribute should be in lower case.

```html
<!-- Don't use this -->
<P CLASS="..."> </P>

<!-- Use this -->
<p class="..."> <p>
```

### Spacing

The accepted indent size is 4 spaces.

```html
<ul>
    <li>Item 1</li>
	<li>Item 2</li>
</ul>
```
### Attribute Overflow

Elements sometimes can get very long because of attributes. Instead of righting a big components with lots of attributes, you can add new lines after attributes.

```html
<!-- Don't use this -->
<input class="input-text input-rounded" id="importantInput" align="center" type="text" name="importantInput"></input>

<!-- Use this -->
<input 
 class="input-text input-rounded"
 id="importantInput"
 align="center"
 type="text"
 name="importantInput"></input>
```

### General Spacing

Please use new lines and tabs while creating new elements.

```html
<!-- Don't use this -->
<div><ul>
<li>Item 1</li>
</ul></div>

<p>lorem ipsum sit dolor amet</p>

<!-- Use this -->
<div>
    <ul>
	<li>Item 1</li>
        <li>Item 2</li>
    </ul>
</div>

<p>
	lorem ipsum sit dolor amet
</p>
```

### What Next?
[CSS Styling Guide](https://github.com/octofex/docs/tree/main/styling/css-styling.md)

