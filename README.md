
Notimoo
=======

This plugin provides the web developer with a way to show notification to the users.

![Screenshot](http://www.paquitosoft.com/notimoo/Notimoo-splash.gif)

How to use
----------

Using Notimoo is very easy. It comes with predefined settings that will allow anybody 
to use it just with a couple of lines:

	#JS
	// First of all I create a Notimoo instance with default configuration
	var notimooManager = new Notimoo();
	
	// Showing a simple notification
	notimooManager.show({
		title: 'Testing notification',
		message: 'This is a sample notitication showing how easy is to use Notimoo.'
	});
	
	// Showing a notification that does not disappear using a custom class.
	notimooManager.show({
		title: 'Testing notification',
	    message: 'This notification will not disapper on its own. You must click on it to close.',
	    sticky: true,
	    customClass: 'info'
	});

There is a lot of settings you can customize when creating the manager and some of them can be 
overriden every time you call the show() method.

	#JS
	// Create the manager so notifications are shown in the upper-left corner:
	var notimooManager = new Notimoo({
		locationVtype: 'top',
		locationHType: 'left'
	});
	
	// Show a notification with a custom width and displaying time:
	notificationManager.show({
		title: 'Custom notification',
		message: 'Testing custom width and visible time for this notification',
		width: 200,
		visibleTime: 2500
	});
	
Please, check the documentation web page for more details.

