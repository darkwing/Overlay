Overlay
=========

Overlay is a compact, simple overlay class which allows for maximum control over its use.

![Screenshot](http://davidwalsh.name/dw-content/overlayscreen.png)

How to Use
----------

Overlay may be initialized at any time.  The first and only required argument is the overlay's "container" which is usually document.body.  Options may be given as the second argument.

Overlay also provides click, close, hide, open, and show events.
	
### Javascript
	var overlay = new Overlay(document.body,{
			id: 'overlay',
			color: '#000',
			duration: 300,
			opacity: 0.4,
			onClick: function() {
				this.close();
			},
			onShow: function() {
				//make ajax call while the overlay is happening...?
				//var Request = new Request()....
			}
	});

For specific usage and options, please read the documentation or visit [http://davidwalsh.name/js/overlay](http://davidwalsh.name/js/overlay)