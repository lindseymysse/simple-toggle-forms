``` code
*** begin ascii art ***
 __           __        ___
/__` |  |\/| |__) |    |__
.__/ |  |  | |    |___ |___

___  __   __   __        ___
 |  /  \ / _` / _` |    |__
 |  \__/ \__> \__> |___ |___

       ___            __
 |\/| |__  |\ | |  | /__`
 |  | |___ | \| \__/ .__/

*** end ascii art ***

```


Design is about understanding the affordances of the medium you are working in. 
That is to say: you have to understand how it breaks to make something truly 
useful. 

When you understand what the user cannot do, you can make sure they use 
whatever you are designing in a certain way.

Anyway, in my raging egotistical opinion, this is currently the best way to do 
menus in HTML, CSS and JS. 


## To Use

Include the simple-toggle-menu.css in your html.

``` html 
<link rel="stylesheet" type="text/css" href="/simple-toggle-menu.css">
```

Adjust the variables for this menu with the following variables:

``` CSS

:root {
  --menu-tag-size: 2em;
  --left-menu-width: calc(100vw - var(--menu-tag-size) - 3em);
  --right-menu-width: calc(100vw - var(--menu-tag-size) - 3em);
  --bottom-menu-height: calc(90vh - var(--menu-tag-size) - 3.75em);
  --menu-bg-color: rgba(0,0,0,0.8);

}
```

Implement the Toggle Menus like this:


``` html


<div id="left-menu" class="left-menu menu">
  <input type="checkbox" name="open" class="left-menu-tag menu-tag" checked/>
  <div id="left-menu-content" class="left-menu-form menu-body">

  	<!-- Put your menu content here -->

  </div>
</div>

<div id="right-menu" class="right-menu menu">
  <input type="checkbox" name="menu-tag" class="right-menu-tag menu-tag" checked/>
  <div id="right-menu-content" class="right-menu-form menu-body" accept-charset="utf-8">

    	<!-- Put your menu content here -->

  </div>
</div>

<div id="bottom-menu" class="bottom-menu menu">
  <input id="bottom-menu-checkbox" type="checkbox" name="menu-tag" class="bottom-menu-tag menu-tag" checked />
  <div id="bottom-menu-content" class="menu-body bottom-menu-form" accept-charset="utf-8">

    	<!-- Put your menu content here -->

  </div>
</div> 

```
LNSY 