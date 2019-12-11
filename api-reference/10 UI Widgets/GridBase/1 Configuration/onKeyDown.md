---
EventForAction: ..\4 Events\keyDown.md
default: null
type: function(e)
---
---
##### shortDescription
A function that is executed when the widget is in focus and a key has been pressed down.

##### param(e): Object
Information about the event that caused the function's execution.

##### field(e.component): {WidgetName}
The widget's instance.

##### field(e.element): dxElement
The widget's container. It is an [HTML Element](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement) or a [jQuery Element](https://api.jquery.com/Types/#jQuery) when you use jQuery.

##### field(e.jQueryEvent): jQuery.Event
The jQuery event that caused the function's execution. Deprecated in favor of the **event** field.

##### field(e.jQueryEvent).deprecated
Use 'event' instead.

##### field(e.event): event
The event that caused the function's execution. It is a [dxEvent](/api-reference/50%20Common/Object%20Structures/dxEvent '/Documentation/ApiReference/Common/Object_Structures/dxEvent/') or a [jQuery.Event](https://api.jquery.com/category/events/event-object) when you use jQuery.

##### field(e.handled): Boolean
Indicates whether the widget has already handled this event.

---