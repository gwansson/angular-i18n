This module has been created by merging the work of 2 developers. See bottom of the page for credits.

This module has:
* a service (localize) 
* a filter (i18n)
* a directive (i18n).
So you can use localization in your controllers, models, template, ...

Use it like this in your template (i18n is the filter)
```
{{'Hello World'|i18n}} 
{{"My name is %s and i am %d years old." | i18n:"Max":"98"}} 
```
	
Define your language files in your approot/i18n/, named as the language you are targeting,
ie approot/i18n/en-US.js
The en-US.js file looks like this
```
lang = 
{
    "Hello World" : "Hello World",
    "My name is %s and i am %d years old." : "My name is %s and i am %d years old."
}
```

The fr-FR.js file looks like this
```
lang = 
{
    "Hello World" : "Bonjour Monde",
    "My name is %s and i am %d years old." : "Mon prenom est %s et j'ai %d ans."
}
```
	
**Credits**
* Jenu : marco.mich...@gmail.com 
* Jim Lavin : http://codingsmackdown.tv/blog/2012/12/14/localizing-your-angularjs-app/
