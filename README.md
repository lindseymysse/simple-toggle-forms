# simple-toggle-forms
Simple HUD menus in CSS. 

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

	Simple Toggle Menus

	Design is about understanding the affordances of the medium you are working in. 
	That is to say: you have to understand how it breaks. Once you understand how
	something breaks you can design around the slip. When you understand what the 
	user cannot do, you can make sure they only use whatever you are designing
	in a certain way.

	Anyway, in my raging egotistical opinion, this is currently the best way to do 
	menus in HTML, CSS and JS. 

  the variables for this menu look like this:

``` CSS

:root {
  --menu-tag-size: 2em;
  --left-menu-width: calc(100vw - var(--menu-tag-size) - 3em);
  --right-menu-width: calc(100vw - var(--menu-tag-size) - 3em);
  --bottom-menu-height: calc(90vh - var(--menu-tag-size) - 3.75em);
}
```

``` HTML

  Implement the Toggle Menus like this:

  <div id="left-menu" class="left-menu menu">
    <input type="checkbox" name="open" class="left-menu-tag menu-tag" checked/>
    <div id="left-menu-content" class="left-menu-form menu-body"></div>
  </div>

  <div id="right-menu" class="right-menu menu">
    <input type="checkbox" name="menu-tag" class="right-menu-tag menu-tag" checked/>
    <div id="right-menu-content" class="right-menu-form menu-body" accept-charset="utf-8">
    </div>
  </div>

  <div id="bottom-menu" class="bottom-menu menu">
    <input id="bottom-menu-checkbox" type="checkbox" name="menu-tag" class="bottom-menu-tag menu-tag" checked />
    <div id="bottom-menu-content" class="menu-body bottom-menu-form" accept-charset="utf-8">
    </div>
  </div> 

```
LNSY 