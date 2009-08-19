# Human Filesize - Shows the size of a file in human readable format

**Author**: [George Ornbo][]
**Source Code**: [Github][]

## Compatibility

* ExpressionEngine Version 1.6.x
* PHP 5.x

## License

Copyright is free for personal and commercial use. 

If you use it commercially use a donation of $5 is suggested. You can send [donations here](http://pledgie.org/campaigns/2898). 

Copyright is licensed under a [Open Source Initiative - BSD License][] license.

## Installation

This file pi.copyright.php must be placed in the /system/plugins/ folder in your [ExpressionEngine][] installation.

## Name

Copyright

## Synopsis

Shows a copyright notice in ExpressionEngine Templates

## Description

The plugin returns a string for display in ExpressionEngine templates

	{exp:copyright:show}

## Parameters ##

### Start Year ###

	start_year="2009"
	
Sets the start date. Default - current year

### End Year ###

	end_year="2009"
	
Sets the end date. Default - current year

### Delimiter ###

	delimiter=""
	
Sets the delimiter between two years. Default - the "-" symbol (&ndash;)

### Copyright symbol ###

	copyright_symbol=""
	
Sets the copyright symbol. Default - the "©" symbol (&copy;)
	
## Examples

	{exp:copyright:show}
	
Outputs a copyright symbol and current year. e.g. &copy; 2009

	{exp:copyright:show start_year="2007"}
	
Outputs a copyright symbol starting from the start year up to the current year. e.g. &copy; 2007 &ndash; 2009

	{exp:copyright:show start_year="2007" end_year="2014"}

Outputs a copyright symbol starting from the start year up to the given end year. e.g. &copy; 2007 &ndash; 2014	

	{exp:copyright:show copyright_symbol="anything"}

Changes the copyright symbol to anything you set. e.g. anything 2009

	{exp:copyright:show delimiter="&nbsp;to&nbsp;" start_year="2005"}	
	
Changes the delimiter to anything you set. e.g. 2005 to 2009
	
[George Ornbo]: http://shapeshed.com/
[Github]: http://github.com/shapeshed/copyright.ee_addon/
[ExpressionEngine]:http://www.expressionengine.com/index.php?affiliate=shapeshed
[Open Source Initiative - BSD License]: http://opensource.org/licenses/bsd-license.php