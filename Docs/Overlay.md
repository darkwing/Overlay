Class: Overlay {#Overlay}
=================================

### Implements:

Options, Events


Overlay Method: constructor {#Overlay:constructor}
-----------------------------------------------------------


### Syntax:

	var overlay = new Overlay(document.body);

### Arguments:

1. container - (*string*)  The ID of the container (usually document.body) which will host the overlay.
2. options - (**)  The options for the Overlay instance.

### Options:

* id - (*string*, defaults to 'overlay') - The ID of the overlay to be created.
* color - (*string*, defaults to '#000') - The base background color of the overlay.  Keep in mind the actual screen color will change with the opacity level.
* duration - (*integer*, defaults to 500) - The open/close duration of the overlay.
* opacity - (*float*, defaults to 0.5) - The destination opacity level of the overlay.

### Events:

### onClick

* (*function*) Function to execute when the overlay is clicked

### Signature

	onClick(fn)
	
### Example

	onClick: function() {
		this.close();
	}
	
### onClose

* (*function*) Function to execute immediately after the close directive has been given (before the opacity fade has completed).

### Signature

	onClose(fn)

### onHide

* (*function*) Function to execute when the overlay has been completely hidden (after the "close" event).

### Signature

	onHide(fn)

### onOpen

* (*function*) Function to execute immediately after the open directive has been given (before the opacity fade has completed).

### Signature

	onOpen(fn)
	
### onShow

* (*function*) Function to execute when the overlay has completed it's fade in (after the "open" event)

### Signature

	onShow(fn)