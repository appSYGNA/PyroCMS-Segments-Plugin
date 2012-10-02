# PyroCMS Segments Plugin

This is a simple plugin that allows you to check to see if a segment exists in the URI. This is helpful when determining if you should display a link on a certain page. 

## Installation

Copy segments.php to your addons/SITE_REF/plugins or addons/shared_addons/plugins folder.

## Usage

Comma separate all the names of segments inside the tag as a parameter called "names". 

```javascript
{{ segments:exists names="incidents,majors" }}
```

Example use with conditional logic:

```javascript
{{ if { segments:exists names="incidents,majors" } }}
	<a class="btn" href="#" id='togglefilter'><i class="icon-filter"> </i></a>
{{ endif }}
```
