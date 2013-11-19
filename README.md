# ihome

---

DPL page for `alipay.us`. We choose `us-` for class prefix.

---

## Usage

The style module ID can be found at left sidebar, you can import them by adding aliases to your package.json:

```js
"spm": {
  "alias": {
   "index": "alice/ihome/1.0.0/index.css"
  }
}
```

And @import the alias name in your css file: `@import url("index");`.

Or add modules you want:

```js
"spm": {
  "alias": {
    "button": "alice/ihome/1.0.0/button.css",
    "step": "alice/ihome/1.0.0/step.css"
  }
}
```

<style>
.nico-insert-code {
  background: #F5F4E9;
  padding: 20px;
  font: 16px/1.5 tahoma, Verdana, arial, sans-serif;
  color: #908a80;
}
</style>

## Button

```js
ID: "button.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/button.css">

````html
<a class="us-button us-button-primary">Continue</a>
<a class="us-button us-button-primary us-button-middle">Continue</a>
<a class="us-button us-button-primary us-button-small">Continue</a>
````

````html
<a class="us-button us-button-info">Search</a>
<a class="us-button us-button-info us-button-middle">Search</a>
<a class="us-button us-button-info us-button-small">Search</a>
````

## Input

```js
ID: "input.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/input.css">

````html
<label class="us-label">
  <span>Label</span>
  <input type="text" class="us-input">
</label>
````

## Tab

```js
ID: "tab.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/tab.css">

````html
<ul class="us-tab">
  <li class="us-tab-item us-tab-item-current">
    <a href="javascript:;">Transaction Records</a>
  </li>
  <li class="us-tab-item">
    <a href="javascript:;">Adjustment Records</a>
  </li>
</ul>
````

````html
<ul class="us-tab">
  <li class="us-tab-item">
    <a href="javascript:;">Transaction Records</a>
  </li>
  <li class="us-tab-item us-tab-item-current">
    <a href="javascript:;">Adjustment Records</a>
  </li>
</ul>
````

## Dropdown

## Table

## Switch

## Paging

## Calendar

## Step

## Select

## Notice

## Radio Card

## Header

## footer

## page layout

