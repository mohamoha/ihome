# ihome

---

DPL page for `alipay.us`. We choose `us-` for class prefix. It is compatible with normal browsers and `IE8+`.

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
- [Radio](#radio)
- [Channel](#channel)
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
  overflow: auto;
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

````html
<a class="us-button us-button-border">(46s) resend an email</a>
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

```js
ID: "dropdown.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/layout.css">
<link type="text/css" rel="stylesheet" media="screen" href="src/dropdown.css">

````html
<div class="us-header">
  <div class="container-990" id="triggers">
    <a class="us-header-item" href="javascript:;">trigger</a>
    <a class="us-header-item" href="javascript:;">long trigger</a>
  </div>
</div>
````

````html
<ul class="us-dropdown fn-hide" id="dropdown-menu">
  <li class="us-dropdown-item"><a href="javascript:;">Option 01</a></li>
  <li class="us-dropdown-item"><a href="javascript:;">Option 02</a></li>
  <li class="us-dropdown-item"><a href="javascript:;">Option 03</a></li>
</ul>
````

````js
seajs.use('arale/popup/1.1.5/popup', function(Popup) {
  var popup = new Popup({
    trigger: '#triggers .us-header-item',
    element: '#dropdown-menu',
    effect: 'slide fade',
    duration: 200
  });
  popup.before('show', function() {
    this.get('trigger').removeClass('us-dropdown-focus');
    this.activeTrigger.addClass('us-dropdown-focus');
  }).after('hide', function() {
    this.get('trigger').removeClass('us-dropdown-focus');
  });
});
````

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
        <div><a href="#">Freight Only Epacket MMP lalabys</a></div>
        <div>201304199322039</div>
      </td>
      <td>Pending</td>
      <td>US $200.00</td>
      <td>
        <a href="#">Detial</a>
      </td>
      <td>Opertion</td>
    </tr>
    <tr>
      <td>2012.03.15</td>
      <td>
        <div><a href="#">Freight Only Epacket MMP lalabys</a></div>
        <div>201304199322039</div>
      </td>
      <td>Pending</td>
      <td>US $200.00</td>
      <td>
        <a href="#">Detial</a>
      </td>
      <td>Opertion</td>
    </tr>
    <tr>
      <td>2012.03.15</td>
      <td>
        <div><a href="#">Freight Only Epacket MMP lalabys</a></div>
        <div>201304199322039</div>
      </td>
      <td>Pending</td>
      <td>US $200.00</td>
      <td>
        <a href="#">Detial</a>
      </td>
      <td>Opertion</td>
    </tr>
    <tr>
      <td>2012.03.15</td>
      <td>
        <div><a href="#">Freight Only Epacket MMP lalabys</a></div>
        <div>201304199322039</div>
      </td>
      <td>Pending</td>
      <td>US $200.00</td>
      <td>
        <a href="#">Detial</a>
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
  <span class="us-switch-dot" unselectable="on">●</span>
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

<link type="text/css" rel="stylesheet" media="screen" href="src/radio.css">

````html
<span class="us-radio">●</span>
<span class="us-radio us-radio-selected">●</span>
````

## Channel

```js
ID: "channel.css"
```

<link type="text/css" rel="stylesheet" media="screen" href="src/channel.css">

````html
<ul class="us-channel">
  <li class="us-channel-item">
    <div class="us-channel-item-header">
      <div class="us-channel-item-left">
        <span class="us-radio">●</span>
        <span class="us-channel-item-icon">
          <i class="iconfont" title="日历/日期">&#xF01C;</i>
        </span>
      </div>
      <span class="us-channel-item-text">Webmoney</span>
      <span class="us-channel-item-text us-money">$</span>
    </div>
    <div class="us-channel-item-box">
    </div>
  </li>
  <li class="us-channel-item">
    <div class="us-channel-item-header">
      <div class="us-channel-item-left">
        <span class="us-radio">●</span>
        <span class="us-channel-item-icon">
          <i class="iconfont" title="日历/日期">&#xF01C;</i>
        </span>
      </div>
      <span class="us-channel-item-text">Webmoney</span>
      <span class="us-channel-item-text us-money">¥</span>
    </div>
    <div class="us-channel-item-box">
    </div>
  </li>
  <li class="us-channel-item us-channel-item-selected">
    <div class="us-channel-item-header">
      <div class="us-channel-item-left">
        <span class="us-radio">●</span>
        <span class="us-channel-item-icon">
          <i class="iconfont" title="日历/日期">&#xF01C;</i>
        </span>
      </div>
      <span class="us-channel-item-text">Webmoney</span>
      <span class="us-channel-item-text us-money">¥</span>
    </div>
    <div class="us-channel-item-box">
    </div>
  </li>
</ul>
````

````js
seajs.use(['$'], function($) {
  $('.us-channel-item').click(function() {
    $('.us-channel-item').removeClass('us-channel-item-selected');
    $(this).addClass('us-channel-item-selected');

    // For IE8 reflow problem
    $('.us-channel-item-left').each(function(index, item) {
      item.innerHTML += '';
    });
  });
});
````

## Page Layout

````iframe:400
<link type="text/css" rel="stylesheet" media="screen" href="src/index.css">

<div class="us-header">
  <div class="container-990">
    <div class="us-header-right">
      <a class="us-header-item us-header-name" href="javascript:;">Hello, Sheldon Smith</a>
      <a class="us-header-item" href="javascript:;">Settings</a>
      <a class="us-header-item" href="javascript:;">Sign Out</a>
      <a class="us-header-item" href="javascript:;">Help Center</a>
      <a class="us-header-item" href="javascript:;">English</a>
    </div>
  </div>
</div>
<div class="container-990" style="height:400px;background:#f6f6f6;margin-top:20px;margin-bottom:20px;line-height:400px;text-align:center;">
  Content
</div>
<div class="us-footer">
  <div class="container-990">
    <p>Copyright 2003 - 2013 ® Alipay. All rights reserved.</p>
    <p>
      <a href="#">About Alipay</a> |
      <a href="#">Aliexpress</a> |
      <a href="#">Alibaba</a> |
      <a href="#">Jobs</a> |
      <a href="#">International Bussiness</a>
    </p>
  </div>
</div>
````

## Money

````html
<style>
.us-money {
  font-family: Arial;
  font-size: 44px;
}
</style>
<span class="us-money">¥</span>
<span class="us-money">$</span>
````
