---
module: animation/frame
export: cancel
---
---
##### shortDescription
Cancels an animation frame request scheduled with the [requestAnimationFrame](/Documentation/ApiReference/Common/Utils/#requestAnimationFramecallback) method.

##### param(requestID): Number
The identifier returned by **requestAnimationFrame** method.

---
This method acts as a normalization of the standard [cancelAnimationFrame](https://developer.mozilla.org/en-US/docs/Web/API/window.cancelAnimationFrame) method of the **window** object.

    <!--JavaScript-->
    window.cancelAnimationFrame ||
    window.webkitCancelAnimationFrame ||
    window.mozCancelAnimationFrame ||
    window.oCancelAnimationFrame ||
    window.msCancelAnimationFrame

If the API in the code above is not supported, the **DevExpress.utils.cancelAnimationFrame(requestID)** method clears a timer set with the **requestAnimationFrame** method.