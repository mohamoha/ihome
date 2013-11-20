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

```js
ID: "table.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/table.css">

````html
<table class="us-table">
    <thead>
        <tr>
            <th>Date</th>
            <th>Transaction Info</th>
            <th>Status</th>
            <th>Gross</th>
            <th></th>
            <th></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>2012.03.15</td>
            <td>
              <div><a href="#">Freight Only Epacket MMP lalabys</a><div>
              <div>201304199322039</div>
            </td>
            <td>Pending</td>
            <td>US $200.00</td>
            <td>
              <div><a href="#">Detial</a><div>
            </td>
            <td>Opertion</td>
        </tr>
        <tr>
            <td>2012.03.15</td>
            <td>
              <div><a href="#">Freight Only Epacket MMP lalabys</a><div>
              <div>201304199322039</div>
            </td>
            <td>Pending</td>
            <td>US $200.00</td>
            <td>
              <div><a href="#">Detial</a><div>
            </td>
            <td>Opertion</td>
        </tr>
        <tr>
            <td>2012.03.15</td>
            <td>
              <div><a href="#">Freight Only Epacket MMP lalabys</a><div>
              <div>201304199322039</div>
            </td>
            <td>Pending</td>
            <td>US $200.00</td>
            <td>
              <div><a href="#">Detial</a><div>
            </td>
            <td>Opertion</td>
        </tr>
        <tr>
            <td>2012.03.15</td>
            <td>
              <div><a href="#">Freight Only Epacket MMP lalabys</a><div>
              <div>201304199322039</div>
            </td>
            <td>Pending</td>
            <td>US $200.00</td>
            <td>
              <div><a href="#">Detial</a><div>
            </td>
            <td>Opertion</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td colspan="6">footer</td>
        </tr>
    </tfoot>
</table>
````

## Switch

## Paging

## Calendar

```js
ID: "calendar.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/calendar.css">

````html
<input id="date-input" type="text" />
````

````js
seajs.use(['arale/calendar/1.0.0/calendar'], function(Calendar) {
  var lang = {
    'Su': 'S',
    'Mo': 'M',
    'Tu': 'T',
    'We': 'W',
    'Th': 'T',
    'Fr': 'F',
    'Sa': 'S',
    'Jan': 'Jan',
    'Feb': 'Feb',
    'Mar': 'Mar',
    'Apr': 'Apr',
    'May': 'May',
    'Jun': 'Jun',
    'Jul': 'Jul',
    'Aug': 'Aug',
    'Sep': 'Sep',
    'Oct': 'Oct',
    'Nov': 'Nov',
    'Dec': 'Dec'
  };
  new Calendar({
    trigger: '#date-input',
    lang: lang
  });
});
````

More usage at: http://aralejs.org/calendar

## Step

```js
ID: "step.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/step.css">

````html
<ol class="us-step us-step-3">
    <li class="us-step-start us-step-done">Email Validation</li>
    <li class="us-step-active">Account Set up</li>
    <li class="us-step-end">Success</li>
</ol>
````

````html
<ol class="us-step us-step-4">
    <li class="us-step-start us-step-done">Validate</li>
    <li class="us-step-done">Something</li>
    <li class="us-step-active">Account Set</li>
    <li class="us-step-end">Success</li>
</ol>
````

````html
<ol class="us-step us-step-5">
    <li class="us-step-start us-step-done">One</li>
    <li class="us-step-done">Two</li>
    <li class="us-step-active">Three</li>
    <li>Four</li>
    <li class="us-step-end">Five</li>
</ol>
````

````html
<ol class="us-step us-step-3 us-step-mini">
    <li class="us-step-start us-step-active">One</li>
    <li>Two</li>
    <li class="us-step-end">Three</li>
</ol>
````

````html
<ol class="us-step us-step-3 us-step-mini">
    <li class="us-step-start us-step-done">One</li>
    <li class="us-step-active">Two</li>
    <li class="us-step-end">Three</li>
</ol>
````

## Select

## Notice

## Radio Card

## Header

## footer

## page layout

## Money

````html
<style>
.us-money {
  font-family: 'Microsoft YaHei',STXihei,MingLiu;
  font-size: 48px;
}
</style>
<span class="us-money">￥<span>
<span class="us-money">$<span>
````
