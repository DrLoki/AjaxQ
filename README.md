# AjaxQ
## A tiny, simple jQuery plugin for sequential ajax requests

See http://foliotek.github.com/AjaxQ for a demonstration and documentation

## Usage

`$.ajaxq` follows the [$.ajax](http://api.jquery.com/jQuery.ajax/) options and return value, with an extra first parameter (the queue name).

    $.ajaxq(name, opts);
    
`$.getq` follows the [$.get](http://api.jquery.com/jQuery.get/) options and return value, with an extra first parameter (the queue name).

    $.getq(name, opts);
    
`$.postq` follows the [$.post](http://api.jquery.com/jQuery.post/) options and return value, with an extra first parameter (the queue name).

    $.postq(name, opts);
    
`$.ajaxq.isRunning` returns a boolean representing if any requests are currently running.  `qname is an optional parameter.

    $.ajaxq.isRunning(qname);

`$.ajaxq.clear` removes any unprocessed requests from the queue.  `qname is an optional parameter.

	$.ajaxq.clear(qname);

`$.ajaxq.abort` aborts the current request, and removes any unprocessed reqeusts from the queue.  `qname is required.

  ```javascript
  $.ajaxq.abort(qname);
  ```
    
## Demo

http://foliotek.github.com/AjaxQ#demo

