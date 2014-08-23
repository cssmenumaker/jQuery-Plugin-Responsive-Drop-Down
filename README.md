#Responsive Dropdown Menu Plugin

A small jQuery plugin which allows you to create various types of menus for mobile devices. You can create a menu which can be toggled with a tap on mobile devices, a menu where the menu and the submenus can be toggled or a select list menu.

##Usage

The plugin is very easy to use. First, create the markup (an unordered list of links contained by a `div`)

```html
<div id="cssmenu">
  <ul>
    <li><a href="">Item</a></li>
    <li><a href="">Item</a></li>
    <li><a href="">Item</a></li>
    <li><a href="">Item</a></li>
  </ul>
</div>
```

Of course, you can create submenus by nesting lists. Next, include the CSS file:
```html
<link rel="stylesheet" type="text/css" href="css/responsivemenu.css">
```
Link the jQuery script:
```html
<script type="text/javascript" src="js/cssmenumaker.js"></script>
```
And finally, initialize the plugin:
```html
<script type="text/javascript">
	$("#cssmenu").menumaker();
</script>
```
##Options
```javascript
$("#cssmenu").menumaker({
	title: "Menu",              // The text of the button which toggles the menu
	format: "multitoggle"       // It takes three values: dropdown for a simple toggle menu, select for select list menu, multitoggle for a menu where each submenu can be toggled separately
});
```