# App Store Badge in CSS

Since every HTTP request adds latency (particularly when using a phone over cell networks), I wondered if it was possible to create a reasonable clone of official Apple App Store badge in pure CSS.

[View the demo page](http://xinsight.github.io/AppStoreBadge/test.html)

<p align="center">
  <img src="https://raw.github.com/xinsight/AppStoreBadge/master/example.png">
</p>

## Usage

```
<link rel="stylesheet" href="style.css" />

<div class="appstorebadge">
	<div class="text">
    	<div class="line1">Available on the</div>
    	<div class="line2">App Store</div>
	</div>
    <div class="iphone">
	    <div class="earpiece"></div>
	    <div class="screen"></div>
	    <div class="button"></div>
    </div>
</div>
```

<style type="text/css" media="screen" href="https://raw.github.com/xinsight/AppStoreBadge/master/style.css"></style>

<div class="appstorebadge">
	<div class="text">
    	<div class="line1">Available on the</div>
    	<div class="line2">App Store</div>
	</div>
    <div class="iphone">
	    <div class="earpiece"></div>
	    <div class="screen"></div>
	    <div class="button"></div>
    </div>
</div>


To increase the size of the badge, use the `zoom` attribute.

```
<div class="appstorebadge" style="zoom: 200%">...</div>
<!-- or -->
<div class="appstorebadge zoom2">...</div>	
```

There are also `zoom2` and `zoom3` classes which work better on Firefox.

Add the `grey` class for the grey version.

```
<div class="appstorebadge grey">...</div>	
```

Add the `white` class for the white version.

```
<div class="appstorebadge white">...</div>	
```

## Bugs, Limtations

`zoom2` and `zoom3` classes work in Firefox, but the height of the element doesn't change.

