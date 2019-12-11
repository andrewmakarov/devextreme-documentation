---
EventForAction: ..\4 Events\editorEnterKey.md
default: null
type: function(e)
---
---
##### shortDescription
A function that is executed when the Enter key has been pressed while an editor is focused.

##### param(e): Object
Information about the event.

##### field(e.component): {WidgetName}
The widget's instance.

##### field(e.element): dxElement
The form's container. It is an [HTML Element](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement) or a [jQuery Element](https://api.jquery.com/Types/#jQuery) when you use jQuery.

##### field(e.model): Object
The model data. Available only if Knockout is used.

##### field(e.dataField): String
The path to the [formData](/api-reference/10%20UI%20Widgets/dxForm/1%20Configuration/formData.md '/Documentation/ApiReference/UI_Widgets/dxForm/Configuration/#formData') object field associated with the current editor.

---