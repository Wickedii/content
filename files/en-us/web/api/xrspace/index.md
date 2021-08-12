---
title: XRSpace
slug: Web/API/XRSpace
tags:
  - API
  - AR
  - Augmented Realty
  - Experimental
  - Interface
  - Reference
  - VR
  - Virtual Reality
  - WebXR
  - WebXR Device API
  - XRSpace
browser-compat: api.XRSpace
---
<div>{{securecontext_header}}{{APIRef("WebXR Device API")}}</div>

<p>The <strong><code>XRSpace</code></strong> interface of the <a href="/en-US/docs/Web/API/WebXR_Device_API">WebXR Device API</a> is an abstract interface providing a common basis for every class which represents a virtual coordinate system within the virtual world, in which its origin corresponds to a physical location. Spatial data in WebXR is always expressed relative to an object based upon one of the descendant interfaces of <code>XRSpace</code>, at the time at which a given {{domxref("XRFrame")}} takes place.</p>

<p class="summary">Numeric values such as pose positions are thus coordinates in the corresponding <code>XRSpace</code>, relative to that space's origin.</p>

<div class="notecard note">
<p class="summary"><strong>Note:</strong> The <code>XRSpace</code> interface is never used directly; instead, all spaces are created using one of the interfaces based on <code>XRSpace</code>. At this time, those are {{domxref("XRReferenceSpace")}} and {{domxref("XRBoundedReferenceSpace")}}.</p>
</div>

<h2 id="Interfaces_based_on_XRSpace">Interfaces based on XRSpace</h2>

<p>Below is a list of interfaces based on the <code>XRSpace</code> interface.</p>

<dl>
	<dt>{{domxref("XRBoundedReferenceSpace")}}</dt>
	<dd>Represents a reference space which may move within a region of space whose borders are defined by an array of points laid out in clockwise order along the floor to define the passable region of the space. The origin of an <code>XRBoundedReferenceSpace</code> is always at floor level, with its X and Z coordinates typically defaulting to a location near the room's center.</dd>
	<dt>{{domxref("XRReferenceSpace")}}</dt>
	<dd>Represents a reference space which is typically expected to remain static for the duration of the {{domxref("XRSession")}}. While objects may move within the space, the space itself remains fixed in place. There are exceptions to this static nature; most commonly, an <code>XRReferenceSpace</code> may move in order to adjust based on reconfiguration of the user's headset or other motion-sensitive device.</dd>
</dl>

<h2 id="Properties">Properties</h2>

<p><em>The <code>XRSpace</code> interface defines no properties of its own; however, it does inherit the properties of its parent interface, {{domxref("EventTarget")}}.</em></p>

<h2 id="Methods">Methods</h2>

<p><em>The <code>XRSpace</code> interface provides no methods of its own. However, it inherits the methods of {{domxref("EventTarget")}}, its parent interface.</em></p>

<h2 id="Specifications">Specifications</h2>

{{Specifications}}

<h2 id="Browser_compatibility">Browser compatibility</h2>

<p>{{Compat}}</p>