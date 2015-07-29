Poppy is a base component for building any kind of popups: modal, tooltip, popup, dropdown, confirm, notifier, popover, lightbox, balloon etc.

```js
var Poppy = require('poppy');


var popup = new Poppy({

});
popup.show(target);


var tooltip = new Poppy({

});


var notification = new Poppy({

});


var dropdown = new Poppy({
	tip: true
});


var modal = new Poppy({
	closable: true,
	escapable: true,
	overlay: true,
	resizable: true,
	placement: 'free',
	draggable: true
});
```

## Why not component/tip, component/dialog etc?

* They hide element from the content when it’s comfortable to always have access to it via DOM.
* They have a very difficult to understand constructing method, options/methods are vague. Bad docs. I did something by docs and it didn’t work.
* Community is agressive and lazy simultaneously. It is not that easy to make changes.
* It has no centralized reliable placing method/algorithm
* It has no default styles
* Dialog has no animation style
* Dialog container is not draggable
* Dialog container has blind click zone of overlay
* Dialog container is weirdly resized, if there is dynamic content within
* Dialog container has no proper overlay within body
* Tip is difficult to customize color, position
* Cannot create multiple dialogs
* Cannot stack dialogs