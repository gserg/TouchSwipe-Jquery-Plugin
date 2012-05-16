A jQuery plugin to capture left, right, up and down swipes on touch devices.

You can capture 2 finger or 1 finger swipes, set the threshold and define either a catch all handler, or individual direction handlers.

###Options:###
|Name              |Type     |Default |Description |
|:-----------------|:--------|:-------|:-----------|
|swipe             |Function |        |A catch all handler that is triggered for all swipe directions. Handler is passed 3 arguments, the original event object, the direction of the swipe : "left", "right", "up", "down" and the distance of the swipe. |
|swipeLeft         |Function |        |A handler that is triggered for "left" swipes. Handler is passed 3 arguments, the original event object, the direction of the swipe : "left", "right", "up", "down" and the distance of the swipe. |
|swipeRight        |Function |        |A handler that is triggered for "right" swipes. Handler is passed 3 arguments, the original event object, the direction of the swipe : "left", "right", "up", "down" and the distance of the swipe. |
|swipeUp           |Function |        |A handler that is triggered for "up" swipes. Handler is passed 3 arguments, the original event object, the direction of the swipe : "left", "right", "up", "down" and the distance of the swipe. |
|swipeDown         |Function |        |A handler that is triggered for "down" swipes. Handler is passed 3 arguments, the original event object, the direction of the swipe : "left", "right", "up", "down" and the distance of the swipe. |
|swipeStatus       |Function |        |A handler triggered for every phase of the swipe. Handler is passed 4 arguments: event : The original event object, phase:The current swipe face, either "start?, "move?, "end? or "cancel?. direction : The swipe direction, either "up", "down", "left" or "right" distance : The distance of the swipe. |
|click             |Function |        |A handler triggered when a user just clicks on the item, rather than swipes it. If they do not move, click is triggered, if they do move, it is not. |
|fingers           |int      |1       |The number of fingers to trigger the swipe, 1 or 2.
|threshold         |int      |75      |The number of pixels that the user must move their finger by before it is considered a swipe.
|timeThreshold     |int      |250     |Time, in milliseconds, between touchStart and touchEnd must not exceed in order to be considered a swipe.
|triggerOnTouchEnd |Boolean  |true    |If true, the swipe events are triggered when the touch end event is received (user releases finger).  If false, it will be triggered on reaching the threshold, and then cancel the touch event automatically.
|allowPageScroll   |String   |"auto"  |How the browser handles page scrolls when the user is swiping on a touchSwipe object. 
										"auto" : all undefined swipes will cause the page to scroll in that direction.
										"none" : the page will not scroll when user swipes.
										"horizontal" : will force page to scroll on horizontal swipes.
										"vertical" : will force page to scroll on vertical swipes.|

This jQuery plugin will only run on devices running Mobile Webkit based browsers (iOS 2.0+, android 2.2+)
