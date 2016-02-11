Controls
========

Javascript library meant to create DOM-controls.

How to use
==========

You create a control instance which turns an array of control properties into dom objects and adds it to a container.

Example:

	var domContainer = document.getElementById("container");
	var controlArray = [{}, {}, ...];
    var controls = new Controls(domContainer, controlArray);

The controls have been added and are ready to use. You can now use the controls instance to manipulate the controls.

Example:

	controls.byName.someName.input                // Input dom element; Can be a button, input element, ... has .value property that can be get and set (not guaranteed to invoke action)

Control properties
==================

		{
			name: "someName",              // Required, string to use as name
			type: "button",                // Possible types: button, text, integer or color (hex)
			text: "Click here"             // Used by some control types as button text or placeholder
			classPrepend: "name-"          // A string that will be added to all classes, default ""
			image: "link/to/image.png",    // If provided this image will be used instead of text
			alt: "Image description",      // Will be used as image alt
			value: "Value",                // The current value
			action: function (value) {},        // Function that will be called with the value when status change (button press, stopped typing, changed value, ...)
			title: "Change value",         // Used as title on button, input, ...
			min: 1,                        // Minimum value for integers
			max: 50                        // Maximum value for integer
		}