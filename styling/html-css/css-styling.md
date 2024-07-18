## CSS Styling

This also applies to:

- scss & sass
- Any other css preprocessor

### Naming & Declaring CSS Classes

Naming CSS classes can be tricky, we have to be creative in order to find fitting names for out classes. First, lets have a look in our rules:

#### Using Hyphens Instead of Other Characters
```css
/* Do not use these */
.navbarblue {}
.navbar_blue {}

/* Use this */
.navbar-blue {}
```

#### Avoid Id Selectors
```css
/* Do not use this */
#navbar {}

/* Use this */
.navbar{}
```

Now we can see our general **naming** rules:

#### Usage of prefixes

If you are working on a big project, prefixes may help keeping the codebase more readable. These prefixes may vary from modules, packages etc.
```css
.auth-form {}
.congress-form {}
```

#### Meaningless Class Names
Do not declare meaningless class names 
```css
/* Do not use this */
navbar-23-34s {}

/* Use this */
navbar-blue {}
```

### Using Short Attributes

```css
/* Do not use these */
.foo {
	margin-right: 3px;
	margin-left: 3px;
	margin-top: 3px;
	margin-bottom: 3px;
	
	padding-right: 3px;
	padding-left: 3px;
	padding-top: 3px;
	padding-bottom: 3px;
}
/* Instead use this */
.foo {
	margin: 3px;
	padding:3px;
}
```
_This rule also applies for font, ...-...-style, background etc._

#### Usage of 0
When declaring a statement which has 0 as the value, do not use any units. Leave it as is.

```css
/* Do not use this */
.foo {
	margin: 0px;
}
/* Use this */
.foo {
	margin: 0;
}
```

Also use 0 before float values (from -1 to 1)
```css
/* Do not use this */
.foo {
	margin: .9px;
}
/* Use this */
.foo {
	margin: 0.9px;
}
```

### CSS Formatting Rules
Formatting rules are rules that keep the codebase readable and nice.
#### Indentation
The size of indentation is 4 spaces.
```css
/* Do not use this */
.foo {
  margin: 0;
}
/* Use this */
.foo {
    margin: 0;
}
```

#### Key-Value Stops
```css
/* Do not use this */
.foo {
	margin:0;
}
/* Use this */
.foo {
	margin: 0;
}
```

#### Declaration Stops
Please include semicolons at the end of the declaration.
```css
/* Do not use this */
.foo {
	margin: 0;
	padding: 0
}
/* Use this */
.foo {
	margin: 0;
	padding: 0;
}
```

#### Separation of Blocks
```css
/* Do not use these */
.foo
{
	margin: 0;
}
.foo{
	margin: 0;
}
/* Use this */
.foo {
	margin: 0;
}
```

#### Placement of Selectors
```css
/* Do not use this */
a, a:hover, a:active {}

/* Use this */
a,
a:hover,
a:active {}
```

#### Separation of Blocks
```css
/* Do not use this: No blank line */
.foo {
	margin: 0;
}
.bar {
	margin: 0;
}

/* Use this */
.foo {
	margin:0;
}

.bar {
	margin: 0;
}
```

### What Next?

[HTML Styling Guide](https://github.com/octofex/docs/tree/main/styling/html-css/css-styling.md)
