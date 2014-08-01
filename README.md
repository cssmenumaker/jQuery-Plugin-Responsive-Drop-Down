#Responsive Dropdown Menu Plugin

A small jQuery plugin which allows you to create toggle and multi-toggle menus for mobile devices.

##Usage

The plugin is very easy to use. First, create the markup (an unordered list of links contained by a `div`)

```
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
```
<link rel="stylesheet" type="text/css" href="css/responsivemenu.css">
```
Link the jQuery script:
```
<script type="text/javascript" src="js/cssmenumaker.js"></script>
```
And finally, initialize the plugin:
```
<script type="text/javascript">
	$("#cssmenu").menumaker();
</script>
```
##Options
```
$("#cssmenu").menumaker({
	title: "Menu",              // The text of the button which toggles the menu
	format: "multitoggle"       // It takes two values: dropdown for a simple toggle menu and multitoggle for a menu where each submenu can be toggle separately
});
```