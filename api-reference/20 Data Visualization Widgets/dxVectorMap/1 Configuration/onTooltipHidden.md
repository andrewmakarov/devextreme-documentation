---
EventForAction: ..\4 Events\tooltipHidden.md
default: null
type: function(e)
---
---
##### notUsedInTheme

##### shortDescription
A function that is executed when a tooltip becomes hidden.

##### param(e): Object
Information about the event.

##### field(e.component): {WidgetName}
The widget's instance.

##### field(e.element): dxElement
The widget's container. It is an [HTML Element](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement) or a [jQuery Element](https://api.jquery.com/Types/#jQuery) when you use jQuery.

##### field(e.model): Object
The model data. Available only if you use Knockout.

##### field(e.target): MapLayerElement
The layer element whose tooltip is hidden; described in the [Layer Element](/api-reference/20%20Data%20Visualization%20Widgets/dxVectorMap/7%20Map%20Elements/Layer%20Element '/Documentation/ApiReference/Data_Visualization_Widgets/dxVectorMap/Map_Elements/Layer_Element/') section.

---