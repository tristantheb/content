---
title: "PointerEvent: tiltX property"
short-title: tiltX
slug: Web/API/PointerEvent/tiltX
page-type: web-api-instance-property
browser-compat: api.PointerEvent.tiltX
---

{{ APIRef("Pointer Events") }}

The **`tiltX`** read-only property of the {{domxref("PointerEvent")}} interface is the angle (in degrees) between the _Y-Z plane_ of the pointer and the screen.
This property is typically only useful for a pen/stylus pointer type.

Depending on the specific hardware and platform, user agents will likely only receive one set of values for the transducer orientation relative to the screen plane — either `tiltX` and {{domxref("PointerEvent.tiltY", "tiltY")}} or {{domxref("PointerEvent.altitudeAngle", "altitudeAngle")}} and {{domxref("PointerEvent.azimuthAngle", "azimuthAngle")}}.

![The tiltX angle of a pointer compared to the tiltY angle](tilt_x_y_angles.svg)

For an additional illustration of this property see [Figure 2 in the specification](https://w3c.github.io/pointerevents/#dom-pointerevent-tiltx).

## Value

The angle in degrees between the Y-Z plane of the pointer (stylus) and the screen. The range of values is `-90` to `90`, inclusive, where a positive value is a tilt to the right.
For devices that do not support this property, the value is `0`.

## Examples

This example illustrates simple accessing of the `tiltX` and {{domxref("PointerEvent.tiltY","tiltY")}} properties.

```js
someElement.addEventListener(
  "pointerdown",
  (event) => {
    process_tilt(event.tiltX, event.tiltY);
  },
  false,
);
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{domxref("PointerEvent.tiltY")}}
- {{domxref("PointerEvent.altitudeAngle")}}
- {{domxref("PointerEvent.azimuthAngle")}}
