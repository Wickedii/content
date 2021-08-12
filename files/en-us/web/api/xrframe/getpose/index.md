---
title: XRFrame.getPose()
slug: Web/API/XRFrame/getPose
tags:
- API
- AR
- Augmented Reality
- Interface
- Method
- Reference
- VR
- Virtual Reality
- WebXR
- WebXR Device API
- XRFrame
- getPose
browser-compat: api.XRFrame.getPose
---
<div>{{APIRef("WebXR Device API")}}</div>

<p>The {{domxref("XRFrame")}} method <code><strong>getPose()</strong></code> returns the relative position and
orientation—the pose—of one {{domxref("XRSpace")}} to that of another space. With this, you can observe the motion of objects relative to each other and to fixed locations throughout the scene.</p>

<p>For example, to get the position of a controller relative to the viewer's head, you would compare the controller's {{domxref("XRInputSource.gripSpace", "gripSpace")}} to the {{domxref("XRReferenceSpace")}} of type <code>viewer</code>.</p>

<h2 id="Syntax">Syntax</h2>

<pre
  class="brush: js">var <var>xrPose</var> = <em>xrFrame</em>.getPose(<em>space</em>, <em>baseSpace</em>);</pre>

<h3 id="Parameters">Parameters</h3>

<dl>
  <dt><code>space</code></dt>
  <dd>An {{domxref("XRSpace")}} specifying the space for which to obtain an
    {{domxref("XRPose")}} describing the item's position and orientation.</dd>
  <dt><code>baseSpace</code></dt>
  <dd>An {{domxref("XRSpace")}} to use as the base or origin for the purposes of computing
    the relative position and orientation.</dd>
</dl>

<h3 id="Return_value">Return value</h3>

<p>An {{domxref("XRPose")}} object specifying the position and orientation, relative to
  the {{domxref("XRSpace")}} indicated by <code>baseSpace</code>.</p>

<h2 id="Specifications">Specifications</h2>

{{Specifications}}

<h2 id="Browser_compatibility">Browser compatibility</h2>

<p>{{Compat}}</p>