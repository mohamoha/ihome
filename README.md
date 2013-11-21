# ihome

---

DPL page for `alipay.us`. We choose `us-` for class prefix.

- [Button](#button)
- [Input](#input)
- [Tab](#tab)
- [Dropdown](#dropdown)
- [Filter](#filter)
- [Table](#table)
- [Switch](#switch)
- [Paging](#paging)
- [Calendar](#calendar)
- [Step](#step)
- [Select](#select)
- [Notice](#notice)
- [Radio Card](#radio-card)
- [Page Layout](#page-layout)
- [Money](#money)

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

For some JavaScript code, you should just copy it to your projects.

<style>
.nico-insert-code {
  background: #F5F4E9;
  padding: 20px;
  font: 16px/1.5 tahoma, Verdana, arial, sans-serif;
  color: #908a80;
}
.nico-insert-code a {
  color: #2d93b4;
  text-decoration: none;
}
.nico-insert-code a:hover {
  color: #3DDEF5;
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
<button class="us-button us-button-primary">Search</button>
<button class="us-button us-button-primary us-button-middle">Search</button>
<button class="us-button us-button-primary us-button-small">Search</button>
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
  <input type="text" class="us-input" size="26">
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

## Filter

```js
ID: "filter.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/filter.css">

````html
<ul class="us-filter">
  <li class="us-filter-item us-filter-item-selected">
    <a href="javascript:;">All</a>
  </li>
  <li class="us-filter-item">
    <a href="javascript:;">Pending</a>
  </li>
  <li class="us-filter-item">
    <a href="javascript:;">In progress</a>
  </li>
  <li class="us-filter-item">
    <a href="javascript:;">Completed</a>
  </li>
</ul>
````

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

```js
ID: "switch.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/switch.css">

````html
<div class="us-switch us-switch-left">
  <span class="us-switch-dot">●</span>
</div>
````

````html
<div class="us-switch us-switch-right">
  <span class="us-switch-dot">●</span>
</div>
````

````js
seajs.use('$', function($) {
  $('.us-switch').click(function() {
    var item = $(this);
    if (item.hasClass('us-switch-left')) {
      item.removeClass('us-switch-left').addClass('us-switch-right');
    } else {
      item.removeClass('us-switch-right').addClass('us-switch-left');
    }
  });
});
````

## Paging

```js
ID: "paging.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/paging.css">

````html
<div class="us-paging">
  <a href="javascript:;" class="us-paging-disabled">« Home</a>
  <a href="javascript:;" class="us-paging-disabled">‹ Previous</a>
  <span class="us-paging-begin">1</span>-<span class="us-paging-end">10</span>
  Items, Totally <span class="us-paging-count">100</span> Items
  <a href="javascript:;">Next ›</a>
  <a href="javascript:;">End »</a>
</div>
````

## Calendar

```js
ID: "calendar.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/calendar.css">

````html
<div style="background:#ECEAD8;padding:20px">
  <div class="us-calendar">
    <input value="2013-11-16" id="date-input" size="12" type="text" />
  </div>
</div>
````

````js
seajs.use(['$', 'arale/calendar/1.0.0/calendar', 'arale/calendar/1.0.0/i18n/en'], function($, Calendar, lang) {
  var cal = new Calendar({
    trigger: '#date-input',
    lang: lang
  });
  cal.on('show', function() {
    $(this.get('trigger')).parent().addClass('us-calendar-focus');
  }).on('hide', function() {
    $(this.get('trigger')).parent().removeClass('us-calendar-focus');
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

```js
ID: "select.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/select.css">

````html
<select id="country" name="country">
    <option value="value1">Brazil</option>
    <option value="value2">China</option>
    <option value="value2">Germany</option>
</select>
````

````js
seajs.use(['arale/select/0.9.7/select'], function(Select) {
    var sel = new Select({
        trigger: '#country',
        triggerTpl: '<a href="#"><span data-role="trigger-content"></span><i class="ui-select-arrow">∟</i></a>',
        width: 250
    }).render();

    sel.before('show', function() {
      this.get('trigger').addClass('ui-select-trigger-focus');
    });

    sel.after('hide', function() {
      this.get('trigger').removeClass('ui-select-trigger-focus');
    });

    sel.on('change', function(target, prev) {
      console.log(target.html());
    });
});
````

More usage at: http://aralejs.org/select

## Notice

```js
ID: "notice.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/notice.css">

````html
<div class="us-notice">
  <span class="us-notice-icon">i</span>
  Some infomatioin in us-notice. Some infomatioin in us-notice.
</div>
````

## Radio Card

```js
ID: "radiocard.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/radiocard.css">

````html
<ul class="us-radiocard">
  <li class="us-radiocard-item">
    <div class="us-radiocard-item-left">
      <span class="us-radiocard-radio">●</span>
      <span class="us-radiocard-item-icon">
        <i class="iconfont" title="日历/日期">&#xF01C;</i>
      </span>
    </div>
    <span class="us-radiocard-item-text">Webmoney</span>
    <span class="us-radiocard-item-text us-money">$</span>
  </li>
  <li class="us-radiocard-item">
    <div class="us-radiocard-item-left">
      <span class="us-radiocard-radio">●</span>
      <span class="us-radiocard-item-icon">
        <i class="iconfont" title="日历/日期">&#xF01C;</i>
      </span>
    </div>
    <span class="us-radiocard-item-text">Webmoney</span>
    <span class="us-radiocard-item-text us-money">¥</span>
  </li>
  <li class="us-radiocard-item us-radiocard-item-selected">
    <div class="us-radiocard-item-left">
      <span class="us-radiocard-radio">●</span>
      <span class="us-radiocard-item-icon">
        <i class="iconfont" title="日历/日期">&#xF01C;</i>
      </span>
    </div>
    <span class="us-radiocard-item-text">Webmoney</span>
    <span class="us-radiocard-item-text us-money">¥</span>
  </li>
</ul>
````

````js
seajs.use(['$'], function($) {
  $('.us-radiocard-item').click(function() {
    $('.us-radiocard-item').removeClass('us-radiocard-item-selected');
    $(this).addClass('us-radiocard-item-selected');

    // For IE8 reflow problem
    $('.us-radiocard-item-left').each(function(index, item) {
      item.innerHTML += '';
    });
  });
});
````

## Page Layout

## Money

````html
<style>
.us-money {
  font-family: Arial;
  font-size: 44px;
}
</style>
<span class="us-money">¥<span>
<span class="us-money">$<span>
````
