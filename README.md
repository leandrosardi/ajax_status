# Ajax_Status
The **Ajax_Status** Little JavaScript module to show the status of an AJAX request in the HTML page.

You can find a [live example](https://expandedventure.com/ajax_status/index.html) of **Ajax_Status** here: [https://expandedventure.com/ajax_status/index.html](https://expandedventure.com/ajax_status/index.html)


# Getting Started
Get started in 3 simple steps.

1. Download the required libraries and stylesheets.
All these files are included in this project. You can download them from this page.

2. Include them in the <header> section of your HTML page.

```html
<script src="./javascripts/jquery-3.5.1.min.js" type="text/javascript"></script>
<script src="./javascripts/1.3.0/adminflare-demo-init.min.js" type="text/javascript"></script>
<link href="https://fonts.googleapis.com/css?family=Open+Sans:300italic,400italic,600italic,700italic,400,300,600,700" rel="stylesheet" type="text/css">	
<link href="./css/1.3.0/black-blue/bootstrap.min.css" media="all" rel="stylesheet" type="text/css" id="bootstrap-css">
<link href="./css/1.3.0/black-blue/adminflare.min.css" media="all" rel="stylesheet" type="text/css" id="adminflare-css">
	
<link rel="stylesheet" href="./ajax_status.css">
<script src="./ajax_status.min.js" type="text/javascript"></script>
```

3. Create a nice prefilled form.

```html
<div id='myAjaxForm1' class="ajax_status_conteiner span3 box"> </div>
<div id='myAjaxForm2' class="ajax_status_conteiner span3 box"> </div>
<div id='myAjaxForm3' class="ajax_status_conteiner span3 box"> </div>
<div id='myAjaxForm4' class="ajax_status_conteiner span3 box"> </div>
<script>
	ctx1 = $('#myAjaxForm1'); // it will remain hidden
	ctx2 = $('#myAjaxForm2'); // it will show saving... message
	ctx3 = $('#myAjaxForm3'); // it will show success message
	ctx4 = $('#myAjaxForm4'); // it will show success message

	$(document).ready(function() {
		ajaxStatus.draw( ctx1 ) ;
		ajaxStatus.draw( ctx2 ) ;
		ajaxStatus.draw( ctx3 ) ;
		ajaxStatus.draw( ctx4 ) ;

		ajaxStatus.switchToSaving( ctx2 ) ;
		ajaxStatus.switchToSuccess( ctx3 ) ;
		ajaxStatus.switchToError( ctx4 ) ;
	});
</script>
```

# Functions in Version 1.0.1
Here are listed each one of the features provided by **Ajax_Status**.

## ajaxStatus.version()
Returns the version of this **Ajax_Status** library.

## hide(ctx) {
Hides the widget.

## switchToSaving(ctx) {
Shows and turns on the blue saving message.

## switchToSuccess(ctx) {
Shows and turns on the green success message.

## switchToError(ctx) {
Shows and turns on the red error message.

# Deployment 
The **Ajax_Status** requires [**JQuery 3.5.1**](https://jquery.com/download/), and the **AdminFlare 1.3.0** used privately at [**ExpandedVenture**](https://expandedventure.com/expandedventure).

All the libraries are already included in this repository.

# Additional Notes
The **Ajax_Status** is used at [**ExpandedVenture**](https://expandedventure.com/expandedventure) to develop different UI/UX features.

The **Ajax_Status** library is just starting on Nov-2020, and more functions will be added as needed.

The **Ajax_Status** library has been written following the [**W3C JavaScript Best Practices**](https://www.w3.org/community/webed/wiki/JavaScript_best_practices).

# Disclaimer
Use at your own risk. The use of the software and scripts downloaded on this site is done at your own discretion and risk and with agreement that you will be solely responsible for any damage to any computer system or loss of data that results from such activities.

# Maintainer
Leandro Daniel Sardi <leandro((dot))sardi((@))expandedventure.com>