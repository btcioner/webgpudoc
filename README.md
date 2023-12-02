File: /files/en-us/web/api/gpuadapterinfo/architecture/index.md
---
title: "GPUAdapterInfo: architecture property"
short-title: architecture
slug: Web/API/GPUAdapterInfo/architecture
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUAdapterInfo.architecture
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`architecture`** read-only property of the
{{domxref("GPUAdapterInfo")}} interface returns the name of the family or class of GPUs the adapter belongs to, or an empty string if it is not available.

## Value

A string.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const adapterInfo = await adapter.requestAdapterInfo();
  console.log(adapterInfo.architecture);

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuadapterinfo/description/index.md
---
title: "GPUAdapterInfo: description property"
short-title: description
slug: Web/API/GPUAdapterInfo/description
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUAdapterInfo.description
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`description`** read-only property of the
{{domxref("GPUAdapterInfo")}} interface returns a human-readable string describing the adapter, or an empty string if it is not available.

## Value

A string.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const adapterInfo = await adapter.requestAdapterInfo();
  console.log(adapterInfo.description);

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuadapterinfo/index.md
---
title: GPUAdapterInfo
slug: Web/API/GPUAdapterInfo
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUAdapterInfo
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUAdapterInfo`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} contains identifying information about a {{domxref("GPUAdapter")}}.

A `GPUAdapterInfo` object instance is requested using the {{domxref("GPUAdapter.requestAdapterInfo()")}} method.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUAdapterInfo.architecture", "architecture")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : The name of the family or class of GPUs the adapter belongs to. Returns an empty string if it is not available.
- {{domxref("GPUAdapterInfo.description", "description")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A human-readable string describing the adapter. Returns an empty string if it is not available.
- {{domxref("GPUAdapterInfo.device", "device")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A vendor-specific identifier for the adapter. Returns an empty string if it is not available.
- {{domxref("GPUAdapterInfo.vendor", "vendor")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : The name of the adapter vendor. Returns an empty string if it is not available.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const adapterInfo = await adapter.requestAdapterInfo();
  console.log(adapterInfo.architecture);
  console.log(adapterInfo.vendor);

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuadapterinfo/device/index.md
---
title: "GPUAdapterInfo: device property"
short-title: device
slug: Web/API/GPUAdapterInfo/device
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUAdapterInfo.device
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`device`** read-only property of the
{{domxref("GPUAdapterInfo")}} interface returns a vendor-specific identifier for the adapter, or an empty string if it is not available.

## Value

A string.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const adapterInfo = await adapter.requestAdapterInfo();
  console.log(adapterInfo.device);

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuadapterinfo/vendor/index.md
---
title: "GPUAdapterInfo: vendor property"
short-title: vendor
slug: Web/API/GPUAdapterInfo/vendor
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUAdapterInfo.vendor
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`vendor`** read-only property of the
{{domxref("GPUAdapterInfo")}} interface returns the name of the adapter vendor, or an empty string if it is not available.

## Value

A string.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const adapterInfo = await adapter.requestAdapterInfo();
  console.log(adapterInfo.vendor);

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpu/getpreferredcanvasformat/index.md
---
title: "GPU: getPreferredCanvasFormat() method"
short-title: getPreferredCanvasFormat()
slug: Web/API/GPU/getPreferredCanvasFormat
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPU.getPreferredCanvasFormat
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`getPreferredCanvasFormat()`** method of the
{{domxref("GPU")}} interface returns the optimal canvas texture format for displaying 8-bit depth, standard dynamic range content on the current system.

This is commonly used to provide a {{domxref("GPUCanvasContext.configure()")}} call with the optimal `format` value for the current system. This is recommended ‚Äî if you don't use the preferred format when configuring the canvas context, you may incur additional overhead, such as additional texture copies, depending on the platform.

## Syntax

```js-nolint
getPreferredCanvasFormat()
```

### Parameters

None.

### Return value

A string indicating a canvas texture format. The value can be `rgba8unorm` or `bgra8unorm`.

### Exceptions

None.

## Examples

```js
const canvas = document.querySelector("#gpuCanvas");
const context = canvas.getContext("webgpu");

context.configure({
  device: device,
  format: navigator.gpu.getPreferredCanvasFormat(),
  alphaMode: "premultiplied",
});
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpu/requestadapter/index.md
---
title: "GPU: requestAdapter() method"
short-title: requestAdapter()
slug: Web/API/GPU/requestAdapter
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPU.requestAdapter
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`requestAdapter()`** method of the
{{domxref("GPU")}} interface returns a {{jsxref("Promise")}} that fulfills with a {{domxref("GPUAdapter")}} object instance. From this you can request a {{domxref("GPUDevice")}}, adapter info, features, and limits.

Note that the user agent chooses whether to return an adapter. If so, it chooses according to the provided options. If no options are provided, the device will provide access to the default adapter, which is usually good enough for most purposes.

## Syntax

```js-nolint
requestAdapter()
requestAdapter(options)
```

### Parameters

- `options` {{optional_inline}}

  - : An object containing the following properties:

    - `powerPreference` {{optional_inline}}

      - : An enumerated value that can be used to provide a hint to the user agent indicating what class of adapter should be chosen from the system's available adapters. Available values are:

        - `undefined` (or not specified), which provides no hint.
        - `"low-power"`, which provides a hint to prioritize power savings over performance. If your app runs OK with this setting, it is recommended to use it, as it can significantly improve battery life on portable devices. This is usually the default if no options are provided.
        - `"high-performance"`, which provides a hint to prioritize performance over power consumption. You are encouraged to only specify this value if absolutely necessary, since it may significantly decrease battery life on portable devices. It may also result in increased {{domxref("GPUDevice")}} loss ‚Äî the system will sometimes elect to switch to a lower-power adapter to save power.

        This hint's primary purpose is to influence which GPU is used in a multi-GPU system. For instance, some laptops have a low-power integrated GPU and a high-performance discrete GPU. Different factors may affect which adapter is returned including battery status, attached displays, or removable GPUs.

        > **Note:** On Chrome running on dual-GPU macOS devices, if `requestAdapter()` is called without a `powerPreference` option, the high-performance discrete GPU is returned when the user's device is on AC power. Otherwise, the low-power integrated GPU is returned.

### Fallback adapters

The adapter provided by the user agent may be a **fallback adapter**, if it determines it to be the most appropriate option available. A fallback adapter generally has significant performance caveats in exchange for some combination of wider compatibility, more predictable behavior, or improved privacy. For example, some browsers may offer a software-based implementation of the API via a fallback adapter. A fallback adapter will not be available on every system.

If you wish to prevent your apps from running on fallback adapters, you should check the {{domxref("GPUAdapter.isFallbackAdapter")}} attribute prior to requesting a {{domxref("GPUDevice")}}.

> **Note:** The specification includes a `forceFallbackAdapter` option for `requestAdapter()`. This is a boolean that, if set to `true`, forces the user agent to return a fallback adapter if one is available. This is not yet supported by any browser.

### Return value

A {{jsxref("Promise")}} that fulfills with a {{domxref("GPUAdapter")}} object instance if the request is successful.

`requestAdapter()` will resolve to `null` if an appropriate adapter is not available.

### Exceptions

None.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const device = await adapter.requestDevice();

  //...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpu/index.md
---
title: GPU
slug: Web/API/GPU
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPU
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPU`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} is the starting point for using WebGPU. It can be used to return a {{domxref("GPUAdapter")}} from which you can request devices, configure features and limits, and more.

The `GPU` object for the current context is accessed via the {{domxref("Navigator.gpu")}} or {{domxref("WorkerNavigator.gpu")}} properties.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPU.wgslLanguageFeatures", "wgslLanguageFeatures")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A {{domxref("WGSLLanguageFeatures")}} object that reports the [WGSL language extensions](https://gpuweb.github.io/gpuweb/wgsl/#language-extension) supported by the WebGPU implementation.

## Instance methods

- {{domxref("GPU.requestAdapter", "requestAdapter()")}} {{Experimental_Inline}}
  - : Returns a {{jsxref("Promise")}} that fulfills with a {{domxref("GPUAdapter")}} object instance. From this you can request a {{domxref("GPUDevice")}}, which is the primary interface for using WebGPU functionality.
- {{domxref("GPU.getPreferredCanvasFormat", "getPreferredCanvasFormat()")}} {{Experimental_Inline}}
  - : Returns the optimal canvas texture format for displaying 8-bit depth, standard dynamic range content on the current system.

## Examples

### Requesting an adapter and a device

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const device = await adapter.requestDevice();

  //...
}
```

### Configuring a GPUCanvasContext with the optimal texture format

```js
const canvas = document.querySelector("#gpuCanvas");
const context = canvas.getContext("webgpu");

context.configure({
  device: device,
  format: navigator.gpu.getPreferredCanvasFormat(),
  alphaMode: "premultiplied",
});
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpu/wgsllanguagefeatures/index.md
---
title: "GPU: wgslLanguageFeatures property"
short-title: wgslLanguageFeatures
slug: Web/API/GPU/wgslLanguageFeatures
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPU.wgslLanguageFeatures
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`wgslLanguageFeatures`** read-only property of the
{{domxref("GPU")}} interface returns a {{domxref("WGSLLanguageFeatures")}} object that reports the [WGSL language extensions](https://gpuweb.github.io/gpuweb/wgsl/#language-extension) supported by the WebGPU implementation.

> **Note:** Not all WGSL language extensions are available to WebGPU in all browsers that support the API. We recommend you thoroughly test any extensions you choose to use.

## Value

A {{domxref("WGSLLanguageFeatures")}} object instance. This is a [setlike](/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set) object.

## Examples

```js
if (!navigator.gpu) {
  throw Error("WebGPU not supported.");
}

const wgslFeatures = navigator.gpu.wgslLanguageFeatures;

// Return the size of the set
console.log(wgslFeatures.size);

// Iterate through all the set values using values()
const valueIterator = wgslFeatures.values();
for (const value of valueIterator) {
  console.log(value);
}

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gputextureview/label/index.md
---
title: "GPUTextureView: label property"
short-title: label
slug: Web/API/GPUTextureView/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUTextureView.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** property of the
{{domxref("GPUTextureView")}} interface provides a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUTexture.createView()")}} call, or you can get and set it directly on the `GPUTextureView` object.

## Value

A string. If this has not been previously set as described above, it will be an empty string.

## Examples

Setting and getting a label via `GPUTextureView.label`:

```js
// ...

const depthTexture = device.createTexture({
  size: [canvas.width, canvas.height],
  format: "depth24plus",
  usage: GPUTextureUsage.RENDER_ATTACHMENT,
});

const view = depthTexture.createView();

view.label = "myview";

console.log(view.label); // "myview"
```

Setting a label via the originating {{domxref("GPUTexture.createView()")}} call, and then getting it via `GPUTextureView.label`:

```js
// ...

const depthTexture = device.createTexture({
  size: [canvas.width, canvas.height],
  format: "depth24plus",
  usage: GPUTextureUsage.RENDER_ATTACHMENT,
});

const view = depthTexture.createView({
  label: "myview",
});

console.log(view.label); // "myview"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gputextureview/index.md
---
title: GPUTextureView
slug: Web/API/GPUTextureView
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUTextureView
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUTextureView`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents a view into a subset of the texture resources defined by a particular {{domxref("GPUTexture")}}.

A `GPUTextureView` object instance is created using the {{domxref("GPUTexture.createView()")}} method.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUTextureView.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Examples

In the WebGPU Samples [Cubemap demo](https://webgpu.github.io/webgpu-samples/samples/cubemap), you will see multiple examples of how `GPUTextureView`s (created by {{domxref("GPUTexture.createView()")}} calls) are used, both as a `resource` in a {{domxref("GPUDevice.createBindGroup()")}} call, and as a provided `view` in the `depthStencilAttachment` object of a {{domxref("GPUCommandEncoder.beginRenderPass()")}} descriptor.

```js
const uniformBindGroup = device.createBindGroup({
  layout: pipeline.getBindGroupLayout(0),
  entries: [
    {
      binding: 0,
      resource: {
        buffer: uniformBuffer,
        offset: 0,
        size: uniformBufferSize,
      },
    },
    {
      binding: 1,
      resource: sampler,
    },
    {
      binding: 2,
      resource: cubemapTexture.createView({
        dimension: "cube",
      }),
    },
  ],
});

const renderPassDescriptor: GPURenderPassDescriptor = {
  colorAttachments: [
    {
      view: undefined, // Assigned later
      loadOp: "clear",
      storeOp: "store",
    },
  ],
  depthStencilAttachment: {
    view: depthTexture.createView(),
    depthClearValue: 1.0,
    depthLoadOp: "clear",
    depthStoreOp: "store",
  },
};

// ...

const commandEncoder = device.createCommandEncoder();
const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpubindgroup/label/index.md
---
title: "GPUBindGroup: label property"
short-title: label
slug: Web/API/GPUBindGroup/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUBindGroup.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** property of the
{{domxref("GPUBindGroup")}} interface provides a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUDevice.createBindGroup()")}} call, or you can get and set it directly on the `GPUBindGroup` object.

## Value

A string. If this has not been previously set as described above, it will be an empty string.

## Examples

Setting and getting a label via `GPUBindGroup.label`:

```js
// ...

const bindGroup = device.createBindGroup({
  layout: bindGroupLayout,
  entries: [
    {
      binding: 0,
      resource: {
        buffer: output,
      },
    },
  ],
});

bindGroup.label = "mybindgroup";

console.log(bindGroup.label); // "mybindgroup";
```

Setting a label via the originating {{domxref("GPUDevice.createBindGroup()")}} call, and then getting it via `GPUBindGroup.label`:

```js
// ...

const bindGroup = device.createBindGroup({
  layout: bindGroupLayout,
  entries: [
    {
      binding: 0,
      resource: {
        buffer: output,
      },
    },
  ],
  label: "mybindgroup",
});

console.log(bindGroup.label); // "mybindgroup";
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpubindgroup/index.md
---
title: GPUBindGroup
slug: Web/API/GPUBindGroup
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUBindGroup
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUBindGroup`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} is based on a {{domxref("GPUBindGroupLayout")}} and defines a set of resources to be bound together in a group and how those resources are used in shader stages.

A `GPUBindGroup` object instance is created using the {{domxref("GPUDevice.createBindGroup()")}} method.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUBindGroup.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Examples

> **Note:** The [WebGPU samples](https://webgpu.github.io/webgpu-samples/) feature many more examples.

### Basic example

Our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/) shows an example of creating a bind group layout and then using that as a template when creating a bind group.

```js
// ...

const bindGroupLayout = device.createBindGroupLayout({
  entries: [
    {
      binding: 0,
      visibility: GPUShaderStage.COMPUTE,
      buffer: {
        type: "storage",
      },
    },
  ],
});

const bindGroup = device.createBindGroup({
  layout: bindGroupLayout,
  entries: [
    {
      binding: 0,
      resource: {
        buffer: output,
      },
    },
  ],
});

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/workernavigator/gpu/index.md
---
title: "WorkerNavigator: gpu property"
short-title: gpu
slug: Web/API/WorkerNavigator/gpu
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.WorkerNavigator.gpu
---

{{APIRef("Web Workers API")}}{{SeeCompatTable}}

The **`gpu`** read-only property of the {{domxref("WorkerNavigator")}} interface returns the {{domxref("GPU")}} object for the current worker context, which is the entry point for the {{domxref("WebGPU_API", "WebGPU API", "", "nocode")}}.

## Value

A {{domxref("GPU")}} object.

## Examples

```js
// Can be run inside a web worker
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const device = await adapter.requestDevice();

  //...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{domxref("WebGPU_API", "WebGPU API", "", "nocode")}}
-e 

File: /files/en-us/web/api/gpucanvascontext/configure/index.md
---
title: "GPUCanvasContext: configure() method"
short-title: configure()
slug: Web/API/GPUCanvasContext/configure
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCanvasContext.configure
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`configure()`** method of the
{{domxref("GPUCanvasContext")}} interface configures the context to use for rendering with a given {{domxref("GPUDevice")}}. When called the canvas will initially be cleared to transparent black.

## Syntax

```js-nolint
configure(configuration)
```

### Parameters

- `configuration`

  - : An object containing the following properties:

    - `alphaMode` {{optional_inline}}
      - : An enumerated value that specifies the effect that alpha values will have on the content of textures returned by {{domxref("GPUCanvasContext.getCurrentTexture()", "getCurrentTexture()")}} when read, displayed, or used as an image source. Possible values are:
        - `opaque`: Alpha values are ignored ‚Äî if a texture is not already opaque, the alpha channel is cleared to 1.0 when it is used as an image source or displayed to the screen. This is the default value.
        - `premultiplied`: Color values are premultiplied by their alpha value. For example, 100% red at 50% alpha is `[0.5, 0, 0, 0.5]`.
    - `colorSpace` {{optional_inline}}
      - : The color space that values written into textures returned by `getCurrentTexture()` should be displayed with. Possible values are `srgb` (the default) and `display-p3`.
    - `device`
      - : The {{domxref("GPUDevice")}} that the rendering information for the context will come from.
    - `format`
      - : The format that textures returned by `getCurrentTexture()` will have. This can be `bgra8unorm`, `rgba8unorm`, or `rgba16float`. The optimal canvas texture format for the current system can be returned by {{domxref("GPU.getPreferredCanvasFormat()")}}. Using this is recommended ‚Äî if you don't use the preferred format when configuring the canvas context, you may incur additional overhead, such as additional texture copies, depending on the platform.
    - `usage` {{optional_inline}}

      - : {{glossary("Bitwise flags")}} specifying the allowed usage for textures returned by `getCurrentTexture()`. Possible values are:

        - `GPUTextureUsage.COPY_SRC`: The texture can be used as the source of a copy operation, for example the source argument of a {{domxref("GPUCommandEncoder.copyTextureToBuffer()")}} call.
        - `GPUTextureUsage.COPY_DST`: The texture can be used as the destination of a copy/write operation, for example the destination argument of a {{domxref("GPUCommandEncoder.copyTextureToTexture()")}} call.
        - `GPUTextureUsage.RENDER_ATTACHMENT`: The texture can be used as a color attachment in a render pass, for example in a color attachment view in a {{domxref("GPUCommandEncoder.beginRenderPass()")}} call. `GPUTextureUsage.RENDER_ATTACHMENT` is the default `usage`, but note that it is not automatically included if a different value is explicitly set; in such cases you need to include it in addition.
        - `GPUTextureUsage.TEXTURE_BINDING`: The texture can be bound for use as a sampled texture in a shader, for example in a bind group entry in a {{domxref("GPUDevice.createBindGroup()")}} call.
        - `GPUTextureUsage.STORAGE_BINDING`: The texture can be bound for use as a storage texture in a shader, for example in a bind group entry in a {{domxref("GPUDevice.createBindGroup()")}} call.

        Note that multiple possible usages can be specified using the [bitwise OR operator](/en-US/docs/Web/JavaScript/Reference/Operators/Bitwise_OR). For example, `usage: GPUTextureUsage.COPY_SRC | GPUTextureUsage.RENDER_ATTACHMENT`.

    - `viewFormats` {{optional_inline}}
      - : An array of formats that views created from textures returned by `getCurrentTexture()` may use. See [Texture Formats](https://gpuweb.github.io/gpuweb/#texture-formats) for all the possible values.

### Return value

None (`undefined`).

## Examples

```js
const canvas = document.querySelector("#gpuCanvas");
const context = canvas.getContext("webgpu");

context.configure({
  device: device,
  format: navigator.gpu.getPreferredCanvasFormat(),
  alphaMode: "premultiplied",
});
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucanvascontext/canvas/index.md
---
title: "GPUCanvasContext: canvas property"
short-title: canvas
slug: Web/API/GPUCanvasContext/canvas
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUCanvasContext.canvas
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`canvas`** read-only property of the
{{domxref("GPUCanvasContext")}} interface returns a reference to the canvas that the context was created from.

## Value

An {{domxref("HTMLCanvasElement")}} or {{domxref("OffscreenCanvas")}} object instance.

## Examples

```js
const canvas = document.querySelector("#gpuCanvas");
const context = canvas.getContext("webgpu");

// returns an HTMLCanvasElement reference
context.canvas;
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucanvascontext/index.md
---
title: GPUCanvasContext
slug: Web/API/GPUCanvasContext
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUCanvasContext
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUCanvasContext`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents the WebGPU rendering context of a {{htmlelement("canvas")}} element, returned via an {{domxref("HTMLCanvasElement.getContext()")}} call with a `contextType` of `"webgpu"`.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUCanvasContext.canvas", "canvas")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : Returns a reference to the canvas that the context was created from.

## Instance methods

- {{domxref("GPUCanvasContext.configure", "configure()")}} {{Experimental_Inline}}
  - : Configures the context to use for rendering with a given {{domxref("GPUDevice")}} and clears the canvas to transparent black.
- {{domxref("GPUCanvasContext.getCurrentTexture", "getCurrentTexture()")}} {{Experimental_Inline}}
  - : Returns the next {{domxref("GPUTexture")}} to be composited to the document by the canvas context.
- {{domxref("GPUCanvasContext.unconfigure", "unconfigure()")}} {{Experimental_Inline}}
  - : Removes any previously-set context configuration, and destroys any textures produced while the canvas context was configured.

## Examples

```js
const canvas = document.querySelector("#gpuCanvas");
const context = canvas.getContext("webgpu");

context.configure({
  device: device,
  format: navigator.gpu.getPreferredCanvasFormat(),
  alphaMode: "premultiplied",
});
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucanvascontext/unconfigure/index.md
---
title: "GPUCanvasContext: unconfigure() method"
short-title: unconfigure()
slug: Web/API/GPUCanvasContext/unconfigure
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCanvasContext.unconfigure
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`unconfigure()`** method of the
{{domxref("GPUCanvasContext")}} interface removes any previously-set context configuration, and destroys any textures returned via {{domxref("GPUCanvasContext.getCurrentTexture", "getCurrentTexture()")}} while the canvas context was configured.

## Syntax

```js-nolint
unconfigure()
```

### Parameters

None.

### Return value

None (`undefined`).

## Examples

```js
const canvas = document.querySelector("#gpuCanvas");
const context = canvas.getContext("webgpu");

context.configure({
  device: device,
  format: navigator.gpu.getPreferredCanvasFormat(),
  alphaMode: "premultiplied",
});

// Later on
context.unconfigure();
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucanvascontext/getcurrenttexture/index.md
---
title: "GPUCanvasContext: getCurrentTexture() method"
short-title: getCurrentTexture()
slug: Web/API/GPUCanvasContext/getCurrentTexture
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCanvasContext.getCurrentTexture
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`getCurrentTexture()`** method of the
{{domxref("GPUCanvasContext")}} interface returns the next {{domxref("GPUTexture")}} to be composited to the document by the canvas context.

## Syntax

```js-nolint
getCurrentTexture()
```

### Parameters

None.

### Return value

A {{domxref("GPUTexture")}} object instance.

### Exceptions

- `InvalidStateError` {{domxref("DOMException")}}
  - : Thrown if `getCurrentTexture()` is called on the canvas context before it is configured (i.e. before {{domxref("GPUCanvasContext.configure()")}} has been called).

## Examples

```js
const canvas = document.querySelector("#gpuCanvas");
const context = canvas.getContext("webgpu");

context.configure({
  device: device,
  format: navigator.gpu.getPreferredCanvasFormat(),
  alphaMode: "premultiplied",
});

//...
// Later on
const commandEncoder = device.createCommandEncoder();

const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: [0, 0, 0, 1], // Opaque black
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
};

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/webgpu_api/index.md
---
title: WebGPU API
slug: Web/API/WebGPU_API
page-type: web-api-overview
status:
  - experimental
browser-compat: api.GPU
---

{{DefaultAPISidebar("WebGPU API")}}{{SeeCompatTable}}{{securecontext_header}}

The **WebGPU API** enables web developers to use the underlying system's GPU (Graphics Processing Unit) to carry out high-performance computations and draw complex images that can be rendered in the browser.

WebGPU is the successor to {{domxref("WebGL_API", "WebGL", "", "nocode")}}, providing better compatibility with modern GPUs, support for general-purpose GPU computations, faster operations, and access to more advanced GPU features.

## Concepts and usage

It is fair to say that {{domxref("WebGL_API", "WebGL", "", "nocode")}} revolutionized the web in terms of graphical capabilities after it first appeared around 2011. WebGL is a JavaScript port of the [OpenGL ES 2.0](https://registry.khronos.org/OpenGL-Refpages/es2.0/) graphics library, allowing web pages to pass rendering computations directly to the device's GPU to be processed at very high speeds, and render the result inside a {{htmlelement("canvas")}} element.

WebGL and the [GLSL](<https://www.khronos.org/opengl/wiki/Core_Language_(GLSL)>) language used to write WebGL shader code are complex, so several WebGL libraries have been created to make WebGL apps easier to write: Popular examples include [Three.js](https://threejs.org/), [Babylon.js](https://www.babylonjs.com/), and [PlayCanvas](https://playcanvas.com/). Developers have used these tools to build immersive web-based 3D games, music videos, training and modeling tools, VR and AR experiences, and more.

However, WebGL has some fundamental issues that needed addressing:

- Since WebGL's release, a new generation of native GPU APIs have appeared ‚Äî the most popular being [Microsoft's Direct3D 12](https://docs.microsoft.com/en-us/windows/win32/direct3d12/direct3d-12-graphics), [Apple's Metal](https://developer.apple.com/metal/), and [The Khronos Group's Vulkan](https://www.vulkan.org/) ‚Äî which provide a multitude of new features. There are no more updates planned to OpenGL (and therefore WebGL), so it won't get any of these new features. WebGPU on the other hand will have new features added to it going forwards.
- WebGL is based wholly around the use case of drawing graphics and rendering them to a canvas. It does not handle general-purpose GPU (GPGPU) computations very well. GPGPU computations are becoming more and more important for many different use cases, for example those based on machine learning models.
- 3D graphics apps are becoming increasingly demanding, both in terms of the number of objects to be rendered simultaneously, and usage of new rendering features.

WebGPU addresses these issues, providing an updated general-purpose architecture compatible with modern GPU APIs, which feels more "webby". It supports graphic rendering, but also has first-class support for GPGPU computations. Rendering of individual objects is significantly cheaper on the CPU side, and it supports modern GPU rendering features such as compute-based particles and post-processing filters like color effects, sharpening, and depth-of-field simulation. In addition, it can handle expensive computations such as culling and skinned model transformation directly on the GPU.

## General model

There are several layers of abstraction between a device GPU and a web browser running the WebGPU API. It is useful to understand these as you begin to learn WebGPU:

![A basic stack diagram showing the position of the different elements of a WebGPU architecture on a device](basic-webgpu-stack.png)

- Physical devices have GPUs. Most devices only have one GPU, but some have more than one. Different GPU types are available:

  - Integrated GPUs, which live on the same board as the CPU and share its memory.
  - Discrete GPUs, which live on their own board, separate from the CPU.
  - Software "GPUs", implemented on the CPU.

  > **Note:** The above diagram assumes a device with only one GPU.

- A native GPU API, which is part of the OS (e.g. Metal on macOS), is a programming interface allowing native applications to use the capabilities of the GPU. API instructions are sent to the GPU (and responses received) via a driver. It is possible for a system to have multiple native OS APIs and drivers available to communicate with the GPU, although the above diagram assumes a device with only one native API/driver.
- A browser's WebGPU implementation handles communicating with the GPU via a native GPU API driver. A WebGPU adapter effectively represents a physical GPU and driver available on the underlying system, in your code.
- A logical device is an abstraction via which a single web app can access GPU capabilities in a compartmentalized way. Logical devices are required to provide multiplexing capabilities. A physical device's GPU is used by many applications and processes concurrently, including potentially many web apps. Each web app needs to be able to access WebGPU in isolation for security and logic reasons.

## Accessing a device

A logical device ‚Äî represented by a {{domxref("GPUDevice")}} object instance ‚Äî is the basis from which a web app accesses all WebGPU functionality. Accessing a device is done as follows:

1. The {{domxref("Navigator.gpu")}} property (or {{domxref("WorkerNavigator.gpu")}} if you are using WebGPU functionality from inside a worker) returns the {{domxref("GPU")}} object for the current context.
2. You access an adapter via the {{domxref("GPU.requestAdapter", "GPU.requestAdapter()")}} method. This method accepts an optional settings object allowing you to request for example a high-performance or low-energy adapter. If this is not included, the device will provide access to the default adapter, which is good enough for most purposes.
3. A device can be requested via {{domxref("GPUAdapter.requestDevice()")}}. This method also accepts an options object (referred to as a descriptor), which can be used to specify the exact features and limits you want the logical device to have. If this is not included, the supplied device will have a reasonable general-purpose spec that is good enough for most purposes.

Putting this together with some feature detection checks, the above process could be achieved as follows:

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const device = await adapter.requestDevice();

  //...
}
```

## Pipelines and shaders: WebGPU app structure

A pipeline is a logical structure containing programmable stages that are completed to get your program's work done. WebGPU is currently able to handle two types of pipeline:

- A render pipeline renders graphics, typically into a {{htmlelement("canvas")}} element, but it could also render graphics offscreen. It has two main stages:

  - A vertex stage, in which a vertex shader takes positioning data fed into the GPU and uses it to position a series of vertices in 3D space by applying specified effects like rotation, translation, or perspective. The vertices are then assembled into primitives such as triangles (the basic building block of rendered graphics) and rasterized by the GPU to figure out what pixels each one should cover on the drawing canvas.

  - A fragment stage, in which a fragment shader computes the color for each pixel covered by the primitives produced by the vertex shader. These computations frequently use inputs such as images (in the form of textures) that provide surface details and the position and color of virtual lights.

- A compute pipeline is for general computation. A compute pipeline contains a single compute stage in which a compute shader takes general data, processes it in parallel across a specified number of workgroups, then returns the result in one or more buffers. The buffers can contain any kind of data.

The shaders mentioned above are sets of instructions processed by the GPU. WebGPU shaders are written in a low-level Rust-like language called [WebGPU Shader Language](https://gpuweb.github.io/gpuweb/wgsl/) (WGSL).

There are several different ways in which you could architect a WebGPU app, but the process will likely contain the following steps:

1. [Create shader modules](#create_shader_modules): Write your shader code in WGSL and package it into one or more shader modules.
2. [Get and configure the canvas context](#get_and_configure_the_canvas_context): Get the `webgpu` context of a `<canvas>` element and configure it to receive information on what graphics to render from your GPU logical device. This step is not necessary if your app has no graphical output, such as one that only uses compute pipelines.
3. [Create resources containing your data](#create_a_buffer_and_write_our_triangle_data_into_it): The data that you want processed by your pipelines needs to be stored in GPU buffers or textures to be accessed by your app.
4. [Create pipelines](#define_and_create_the_render_pipeline): Define pipeline descriptors that describe the desired pipelines in detail, including the required data structure, bindings, shaders, and resource layouts, then create pipelines from them. Our basic demos only contain a single pipeline, but non-trivial apps will usually contain multiple pipelines for different purposes.
5. [Run a compute/rendering pass](#running_a_rendering_pass): This involves a number of substeps:
   1. Create a command encoder that can encode a set of commands to be passed to the GPU to execute.
   2. Create a pass encoder object on which compute/render commands are issued.
   3. Run commands to specify which pipelines to use, what buffer(s) to get the required data from, how many drawing operations to run (in the case of render pipelines), etc.
   4. Finalize the command list and encapsulate it in a command buffer.
   5. Submit the command buffer to the GPU via the logical device's command queue.

In the sections below, we will examine a basic render pipeline demo, to allow you to explore what it requires. Later on, we'll also examine a [basic compute pipeline](#basic_compute_pipeline) example, looking at how it differs from the render pipeline.

## Basic render pipeline

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/) we give a `<canvas>` element a solid blue background and draw a triangle onto it.

### Create shader modules

We are using the following shader code. The vertex shader stage (`@vertex` block) accepts a chunk of data containing a position and a color, positions the vertex according to the given position, interpolates the color, then passes the data along to the fragment shader stage. The fragment shader stage (`@fragment` block) accepts the data from the vertex shader stage and colors the vertex according to the given color.

```js
const shaders = `
struct VertexOut {
  @builtin(position) position : vec4f,
  @location(0) color : vec4f
}

@vertex
fn vertex_main(@location(0) position: vec4f,
               @location(1) color: vec4f) -> VertexOut
{
  var output : VertexOut;
  output.position = position;
  output.color = color;
  return output;
}

@fragment
fn fragment_main(fragData: VertexOut) -> @location(0) vec4f
{
  return fragData.color;
}
`;
```

> **Note:** In our demos we are storing our shader code inside a template literal, but you can store it anywhere from which it can easily be retrieved as text to be fed into your WebGPU program. For example, another common practice is to store shaders inside a {{htmlelement("script")}} element and retrieve the contents using {{domxref("Node.textContent")}}. The correct mime type to use for WGSL is `text/wgsl`.

To make your shader code available to WebGPU, you have to put it inside a {{domxref("GPUShaderModule")}} via a {{domxref("GPUDevice.createShaderModule()")}} call, passing your shader code as a property inside a descriptor object. For example:

```js
const shaderModule = device.createShaderModule({
  code: shaders,
});
```

### Get and configure the canvas context

In a render pipeline, we need to specify somewhere to render the graphics to. In this case we are getting a reference to an onscreen `<canvas>` element then calling {{domxref("HTMLCanvasElement.getContext()")}} with a parameter of `webgpu` to return its GPU context (a {{domxref("GPUCanvasContext")}} instance).

From there, we configure the context with a call to {{domxref("GPUCanvasContext.configure()")}}, passing it an options object containing the {{domxref("GPUDevice")}} that the rendering information will come from, the format the textures will have, and the alpha mode to use when rendering semi-transparent textures.

```js
const canvas = document.querySelector("#gpuCanvas");
const context = canvas.getContext("webgpu");

context.configure({
  device: device,
  format: navigator.gpu.getPreferredCanvasFormat(),
  alphaMode: "premultiplied",
});
```

> **Note:** The best practice for determining the texture format is to use the {{domxref("GPU.getPreferredCanvasFormat()")}} method; this selects the most efficient format (either `bgra8unorm` or `rgba8unorm`) for the user's device.

### Create a buffer and write our triangle data into it

Next we will provide our WebGPU program with our data, in a form it can use. Our data is initially provided in a {{jsxref("Float32Array")}}, which contains 8 data points for each triangle vertex ‚Äî X, Y, Z, W for position, and R, G, B, A for color.

```js
const vertices = new Float32Array([
  0.0, 0.6, 0, 1, 1, 0, 0, 1, -0.5, -0.6, 0, 1, 0, 1, 0, 1, 0.5, -0.6, 0, 1, 0,
  0, 1, 1,
]);
```

However, we've got an issue here. We need to get our data into a {{domxref("GPUBuffer")}}. Behind the scenes, this type of buffer is stored in memory very tightly integrated with the GPU's cores to allow for the desired high performance processing. As a side effect, this memory can't be accessed by processes running on the host system, like the browser.

The {{domxref("GPUBuffer")}} is created via a call to {{domxref("GPUDevice.createBuffer()")}}. We give it a size equal to the length of the `vertices` array so it can contain all the data, and `VERTEX` and `COPY_DST` usage flags to indicate that the buffer will be used as a vertex buffer and the destination of copy operations.

```js
const vertexBuffer = device.createBuffer({
  size: vertices.byteLength, // make it big enough to store vertices in
  usage: GPUBufferUsage.VERTEX | GPUBufferUsage.COPY_DST,
});
```

We could handle getting our data into the `GPUBuffer` using a mapping operation, like we use in the [compute pipeline example](#basic_compute_pipeline) to read data from the GPU back to JavaScript. However, in this case we are going to use the handy {{domxref("GPUQueue.writeBuffer()")}} convenience method, which takes as its parameters the buffer to write to, the data source to write from, an offset value for each, and the size of data to write (we've specified the whole length of the array). The browser then works out the most efficient way to handle writing the data.

```js
device.queue.writeBuffer(vertexBuffer, 0, vertices, 0, vertices.length);
```

### Define and create the render pipeline

Now we've got our data into a buffer, the next part of the setup is to actually create our pipeline, ready to be used for rendering.

First of all, we create an object that describes the required layout of our vertex data. This perfectly describes what we saw earlier on in our `vertices` array and vertex shader stage ‚Äî each vertex has position and color data. Both are formatted in `float32x4` format (which maps to the WGSL `vec4<f32>` type), and the color data starts at an offset of 16 bytes into each vertex. `arrayStride` specifies the stride, meaning the number of bytes making up each vertex, and `stepMode` specifies that the data should be fetched per-vertex.

```js
const vertexBuffers = [
  {
    attributes: [
      {
        shaderLocation: 0, // position
        offset: 0,
        format: "float32x4",
      },
      {
        shaderLocation: 1, // color
        offset: 16,
        format: "float32x4",
      },
    ],
    arrayStride: 32,
    stepMode: "vertex",
  },
];
```

Next, we create a descriptor object that specifies the configuration of our render pipeline stages. For both the shader stages, we specify the {{domxref("GPUShaderModule")}} that the relevant code can be found in (`shaderModule`), and the name of the function that acts as the entry point for each stage.

In addition, in the case of the vertex shader stage we provide our `vertexBuffers` object to provide the expected state of our vertex data. And in the case of our fragment shader stage, we provide an array of color target states that indicate the specified rendering format (this matches the format specified in our canvas context config earlier).

We also specify a `primitive` state, which in this case just states the type of primitive we will be drawing, and a `layout` of `auto`. The `layout` property defines the layout (structure, purpose, and type) of all the GPU resources (buffers, textures, etc.) used during the execution of the pipeline. In more complex apps, this would take the form of a {{domxref("GPUPipelineLayout")}} object, created using {{domxref("GPUDevice.createPipelineLayout()")}} (you can see an example in our [Basic compute pipeline](#basic_compute_pipeline)), which allows the GPU to figure out how to run the pipeline most efficiently ahead of time. Here however we are specifying the `auto` value, which will cause the pipeline to generate an implicit bind group layout based on any bindings defined in the shader code.

```js
const pipelineDescriptor = {
  vertex: {
    module: shaderModule,
    entryPoint: "vertex_main",
    buffers: vertexBuffers,
  },
  fragment: {
    module: shaderModule,
    entryPoint: "fragment_main",
    targets: [
      {
        format: navigator.gpu.getPreferredCanvasFormat(),
      },
    ],
  },
  primitive: {
    topology: "triangle-list",
  },
  layout: "auto",
};
```

Finally, we can create a {{domxref("GPURenderPipeline")}} based on our `pipelineDescriptor` object, by passing it in as a parameter to a {{domxref("GPUDevice.createRenderPipeline()")}} method call.

```js
const renderPipeline = device.createRenderPipeline(pipelineDescriptor);
```

### Running a rendering pass

Now that all the setup is done, we can actually run a rendering pass and draw something onto our `<canvas>`. To encode any commands to be later issued to the GPU, you need to create a {{domxref("GPUCommandEncoder")}} instance, which is done using a {{domxref("GPUDevice.createCommandEncoder()")}} call.

```js
const commandEncoder = device.createCommandEncoder();
```

Next up we start the rendering pass running by creating a {{domxref("GPURenderPassEncoder")}} instance with a {{domxref("GPUCommandEncoder.beginRenderPass()")}} call. This method takes a descriptor object as a parameter, the only mandatory property of which is a `colorAttachments` array. In this case, we specify:

1. A texture view to render into; we create a new view from the `<canvas>` via {{domxref("GPUTexture.createView", "context.getCurrentTexture().createView()")}}.
2. That the view should be "cleared" to a specified color once loaded and before any drawing takes place. This is what causes the blue background behind the triangle.
3. That the value of the current rendering pass should be stored for this color attachment.

```js
const clearColor = { r: 0.0, g: 0.5, b: 1.0, a: 1.0 };

const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
};

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);
```

Now we can invoke methods of the rendering pass encoder to draw our triangle:

1. {{domxref("GPURenderPassEncoder.setPipeline()")}} is called with our `renderPipeline` object as a parameter to specify the pipeline to use for the rendering pass.
2. {{domxref("GPURenderPassEncoder.setVertexBuffer()")}} is called with our `vertexBuffer` object as a parameter to act as the data source to pass to the pipeline to render. The first parameter is the slot to set the vertex buffer for, and is a reference to the index of the element in the `vertexBuffers` array which describes this buffer's layout.
3. {{domxref("GPURenderPassEncoder.draw()")}} sets the drawing in motion. There is data for three vertices inside our `vertexBuffer`, so we set a vertex count value of `3` to draw them all.

```js
passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);
```

To finish encoding the sequence of commands and issue them to the GPU, three more steps are needed.

1. We invoke the {{domxref("GPURenderPassEncoder.end()")}} method to signal the end of the render pass command list.
2. We invoke the {{domxref("GPUCommandEncoder.finish()")}} method to complete recording of the issued command sequence and encapsulate it into a {{domxref("GPUCommandBuffer")}} object instance.
3. We submit the {{domxref("GPUCommandBuffer")}} to the device's command queue (represented by a {{domxref("GPUQueue")}} instance) to be sent to the GPU. The device's queue is available via the {{domxref("GPUDevice.queue")}} property, and an array of {{domxref("GPUCommandBuffer")}} instances can be added to the queue via a {{domxref("GPUQueue.submit()")}} call.

These three steps can be achieved via the following two lines:

```js
passEncoder.end();

device.queue.submit([commandEncoder.finish()]);
```

## Basic compute pipeline

In our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/), we get the GPU to calculate some values, store them in an output buffer, copy the data across to a staging buffer, then map that staging buffer so that the data can be read out to JavaScript and logged to the console.

The app follows a similar structure to the basic rendering demo. We create a {{domxref("GPUDevice")}} reference in the same way as before, and encapsulate our shader code into a {{domxref("GPUShaderModule")}} via a {{domxref("GPUDevice.createShaderModule()")}} call. The difference here is that our shader code only has one shader stage, a `@compute` stage:

```js
// Define global buffer size
const BUFFER_SIZE = 1000;

const shader = `
@group(0) @binding(0)
var<storage, read_write> output: array<f32>;

@compute @workgroup_size(64)
fn main(
  @builtin(global_invocation_id)
  global_id : vec3u,

  @builtin(local_invocation_id)
  local_id : vec3u,
) {
  // Avoid accessing the buffer out of bounds
  if (global_id.x >= ${BUFFER_SIZE}) {
    return;
  }

  output[global_id.x] =
    f32(global_id.x) * 1000. + f32(local_id.x);
}
`;
```

### Create buffers to handle our data

In this example we create two {{domxref("GPUBuffer")}} instances to handle our data, an `output` buffer to write the GPU calculation results to at high speed, and a `stagingBuffer` that we'll copy the `output` contents to, which can be mapped to allow JavaScript to access the values.

- `output` is specified as a storage buffer that will be the source of a copy operation.
- `stagingBuffer` is specified as a buffer that can be mapped for reading by JavaScript, and will be the destination of a copy operation.

```js
const output = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.STORAGE | GPUBufferUsage.COPY_SRC,
});

const stagingBuffer = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.MAP_READ | GPUBufferUsage.COPY_DST,
});
```

### Create a bind group layout

When the pipeline is created, we specify a bind group to use for the pipeline. This involves first creating a {{domxref("GPUBindGroupLayout")}} (via a call to {{domxref("GPUDevice.createBindGroupLayout()")}}) that defines the structure and purpose of GPU resources such as buffers that will be used in this pipeline. This layout is used as a template for bind groups to adhere to. In this case we give the pipeline access to a single memory buffer, tied to binding slot 0 (this matches the relevant binding number in our shader code ‚Äî `@binding(0)`), usable in the compute stage of the pipeline, and with the buffer's purpose defined as `storage`.

```js
const bindGroupLayout = device.createBindGroupLayout({
  entries: [
    {
      binding: 0,
      visibility: GPUShaderStage.COMPUTE,
      buffer: {
        type: "storage",
      },
    },
  ],
});
```

Next we create a {{domxref("GPUBindGroup")}} by calling {{domxref("GPUDevice.createBindGroup()")}}. We pass this method call a descriptor object that specifies the bind group layout to base this bind group on, and the details of the variable to bind to the slot defined in the layout. In this case, we are declaring binding 0, and specifying that the `output` buffer we defined earlier should be bound to it.

```js
const bindGroup = device.createBindGroup({
  layout: bindGroupLayout,
  entries: [
    {
      binding: 0,
      resource: {
        buffer: output,
      },
    },
  ],
});
```

> **Note:** You could retrieve an implicit layout to use when creating a bind group by calling the {{domxref("GPUComputePipeline.getBindGroupLayout()")}} method. There is also a version available for render pipelines: see {{domxref("GPURenderPipeline.getBindGroupLayout()")}}.

### Create a compute pipeline

With the above all in place, we can now create a compute pipeline by calling {{domxref("GPUDevice.createComputePipeline()")}}, passing it a pipeline descriptor object. This works in a similar way to creating a render pipeline. We describe the compute shader, specifying what module to find the code in and what the entry point is. We also specify a `layout` for the pipeline, in this case creating a layout based on the `bindGroupLayout` we defined earlier via a {{domxref("GPUDevice.createPipelineLayout()")}} call.

```js
const computePipeline = device.createComputePipeline({
  layout: device.createPipelineLayout({
    bindGroupLayouts: [bindGroupLayout],
  }),
  compute: {
    module: shaderModule,
    entryPoint: "main",
  },
});
```

One difference here from the render pipeline layout is that we are not specifying a primitive type, as we are not drawing anything.

### Running a compute pass

Running a compute pass is similar in structure to running a rendering pass, with some different commands. For a start, the pass encoder is created using {{domxref("GPUCommandEncoder.beginComputePass()")}}.

When issuing the commands, we specify the pipeline to use in the same way as before, using {{domxref("GPUComputePassEncoder.setPipeline()")}}. We then however use {{domxref("GPUComputePassEncoder.setBindGroup()")}} to specify that we want to use our `bindGroup` to specify the data to use in the calculation, and {{domxref("GPUComputePassEncoder.dispatchWorkgroups()")}} to specify the number of GPU workgroups to use to run the calculations.

We then signal the end of the render pass command list using {{domxref("GPURenderPassEncoder.end()")}}.

```js
passEncoder.setPipeline(computePipeline);
passEncoder.setBindGroup(0, bindGroup);
passEncoder.dispatchWorkgroups(Math.ceil(BUFFER_SIZE / 64));

passEncoder.end();
```

### Reading the results back to JavaScript

Before submitting the encoded commands to the GPU for execution using {{domxref("GPUQueue.submit()")}}, we copy the contents of the `output` buffer to the `stagingBuffer` buffer using {{domxref("GPUCommandEncoder.copyBufferToBuffer()")}}.

```js
// Copy output buffer to staging buffer
commandEncoder.copyBufferToBuffer(
  output,
  0, // Source offset
  stagingBuffer,
  0, // Destination offset
  BUFFER_SIZE,
);

// End frame by passing array of command buffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);
```

Once the output data is available in the `stagingBuffer`, we use the {{domxref("GPUBuffer.mapAsync()")}} method to map the data to intermediate memory, grab a reference to the mapped range using {{domxref("GPUBuffer.getMappedRange()")}}, copy the data into JavaScript, and then log it to the console. We also unmap the `stagingBuffer` once we are finished with it.

```js
// map staging buffer to read results back to JS
await stagingBuffer.mapAsync(
  GPUMapMode.READ,
  0, // Offset
  BUFFER_SIZE, // Length
);

const copyArrayBuffer = stagingBuffer.getMappedRange(0, BUFFER_SIZE);
const data = copyArrayBuffer.slice();
stagingBuffer.unmap();
console.log(new Float32Array(data));
```

## GPU error handling

WebGPU calls are validated asynchronously in the GPU process. If errors are found, the problem call is marked as invalid on the GPU side. If another call is made that relies on the return value of an invalidated call, that object will also be marked as invalid, and so on. For this reason, errors in WebGPU are referred to as "contagious".

Each {{domxref("GPUDevice")}} instance maintains its own error scope stack. This stack is initially empty, but you can start pushing an error scope to the stack by invoking {{domxref("GPUDevice.pushErrorScope()")}} to capture errors of a particular type.

Once you are done capturing errors, you can end capture by invoking {{domxref("GPUDevice.popErrorScope()")}}. This pops the scope from the stack and returns a {{jsxref("Promise")}} that resolves to an object ({{domxref("GPUInternalError")}}, {{domxref("GPUOutOfMemoryError")}}, or {{domxref("GPUValidationError")}}) describing the first error captured in the scope, or `null` if no errors were captured.

We have attempted to provide useful information to help you understand why errors are occurring in your WebGPU code in "Validation" sections where appropriate, which list criteria to meet to avoid errors. See for example the [`GPUDevice.createBindGroup()` Validation section](/en-US/docs/Web/API/GPUDevice/createBindGroup#validation). Some of this information is complex; rather than repeat the spec, we have decided to just list error criteria that are:

- Non-obvious, for example combinations of descriptor properties that produce validation errors. There is no point telling you to make sure you use the correct descriptor object structure. That is both obvious and vague.
- Developer-controlled. Some of the error criteria are purely based on internals and not really relevant to web developers.

You can find more information about WebGPU error handling in the explainer ‚Äî see [Object validity and destroyed-ness](https://gpuweb.github.io/gpuweb/explainer/#invalid-and-destroyed) and [Errors](https://gpuweb.github.io/gpuweb/explainer/#errors). [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling) provides useful real-world examples and advice.

> **Note:** The historic way of handling errors in WebGL is to provide a {{domxref("WebGLRenderingContext.getError", "getError()")}} method to return error information. This is problematic in that it returns errors synchronously, which is bad for performance ‚Äî each call requires a round-trip to the GPU and requires all previously issued operations to be finished. Its state model is also flat, meaning that errors can leak between unrelated code. The creators of WebGPU were determined to improve on this.

## Interfaces

### Entry point for the API

- {{domxref("Navigator.gpu")}} / {{domxref("WorkerNavigator.gpu")}}
  - : The entry point for the API ‚Äî returns the {{domxref("GPU")}} object for the current context.
- {{domxref("GPU")}}
  - : The starting point for using WebGPU. It can be used to return a {{domxref("GPUAdapter")}}.
- {{domxref("GPUAdapter")}}
  - : Represents a GPU adapter. From this you can request a {{domxref("GPUDevice")}}, adapter info, features, and limits.
- {{domxref("GPUAdapterInfo")}}
  - : Contains identifying information about an adapter.

### Configuring GPUDevices

- {{domxref("GPUDevice")}}
  - : Represents a logical GPU device. This is the main interface through which the majority of WebGPU functionality is accessed.
- {{domxref("GPUSupportedFeatures")}}
  - : A [setlike](/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set) object that describes additional functionality supported by a {{domxref("GPUAdapter")}} or {{domxref("GPUDevice")}}.
- {{domxref("GPUSupportedLimits")}}
  - : Describes the limits supported by a {{domxref("GPUAdapter")}} or {{domxref("GPUDevice")}}.

### Configuring a rendering `<canvas>`

- {{domxref("HTMLCanvasElement.getContext()")}} ‚Äî the `"webgpu"` `contextType`
  - : Invoking `getContext()` with the `"webgpu"` `contextType` returns a {{domxref("GPUCanvasContext")}} object instance, which can then be configured with {{domxref("GPUCanvasContext.configure()")}}.
- {{domxref("GPUCanvasContext")}}
  - : Represents the WebGPU rendering context of an {{htmlelement("canvas")}} element.

### Representing pipeline resources

- {{domxref("GPUBuffer")}}
  - : Represents a block of memory that can be used to store raw data to use in GPU operations.
- {{domxref("GPUExternalTexture")}}
  - : A wrapper object containing an {{domxref("HTMLVideoElement")}} snapshot that can be used as a texture in GPU rendering operations.
- {{domxref("GPUSampler")}}
  - : Controls how shaders transform and filter texture resource data.
- {{domxref("GPUShaderModule")}}
  - : A reference to an internal shader module object, a container for WGSL shader code that can be submitted to the GPU to execution by a pipeline.
- {{domxref("GPUTexture")}}
  - : A container used to store 1D, 2D, or 3D arrays of data, such as images, to use in GPU rendering operations.
- {{domxref("GPUTextureView")}}
  - : A view onto some subset of the texture subresources defined by a particular {{domxref("GPUTexture")}}.

### Representing pipelines

- {{domxref("GPUBindGroup")}}
  - : Based on a {{domxref("GPUBindGroupLayout")}}, a `GPUBindGroup` defines a set of resources to be bound together in a group and how those resources are used in shader stages.
- {{domxref("GPUBindGroupLayout")}}
  - : Defines the structure and purpose of related GPU resources such as buffers that will be used in a pipeline, and is used as a template when creating {{domxref("GPUBindGroup")}}s.
- {{domxref("GPUComputePipeline")}}
  - : Controls the compute shader stage and can be used in a {{domxref("GPUComputePassEncoder")}}.
- {{domxref("GPUPipelineLayout")}}
  - : Defines the {{domxref("GPUBindGroupLayout")}}s used by a pipeline. {{domxref("GPUBindGroup")}}s used with the pipeline during command encoding must have compatible {{domxref("GPUBindGroupLayout")}}s.
- {{domxref("GPURenderPipeline")}}
  - : Controls the vertex and fragment shader stages and can be used in a {{domxref("GPURenderPassEncoder")}} or {{domxref("GPURenderBundleEncoder")}}.

### Encoding and submitting commands to the GPU

- {{domxref("GPUCommandBuffer")}}
  - : Represents a recorded list of GPU commands that can be submitted to a {{domxref("GPUQueue")}} for execution.
- {{domxref("GPUCommandEncoder")}}
  - : Represents a command encoder, used to encode commands to be issued to the GPU.
- {{domxref("GPUComputePassEncoder")}}
  - : Encodes commands related to controlling the compute shader stage, as issued by a {{domxref("GPUComputePipeline")}}. Part of the overall encoding activity of a {{domxref("GPUCommandEncoder")}}.
- {{domxref("GPUQueue")}}
  - : controls execution of encoded commands on the GPU.
- {{domxref("GPURenderBundle")}}
  - : A container for pre-recorded bundles of commands (see {{domxref("GPURenderBundleEncoder")}}).
- {{domxref("GPURenderBundleEncoder")}}
  - : Used to pre-record bundles of commands. These can be reused in {{domxref("GPURenderPassEncoder")}}s via the {{domxref("GPURenderPassEncoder.executeBundles", "executeBundles()")}} method, as many times as required.
- {{domxref("GPURenderPassEncoder")}}
  - : Encodes commands related to controlling the vertex and fragment shader stages, as issued by a {{domxref("GPURenderPipeline")}}. Part of the overall encoding activity of a {{domxref("GPUCommandEncoder")}}.

### Running queries on rendering passes

- {{domxref("GPUQuerySet")}}
  - : Used to record the results of queries on passes, such as occlusion or timestamp queries.

### Debugging errors

- {{domxref("GPUCompilationInfo")}}
  - : An array of {{domxref("GPUCompilationMessage")}} objects, generated by the GPU shader module compiler to help diagnose problems with shader code.
- {{domxref("GPUCompilationMessage")}}
  - : Represents a single informational, warning, or error message generated by the GPU shader module compiler.
- {{domxref("GPUDeviceLostInfo")}}
  - : Returned when the {{domxref("GPUDevice.lost")}} {{jsxref("Promise")}} resolves, providing information as to why the device was lost.
- {{domxref("GPUError")}}
  - : The base interface for errors surfaced by {{domxref("GPUDevice.popErrorScope")}} and the {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event.
- {{domxref("GPUInternalError")}}
  - : One of the types of errors surfaced by {{domxref("GPUDevice.popErrorScope")}} and the {{domxref("GPUDevice")}} {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event. Indicates that an operation failed for a system or implementation-specific reason, even when all validation requirements were satisfied.
- {{domxref("GPUOutOfMemoryError")}}
  - : One of the types of errors surfaced by {{domxref("GPUDevice.popErrorScope")}} and the {{domxref("GPUDevice")}} {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event. Indicates that there was not enough free memory to complete the requested operation.
- {{domxref("GPUPipelineError")}}
  - : Describes a pipeline failure. The value received when a {{jsxref("Promise")}} returned by a {{domxref("GPUDevice.createComputePipelineAsync()")}} or {{domxref("GPUDevice.createRenderPipelineAsync()")}} call rejects.
- {{domxref("GPUUncapturedErrorEvent")}}
  - : The event object type for the {{domxref("GPUDevice")}} {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event.
- {{domxref("GPUValidationError")}}
  - : One of the types of errors surfaced by {{domxref("GPUDevice.popErrorScope")}} and the {{domxref("GPUDevice")}} {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event. Describes an application error indicating that an operation did not pass the WebGPU API's validation constraints.

## Security requirements

The whole API is available only in a [secure context](/en-US/docs/Web/Security/Secure_Contexts).

## Examples

- [Basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/)
- [Basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/)
- [WebGPU samples](https://webgpu.github.io/webgpu-samples/)

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [WebGPU best practices](https://toji.dev/webgpu-best-practices/)
- [WebGPU explainer](https://gpuweb.github.io/gpuweb/explainer)
- [WebGPU ‚Äî All of the cores, none of the canvas](https://surma.dev/things/webgpu/)
-e 

File: /files/en-us/web/api/webgpu_api/basic-webgpu-stack.png
âPNG

   
IHDR  ˇ     KÑò   PLTEˇˇˇ   ˙˙˙ˆˆˆöööiii@@@¸¸¸“““ççç’’’MMM"""ZZZÚÚÚwwwccc^^^äääBBBﬂﬂﬂŒŒŒ&&&ÇÇÇlllUUUÎÎÎGGGEEE‚‚‚:::ÂÂÂttt¢¢¢...≈≈≈±±≤ÔÔÔïîïfffËËËííí***∂∂∂óóóqqq222ÀÀÀèèè∫∫∫ûûû´´´⁄⁄⁄555¡¡¡áááQQQßßßyyyΩΩΩ»»»|||ooo===ÿÿÿÑÑÑKKK‹‹‹¥¥¥§§§ÆÆÆ‰‰‰XWX""#»aw˛  ˜IDATx⁄ÏùÎR⁄PFøÌ!»Mî(®U)Ç‘⁄¢µwÌÂ˝ﬂ¶ë^f:#í†—ìsæıã…ü5{Øa2ìÃú@àÕ@@ÏÖ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌÜ˝ÌFõ˛Ój˘‘ìá∆;-Ø:ÙÍﬂøßZ√C<<á√ñﬂ•W˜˛/FàèBS?o±xì÷ˇ≈[ƒI£IØŒ˝{#ƒÀj˜voˇc∏W”˛éB‹¯9zµÌø⁄B‹
Ùj€ø<D‹\ñü»[”h^]˚ü"nˆNÈ’∂øá¯ÒË’∂ø ~Ñ^ˆ∑‹À˛v{Ÿﬂn/˚€ÌeªΩÏo∑ó˝Ìˆ≤ø›^ˆ∑€À˛v{Ÿﬂn/˚€ÌMVˇJ˛9Äz@.øá?\>_–Ao¬˙/À@VÍ¿∫ÙG::ËMX§&¿kë4–ó¸Ω˜Ao“˙◊–WÂ	PV9úx©Ié4<µñ«îÂLv˜¬¡u¶◊.ΩÕ°Zdè;Û—ΩÎ∑x›GÊCxÕÌø/üP¨ÌãÉT
Ôd≠ø&Øë‚íR8GÈÇ§—êçnSFd;Ω-√ŸéËﬁÚ˝ΩÕõ∞˛uª≤ø#oÇÿmÆZr$»>ûÛ@q
Y6≥R.‹‘ Gúﬁ ^çÊMXîVﬁ…wlº?ózN⁄’j5µ9Ω:“¿t!˝Ê3πŸÄæ∏ﬁ¿Ê«z◊?S∫8Z«Õ,*rú	Ë:Ú
»©È>*J≠÷Ç}î Ù§‚e œf8·≠.‡5∑ˇ+QU‡DTPõ ∫W”ø¬≤\# -y‡f‚≈,ºèÄ£Vf8ËM\ˇCë¿yTe\o»ï\⁄)´
:“Ÿ…Æ”êÃN_Z$]H'¥cqÔUúﬁ ,Ô’ÌÛö€mq¨…!Pôà»)ä®‹‡lãú}ñãÜjãl∫⁄J‘RH«˝Ω’ƒy◊ˇ?vÜ[∏¡˝‰¸ª¥lU%ºﬁ‡eúew¶√LØcÛü∞˚ò‚eÓr–kjˇ—.¶L™w9Ë5µ‚ﬁ√Ú˝Ø˚∞ÕÀ˛v{Ÿﬂn/˚€ÌeªΩÏo∑ó˝Ìˆ≤ø›^ˆ∑€À˛v{Ÿﬂn/˚€ÌeªΩ∫ˆ∑ÌNûˇ©«y∏∂yuÌ_"njÙj€ˇŒ√ˇ0zÔ@'ØÆ˝q#9zµÌènÏﬂ√È”´q4àì˜zµÓèÊ*‚cu@ØÊ˝—ıó{xxˆ“Ô-Ω∫ˆGÆPãÁ{∏£‹›ﬁë]^]˚GaúFË5¥øÔ#ÙöŸøÁ˚Ô1z
ÌØDÛ°◊Ã˛c%‚∑0z
Ìü_â∏òCL^ÛH‘º…ÎÆT˚ÿ˜3òCﬁ∂qﬁ‰ıvñOø®¥é\‹	ΩÜˆﬂ∆+@èL‡MáÒ&kﬁ‰ı◊z
ÌønÙ⁄ˇ∫å0–khˇÛΩÜˆµâ0–khˇoÑÅ^C˚wäΩÜˆø˙Ç0–khˇó€ΩÜˆ?yÜ0–´_!Oá˝Ò º˘à»–c˙Ï"2Ùö”ˇrÅ}–kNˇ·"CØ9˝◊èzÕÈüo„IX_¿´—ºÏ_ÔB¬˛qˆ_^†ΩÊÙˇ¥Å»–kNˇØ?z
ÈÔıg1ØFÛö—?˝≥≥ì≈g5ƒ£xØûƒ;˛Îeˇ)IïîÚ≥àΩÜÙGFDâ:G4Ë5•ø#)DÑ^S˙£Âã?FDË5¶?D¢BØ9˝ó¸¢BØ9˝±w¶Mâca}oDdDP‹Ì∂ÁˇˇõI‚2SéˆLßCôãÔ˘íÓ∫VùzÔ)≠h4◊ ò¯Lﬁ ÕË˛V69ü˜·eM8à7–˝Tu–Üˇ¥’Õlƒ‰˛˚Gò±ÄÄycòÆW∑˛˚SÃì≠ ﬁ‡ˆ?ò˚˚[î˜sƒıÍ‘ﬂTò7õÒ˙’?bô¯Âãx‰˙“y8± ù√Û	Û˛rˇã∞9°rboê7Ô2ÑWjä§∫ã¬fLUÈ»sº}„˚îÛ∞f…OÚf4ÔØÙèS¡¶H6 úqÔˆœêÖVØN^ Ë≥òNg∆‰ô”ˇÒ˝˛:Ô´y•?é ì‰Ä≥Ôˆ?cø¸t≠ª˝7û˛ìˇIˇ ùá˘’ºø‘?√0·« : ì‚üïÀ¶”øuﬁ1V£Ä•8ÄÀ∂qÛ⁄ﬂ"#ˇÏÿÛp≈˚ì˛5ÓKúú≤çïâ≤ûg˛]í◊}2á8+xÂµˇê§ø&ﬁ˚óôpäö!û°À"⁄T
`âUß»r{Ã H≈J@ü{π‹dö`U˙Î‚˝∞?lÔÚÃ‡ú!∞ ¿¢Å.ó4I≥≈s C:l9˝üXoJ]º˜/pÔC@BE*°¿Œ™
ivyõ1ÀCf ‹ƒb±‚Sˇs˚ü°I@áe81´’~|5Ô«˝˜∏ñ‰=–„Ña†»Œéãı|ˇÕ«(˚xb˙‘/¨Û=Ü~o?ÓÔÒ•(ﬁPæ˜µÉwµVÛ~‹øƒæJ Ërù˚¿[∞›†ÀÍÛ]~ä¿!Ry€?√)*Ï˛ﬁ~¨Ô‡=Bƒ“€æˆ˜Æ÷jﬁè˚cLˆ §HÅ!w Dyç.√M‡ò´¿î˝G'ˇîo˚ôh¯N¶Ê≤•‹ú˚{Wk5ÔO˙_í]ÿÏêm 2Ê˛C»`]r|SúVû∆rÎ∂¬˛€˛Ê)√’lë¨˘¥èE>∑Är1ü>I£{L*™ÿ∫Ec;‰wÔjΩÊ˝IˇãÁœ›Î∞Ÿ›&⁄~ÆÖIÓ¡&U•M¯“T∑Ó!^±2¥1N|⁄+‹˘c⁄æÊßQnáV8∫Á]≠¿∏ø˝Ω´5õó ˛/«3OƒsÊKÁ‹Ò.ﬁ≈å€+~ÌGçQ ∆ˆ	G@››èåa°©jçS¶ ˙ŸﬂªZªyÉ¸ˇˇÏGUEÄ’0Äsw?Íßpe”uN˝ÍÔM≠Ìº∫ÙOw L8€wÆ1w?åe84òø:Qæı˜¶÷v^]˙o±q˜÷π›˝XÈ ©˛0iX∞Ë[ojmÁ
~ˇ¸7õá8´©õƒ*¢,ŒéËÓ«	ónñ9™™˚ç/#>ı˜¶÷vﬁ‡˜ßC!í„2PSL√fÅÃ◊0 ìôª>ı˜¶÷vﬁ¿˜%5(h7"÷N·“‹ÄCº	Ïöﬁºæ®5ûWü˛OlpÎf»Éπ{?V/÷º∫ıG®C„|Óﬁè’6Øv˝Å‘Áx]ı¬Õ´aÒ~Ω˛÷ÃzÁÅ∏^oÍ≈ôWì˛|;~àæxΩ©g^m˚óræxΩ©g^
˙[W˘Ì£H]ÂÎ∑f˘zDÓZ›;`cU≠¥º‡ÕÎãZ„y5Ë_d&CFq≠.oπå¸6–‡$DÁŸx(Õoœﬁºæ®5û7¯˝Gúóåsà±9eU#"NVˆ_<y˝QÎ;o˚9 .ÕÚjm≠»Ë=á„!¢™‡≤‡…ÎèZﬂyÉﬂˇÑª@é—s.;l†íú1éëN¿·e¡ì◊µæÛøˇø-FCå—•y’B|zFû\{Y‰ıG≠Ôº¡ÔoïÚEÇ—]ÆFèÎ}†M∏˚q√”Ë!kœﬁºæ®5û7¯˝—PdÅQÏ)2p«]w?P#çµ»ÛÇ7Ø/jçÁ’†?¨\È˘èºYE^<z˝PÎ<Ø˝≈˚ÂüˇàW˙ãW˙ãW˙ãW˙ãW˙ãW˙ãw˙µ˜pjÒ˛Oˇê˜ˇƒ‘˛…ÊM##ﬁ¿ˆœV1oÆéƒÿ˛Ê&Ê
#‚
l¥Ê~œ!ƒ‹˛(laû\ˆ Ò∏?
YÃèlÄxÉ‹≠Õﬁl˛≥€∏‚!lƒË˛àƒ2Û9˜(Òªø_,ˆ˘ﬂ¬øê˛ÇÙ§ø ˝È/HA˙“_ê˛ÇÙ§ø ˝È/HA˙“_ê˛Ç6˝≠lÚè
ø˝˚YS«˛™:hC¯]⁄ÉÍfKø˛˚1~+Ë÷
¡?∂
zı?êœ~…∂tÍo)˛≤©”ﬂˇf´¸•”®r ¡_fIç˙ˇ!ﬂ¯Ω%ﬂˇ≥·|π˜…œÑﬂ≈ﬁˇ'˝m§ø ˝È/HA˙“_ê˛ÇÙ§ø ˝?ÀÇÜHœ‹ê5¸ME·]öe¡E˙{Êí‹˘˝óGpë˛^1
e∞,˝ˇÊkıÔ≤w…,étínˇn!—ÔV≤µW4÷Ä¥¡Î,PﬁÔt
q Èj43F`ê˛^)re6g‰8L*†F^_ì{híLT»NÎK»)c™	`(≈ÉÙ˜H…iüg∞à®Ä∆Å3Ó;˝◊Ä	UÍÈÎÖ!«¨˚∫!î˛i1LŸÜºê¢ˆˆ 3ÈÙ∑ 9s˚ÁòáÕ:G0ÿ@Äê˛©3s~^§2qÀ!l˙
@¥∑¶€øõ)œ‹˛C´6'0TB˙{#«g∫ËÒÏÂ˛ˇYŸœ∫˝Wa”‚–ÌHc«e #å !˝Ω—c´d”‚
6Ü¬å™
ƒ›˛˘ßè π˝ª<ÖÕn‹î˛—ﬂRl¬¶D6Lò¿æ3	`…Ìœ–TLπ˝À§Xa¶§ˇBÙˇŒ"\ÓxÇmn[§¬à<8KíıAì’Íå[,cç◊√·òÁê˛—ˇî{p©q•míÈS§qú·jì„
…¥	ƒÛ¸´Jõ[KˇËˇÜ—q.ëŸ=Ä˚Rì´xº(√•l(]LJ“.8˝µ@˙?#˝•ˇ_Ï›¡JÇQÜ·Ô)“¬¿BW˛·*⁄î˜M]¿ èyﬂçp\¸3„∫Ó≤ˇ⁄·_;¸káÌØ˛µ√øv¯◊ˇ⁄·_;¸káÌú¸Ÿˇ˘SÕ˝üÏˇ˝≠‚˛_ˆÔ∏1ÚgˇˇÆ#ˇªç≠9›ˇ–â˚?cõŒN˜§Ììh\≥◊˝/i;âF5Õn˜ˇ§SÃÔ{Q∂˝Ò⁄Œ~˜?•’√Ü˚ø#Óˇ^Vé˜-Z.Â˛…¬˚è*˛πﬁ"¨Ô„ü+Z≥ ¯'ük÷ ˇT—"¨ ˛πÁø8Œ ˇLØÎ]Ôªıãl√?”£‘˚◊èm¯'Î&ˇ„ˇ˛¯„è?˛¯„è?˛¯„è?˛¯„è?˛ÓOˇ÷-¯[g˛˛Ö?˛¯„è?˛¯„è?˛¯„O¯˛Ñ?·O¯˛Ñ?·O¯˛üÏ›kS⁄@Ü·Áaì "ê!BP"'(‡-÷:÷ˇˇsö⁄§-¶%eÔ≥Óé.îW≤ÎIˇ›N˙À˘?/∑
˛pˇ˛ó˛“_˙KÈ/˝•øÙó˛“_˙Kˇﬂ$˝•øÙó˛“_˙Ô∞mÍ_Égì˛ÎtÒöˆ˘“y˘¸ø;Í/üˇ{∑˝ÂÛˇÔ∏øº˛«n˚ÀÎˇÏ∏øº˛◊n˚ÀÎˇÌ∏Ø/∑Æø¶˝
ˇ—…$+({G"ªw2ZÀˇ#˚∞Ào2ﬁ‚G"∫∂ˇuyÔj4Ev˛eÒ¡(<)ß÷œÒˆœ¸∑÷\”øØH˙5ã(/ˇ»XœˇÓƒÄlÌåŒ√F¸cô|–L¡™˚⁄å=;˛≈z≥ôã HúÏ'á∂NO€ÎzıŒ‹°QæYáVˆø>Çl#˘RõÇ Ñl ∑‰0H
 c≠
)FÄ"£∂ˇ√ <Çà.j*dpUˇÑ∑]›™ÍõgR√ò:4¡
B9€ﬂ§_Eóe@·≈≥j˚Ôs˚èñøÎP\jbeˇ´èêm¨‹Ÿ&¸k@àAÙi€ƒ)êaVá@aev˚ﬂd_xÀﬂu®  cUˇG≤
6º«øÛ›ˇ]T‡˚∞∫ËS—≠é†à–Ã?≈3¥Ÿ∞˝]áÆÿÉUvEΩ
Ÿ{πyèˇ'MO3àÊårˆUa
¥©ú.m˘ôöÏ±d˚ª˘¯´‡j˛£d-Yyáˇ)èaÁ„ùã≤¡èéµ@ã7∞*ETó?&Ã∞Ä?O ƒπö†
ŸFk‰ﬁ·_"+ é\îFU‡ôER¥ „n?≥<]Ùøg6≠Ëˇ°ŸF+ﬂ·è0Y'pQ‚ò«˝3R úÙ˚Cﬁ¡Ìoêå/˙„âá·WÛœ$!€p±˝w¯#•êCs˛∆1…ƒç ¥Z}Rg7Ï≥◊:x„_êJ*Z^≈ø™C∂·ûûﬂ„ªÉtœ1Õè,‡%ﬁ§©°T&WÒ˜◊!€puˇä˛kgpà7=“–Ê’*˛WWêm∏´´ø„/+|∆€L*ıõ‹—ÛˇYcåÓ5x!üÔÔ¯kÊñTk<	≥sé-Ù◊YVaï¶Wµ¢˙ª!Ü˚&≠Ã>¨ÓËTn®?úx$O±∏≥  ~ñ'˝”6˙?ë©%˛F~3ƒ‡'_√æΩÈÒöâDrè¸‰ÅÛ≤ ,Ï¨≤éü%˝ˇFé??/˜ˇeü)*∞⁄<∑UOa5 œó˙´äPXÊvJˇ≠?·ÒwˇV.z—È	ÖìÍ$ıÄí˛—5Ó‡t√0ú>)ßﬂU1de©ãù¶Äπù“+¸&og˛ß‰dBVq#XˆADQß@õGÆq'¡8¶πTK‰Á•˛y^Ó3ª∞S˙oÖzü¬ò˙nYü˛¸∑˝G, òp‡w∞3® EÏ“∂ÍQ&sŸû"¥Ãﬂ∞Ì≥Ã`nÁ‚*ﬁˆáèâ©µ
†ÀÿˇPêä4]„3‹!Äs⁄ÌŸ™”Ç˚XÊ∆0pÕ‹;ˇó˚E∆<ÓØE9v¸±ﬂŸ“Ì{h∞ÁwÄ#Ø –¬·¡‘?oΩ€h≈'fïôºªÀS®Óù“[¸1f4b˚øíf=5Áˇ»'ò¨π«úkp™L˝OóN8e8´Â⁄È1ˇÒ°àÊ#∏◊Øaï“/g+÷*zËüŒB@K•Ü◊⁄m!xìÒà?íÃS«=≈9ôÛ«ê&·wp:dN>∑ˇ‚‡ƒ¥œ´3æz÷?M°G…bçBT¡¯∑ï÷ÖôFÇ4ÊU¥)$≠UÖ"ÓCê˙Ï;÷7Ôﬂfñ]∏«ú*≥ﬂˇGt˚/N8i≥üYÛ™Äc†«nÿuÓ"˝X)2fØòü°≥j˚ﬂcDh8f≈#˛8µ˝d„6Fñ/qƒ|wÍN*!∏∆f’…d8úg‘Ìø88·Ù¬¸∑œ’Û™ûÅ8‘À"^ |˛±‚¯ﬂ∞`ƒ$⁄| B§ú±∑ı˛˙‘Í@[!ïní:"YæN˝°Ûpç;Ã
˘IÒj‰Å;ﬁ.úp∫aNß<tÌÙ‘ﬂˇ«$ç4†	°™÷Àè«?ÀÇÆÎ¢=ùˇR ¯Èﬂzˇ˘B˜ü|6 5∏Z6Ó†Zè3„•É€”˙˛x<híÏuéGÃπV¡√Ç]mæÿ˛AO˙ˇß≠ÔIEõ¿òπè¨∏Vˇ!3 ‘»ÈøÖ≠Ô/îßÑ!Ç!◊Jëy «k¸H˙oaõ∏ˇ?Á p@πW4ä´Zâºn˘(J“[ﬂﬂH“Í© C¶ÁVrd˜QíÕ
–fı€0xO˙oGÎ˚•jw ª"ıÖïÛís€ﬂ⁄˜‡ﬂw¢µ˝››±ı=˛˚ïΩ{ÎM"ä¬0¸-˜ ßéK¡J+‘§÷ÇJK≠1˛ˇü#S(ööπëeúÕ˙û+í}CÚfdÜµLPÏ_ È&›ˇ7A±ˇª˜≠:˚{Üœˇÿ∆˛∂±ømÏo˚€∆˛∂±ømÏo˚€∆˛∂y’_HùO˝y˝œæ˛Ÿ`bbbbbbbbbbbbbbˇ)íX≥2¬ä{∞øää‘¢®’˘åM/vU≥øRˇ#ÃMúL‡ˆ◊Ïè¨¥ÅËÕVeò∞"dyòÏØ⁄ˇ©HÅsÚ"iEH|ò¢oÏØ⁄y©#ê”oôÑ!À√‘`›˛Cô!ê.WÑƒá)¬˛⁄◊Å+"qEH‡“4˛ó˝u˚?ì⁄b¬a“äê¯0Mÿ_µY∆ã˛I+BÿÉ˚ß‚Íã˛I+BÿC˚//wÛ"],˚'¨aˇçÏIl8˝Äπ|ú8iEHû˝7∞Ç«+B“á˝mc€ÿﬂ6ˆ∑Õß˛ÉHŸ`‡Oˇl§¨óıßˇ˛sê≤Øﬂ¸Èﬂ®ÄîΩ‹Úß?>u@™^Á·Qˇ‹;ê™√kü˙w˘†ÏÂïO˝Ò|§Ë¸^ıüyÒü
Ô¸Íè√mêö‹1<Îèﬁ§§úÉw˝QÂM %”<Ïè''}–⁄:◊Ø‡eÏo@k98˘¥O˚’∑Ìp2+Å˛Bi6©∂á!‡o†[.4ù–_pÕZπ¯›ü÷√˛ƒ˛ƒ˛ƒ˛ƒ˛ƒ˛ƒ˛÷±ømÏo˚€∆˛∂±ømÏo˚€∆˛∂±ømÏo˚€ñ˙˛G—
ü¸[õ+Dg>ˆÔﬂl¨Û…ﬂµïÍŸÌ¬éw˝;˘H…(Ë{÷ñ¢ÕIõ‡Ù¬Ø˛ê¶LÕ´˛„*H’Ì‘ß˛Ó)HU…y‘ˇåÛ’E˙≥ˇä≈˘üúˇ˚ÉÛ9ˇ˚¶Ê≥ˇ˚˚˚˚˚˚˚˚˚˚ˇ7;£+ØnR≥ø¶´˜2◊>«‹XÓΩ=Ã ◊réXCjHˆWî˘>)àTî•EïÇHÿñ/ÏøÒ˝Ôƒu1∑Â§˜ﬂ√‹ÖHü˝MÙøî˜nÉΩU•À˛&˙;)·¡™G‰é˝-Ùﬂë @ÒY¨˜’h|8æë”"˚[Ëﬂê!Äæƒ
qˇÖ¸øˇôËﬂó ¿”0Àã˛≠˘À√£ÄìUˇ]§˚ÎqrÄ{›Eˇ=<∏ïWà}óóHˆ◊Sìp˘F˜ﬂì›Â¡È¬˛z∫Àﬂˇ#y‹ø#üÃI€ﬂóŸ_QO§Ü-yÒ∏?Bë^9…!eÿ_Q1ÎDƒ˝ÿi’Ä±|¡/’ >π."eÿ_UÊ‚hñ–¯ıŸEÍÍ≥øu?€ªcïÜÇ(ä¢WRÜ¿≥ƒVb!VäÇSÊˇHª`aïÅºÀYÎv3≈pè˛ŸÙœ¶6˝≥ÈüMˇl˙g”?õ˛ŸÙœ¶6˝≥ÈüMˇlù˙ªˇyñxˇ”˝ﬂ≥ƒ˚ø„PLv¯Ï”ø6Üü&{Ótˇøæøä©ZÌ‘≤¬îù›>µ⁄ˇ©˚_SΩ›˜Í_/Ô£òd¥€ˇ´z‹mÔNûÅ€ü^∑Àæ›˛ÁØq‹ŸˇΩÿf9éé˚ø¸'eˇõ?ÙGÙGÙGÙGÙGÙGÙGÙGÙgu˝πö5Ùg]Ùœ¶6˝≥ÈüMˇl˙g”?õ˛ŸÙœ¶6˝≥ÈüMˇl˙g”?õ˛ŸÙœ¶∂?Ú≤˝ “Rÿá+{ë    IENDÆB`Ç-e 

File: /files/en-us/web/api/gpuinternalerror/gpuinternalerror/index.md
---
title: "GPUInternalError: GPUInternalError() constructor"
short-title: GPUInternalError()
slug: Web/API/GPUInternalError/GPUInternalError
page-type: web-api-constructor
status:
  - experimental
browser-compat: api.GPUInternalError.GPUInternalError
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUInternalError()`** constructor creates a new
{{domxref("GPUInternalError")}} object instance.

## Syntax

```js-nolint
new GPUInternalError(message)
```

### Parameters

- `message`
  - : A string providing a human-readable message that explains why the error occurred.

## Examples

A developer would not manually use the constructor to create a `GPUInternalError` object. The user agent uses this constructor to create an appropriate object when an internal error is surfaced by {{domxref("GPUDevice.popErrorScope")}} or the {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event.

See the main [`GPUInternalError`](/en-US/docs/Web/API/GPUInternalError#examples) page for an example involving a `GPUInternalError` object instance.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling)
-e 

File: /files/en-us/web/api/gpuinternalerror/index.md
---
title: GPUInternalError
slug: Web/API/GPUInternalError
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUInternalError
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUInternalError`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} describes an application error indicating that an operation did not pass the WebGPU API's validation constraints.

It represents one of the types of errors surfaced by {{domxref("GPUDevice.popErrorScope")}} and the {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event.

Internal errors occur when something happens in the WebGPU implementation that wasn't caught by validation and wasn't clearly identifiable as an out-of-memory error. It generally means that an operation your code performed hit a system limit in a way that was difficult to express with WebGPU's [supported limits](/en-US/docs/Web/API/GPUSupportedLimits). The same operation might succeed on a different device. These can only be raised by pipeline creation, usually if the shader is too complex for the device.

{{InheritanceDiagram}}

## Constructor

- {{domxref("GPUInternalError.GPUInternalError", "GPUInternalError()")}} {{Experimental_Inline}}
  - : Creates a new `GPUInternalError` object instance.

## Instance properties

The `message` property is inherited from its parent, {{domxref("GPUError")}}:

- {{domxref("GPUError.message", "message")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A string providing a human-readable message that explains why the error occurred.

## Examples

The following example uses an error scope to capture a suspected validation error, logging it to the console.

```js
device.pushErrorScope("internal");

const module = device.createShaderModule({
  code: shader, // REALLY complex shader
});

device.popErrorScope().then((error) => {
  if (error) {
    // error is a GPUInternalError object instance
    module = null;
    console.error(`An error occurred while creating shader: ${error.message}`);
  }
});
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling)
-e 

File: /files/en-us/web/api/gpucommandencoder/writetimestamp/index.md
---
title: "GPUCommandEncoder: writeTimestamp() method"
short-title: writeTimestamp()
slug: Web/API/GPUCommandEncoder/writeTimestamp
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCommandEncoder.writeTimestamp
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`writeTimestamp()`** method of the
{{domxref("GPUCommandEncoder")}} interface encodes a command that writes a timestamp into a {{domxref("GPUQuerySet")}} once the previous commands recorded into the same queued {{domxref("GPUCommandBuffer")}} have been executed by the GPU.

> **Note:** To use timestamp queries, the `timestamp-query` {{domxref("GPUSupportedFeatures", "feature", "", "nocode")}} must be enabled in the {{domxref("GPUDevice")}}.

## Syntax

```js-nolint
writeTimestamp(querySet, queryIndex)
```

### Parameters

- `querySet`
  - : A {{domxref("GPUQuerySet")}} object representing the query set that will store the timestamp values.
- `queryIndex`
  - : A number representing the index of the query in the query set.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`writeTimestamp()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUCommandEncoder")}} becomes invalid:

- The `timestamp-query` {{domxref("GPUSupportedFeatures", "feature", "", "nocode")}} is enabled in the {{domxref("GPUDevice")}}.
- The `querySet` {{domxref("GPUQuerySet.type")}} is `"timestamp"`
- The `queryIndex` value is less than the {{domxref("GPUQuerySet.count")}}.

## Examples

```js
// ...

const querySet = device.createQuerySet({
  type: "timestamp",
  count: 32,
});

// ...

commandEncoder.writeTimestamp(querySet, 0);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/begincomputepass/index.md
---
title: "GPUCommandEncoder: beginComputePass() method"
short-title: beginComputePass()
slug: Web/API/GPUCommandEncoder/beginComputePass
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCommandEncoder.beginComputePass
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`beginComputePass()`** method of the
{{domxref("GPUCommandEncoder")}} interface starts encoding a compute pass, returning a {{domxref("GPUComputePassEncoder")}} that can be used to control computation.

## Syntax

```js-nolint
beginComputePass()
beginComputePass(descriptor)
```

### Parameters

- `descriptor` {{optional_inline}}

  - : An object containing the following properties:

    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
    - `timestampWrites` {{optional_inline}}

      - : An array of objects defining where and when timestamp query values will be written for this pass. These objects have the following properties:

        - `location`: An enumerated value specifying when the timestamp will be executed. Available values are:
          - `"beginning"`: The timestamp is executed along with the other encoded commands in the compute pass once the corresponding {{domxref("GPUCommandBuffer")}} is submitted.
          - `"end"`: The timestamp is executed as part of a separate list of timestamp attachments once the pass ends.
        - `queryIndex`: A number specifying the index position in the `querySet` that the timestamp will be written to.
        - `querySet`: The {{domxref("GPUQuerySet")}} that the timestamp will be written to.

        > **Note:** To use timestamp queries, the `timestamp-query` {{domxref("GPUSupportedFeatures", "feature", "", "nocode")}} must be enabled in the {{domxref("GPUDevice")}}.

### Return value

A {{domxref("GPUComputePassEncoder")}} object instance.

### Validation

The following criteria must be met when calling **`beginComputePass()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPUComputePassEncoder")}} is returned:

- The `timestamp-query` {{domxref("GPUSupportedFeatures", "feature", "", "nocode")}} is enabled in the {{domxref("GPUDevice")}}.
- No two `timestampWrites` objects have the same `location`. In effect, this means that you can only run two timestamp queries per render pass.
- For each timestamp query, the `querySet` {{domxref("GPUQuerySet.type")}} is `"timestamp"`, and the `queryIndex` value is less than the {{domxref("GPUQuerySet.count")}}.

## Examples

In our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/), several commands are recorded via a {{domxref("GPUCommandEncoder")}}. Most of these commands originate from the {{domxref("GPUComputePassEncoder")}} created via `beginComputePass()`.

```js
// ...

// Create GPUCommandEncoder to encode commands to issue to the GPU
const commandEncoder = device.createCommandEncoder();

// Initiate render pass
const passEncoder = commandEncoder.beginComputePass();

// Issue commands
passEncoder.setPipeline(computePipeline);
passEncoder.setBindGroup(0, bindGroup);
passEncoder.dispatchWorkgroups(Math.ceil(BUFFER_SIZE / 64));

// End the render pass
passEncoder.end();

// Copy output buffer to staging buffer
commandEncoder.copyBufferToBuffer(
  output,
  0, // Source offset
  stagingBuffer,
  0, // Destination offset
  BUFFER_SIZE,
);

// End frame by passing array of command buffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/copybuffertotexture/index.md
---
title: "GPUCommandEncoder: copyBufferToTexture() method"
short-title: copyBufferToTexture()
slug: Web/API/GPUCommandEncoder/copyBufferToTexture
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCommandEncoder.copyBufferToTexture
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`copyBufferToTexture()`** method of the
{{domxref("GPUCommandEncoder")}} interface encodes a command that copies data from a {{domxref("GPUBuffer")}} to a {{domxref("GPUTexture")}}.

## Syntax

```js-nolint
copyBufferToTexture(source, destination, copySize)
```

### Parameters

- `source`
  - : An object that defines the buffer to copy from, plus the layout of the data in the buffer to be copied to the texture. Combined with `copySize`, it defines the region of the source buffer. `source` can take the following properties:
    - `buffer`
      - : The {{domxref("GPUBuffer")}} to copy from.
    - `offset` {{optional_inline}}
      - : The offset, in bytes, from the beginning of `data` to the start of the image data to be copied. If omitted, `offset` defaults to 0.
    - `bytesPerRow` {{optional_inline}}
      - : A number representing the stride, in bytes, between the start of each block row (i.e. a row of complete texel blocks) and the subsequent block row. This is required if there are multiple block rows (i.e. the copy height or depth is more than one block).
    - `rowsPerImage` {{optional_inline}}
      - : The number of block rows per single image inside the data. `bytesPerRow` &times; `rowsPerImage` will give you the stride, in bytes, between the start of each complete image. This is required if there are multiple images to copy.
- `destination`

  - : An object defining the texture to write the data to. Combined with `copySize`, defines the region of the destination texture subresource. `destination` can take the following properties:

    - `aspect` {{optional_inline}}

      - : An enumerated value defining which aspects of the texture to write the data to. Possible values are:

        - `"all"`
          - : All available aspects of the texture format will be written to, which can mean all or any of color, depth, and stencil, depending on what kind of format you are dealing with.
        - `"depth-only"`
          - : Only the depth aspect of a [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format) will be written to.
        - `"stencil-only"`
          - : Only the stencil aspect of a depth-or-stencil format will be written to.

        If omitted, `aspect` takes a value of `"all"`.

    - `mipLevel` {{optional_inline}}
      - : A number representing the mip-map level of the texture to write the data to. If omitted, `mipLevel` defaults to 0.
    - `origin` {{optional_inline}}

      - : An object or array specifying the origin of the copy ‚Äî the minimum corner of the texture region to write the data to. Together with `size`, this defines the full extent of the region to copy to. The `x`, `y`, and `z` values default to 0 if any of all of `origin` is omitted.

        What follows is a sample array:

        ```js
        [0, 0, 0];
        ```

        The object equivalent would look like this:

        ```js
        {
          x: 0,
          y: 0,
          z: 0
        }
        ```

    - `texture`
      - : A {{domxref("GPUTexture")}} object representing the texture to write the data to.

- `copySize`

  - : An object or array specifying the width, height, and depth/array layer count of the copied data. The width value must always be specified, while the height and depth/array layer count values are optional and will default to 1 if omitted.

    What follows is a sample `copySize` array:

    ```js
    [16, 16, 2];
    ```

    The object equivalent would look like this:

    ```js
    {
      width: 16,
      height: 16,
      depthOrArrayLayers: 2
    }
    ```

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`copyBufferToTexture()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUCommandEncoder")}} becomes invalid.

For the `source`:

- `source.bytesPerRow` is a multiple of 256.
- The `source.buffer`'s {{domxref("GPUBuffer.usage")}} includes the `GPUBufferUsage.COPY_SRC` flag.

For the `destination`:

- `mipLevel` is less than the {{domxref("GPUTexture.mipLevelCount")}}.
- `origin.x` is a multiple of the texel block width of the {{domxref("GPUTexture.format")}}.
- `origin.y` is a multiple of the texel block height of the {{domxref("GPUTexture.format")}}.
- If the {{domxref("GPUTexture.format")}} is a [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format) or {{domxref("GPUTexture.sampleCount")}} is more than 1, the subresource size is equal to `size`.
- The `destination`'s {{domxref("GPUTexture.usage")}} includes the `GPUTextureUsage.COPY_DST` flag.
- The `destination`'s {{domxref("GPUTexture.sampleCount")}} is 1.
- `destination.aspect` refers to a single aspect of the {{domxref("GPUTexture.format")}}.
- That aspect is a valid image copy destination according to [depth-or-stencil formats](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format).
- The `destination` is compatible with the `copySize`.

## Examples

```js
commandEncoder.copyBufferToTexture(
  {
    buffer: sourceBuffer,
  },
  {
    texture: destinationTexture,
  },
  {
    width: 16,
    height: 16,
    depthOrArrayLayers: 2,
  },
);
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/copybuffertobuffer/index.md
---
title: "GPUCommandEncoder: copyBufferToBuffer() method"
short-title: copyBufferToBuffer()
slug: Web/API/GPUCommandEncoder/copyBufferToBuffer
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCommandEncoder.copyBufferToBuffer
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`copyBufferToBuffer()`** method of the
{{domxref("GPUCommandEncoder")}} interface encodes a command that copies data from one {{domxref("GPUBuffer")}} to another.

## Syntax

```js-nolint
copyBufferToBuffer(source, sourceOffset, destination, destinationOffset, size)
```

### Parameters

- `source`
  - : The {{domxref("GPUBuffer")}} to copy from.
- `sourceOffset`
  - : The offset, in bytes, into the `source` to begin copying from.
- `destination`
  - : The {{domxref("GPUBuffer")}} to copy to.
- `destinationOffset`
  - : The offset, in bytes, into the `destination` to begin copying to.
- `size`
  - : The number of bytes to copy.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`copyBufferToBuffer()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUCommandEncoder")}} becomes invalid:

- The `source`'s {{domxref("GPUBuffer.usage")}} includes the `GPUBufferUsage.COPY_SRC` flag.
- The `destination`'s {{domxref("GPUBuffer.usage")}} includes the `GPUBufferUsage.COPY_DST` flag.
- `size`, `sourceOffset`, and `destinationOffset` are all multiples of 4.
- The `source`'s {{domxref("GPUBuffer.size")}} is greater than or equal to `sourceOffset` + `size`.
- The `destination`'s {{domxref("GPUBuffer.size")}} is greater than or equal to `destinationOffset` + `size`.
- `source` and `destination` are different {{domxref("GPUBuffer")}}s (you can't copy from and to the same buffer).

## Examples

In our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/), we use `copyBufferToBuffer()` to copy the contents of our `output` buffer to the `stagingBuffer`.

```js
// ...

// Create an output buffer to read GPU calculations to, and a staging buffer to be mapped for JavaScript access

const output = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.STORAGE | GPUBufferUsage.COPY_SRC,
});

const stagingBuffer = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.MAP_READ | GPUBufferUsage.COPY_DST,
});

// ...

// Create GPUCommandEncoder to encode commands to issue to the GPU
const commandEncoder = device.createCommandEncoder();

// ...

// Copy output buffer to staging buffer
commandEncoder.copyBufferToBuffer(
  output,
  0, // Source offset
  stagingBuffer,
  0, // Destination offset
  BUFFER_SIZE,
);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/label/index.md
---
title: "GPUCommandEncoder: label property"
short-title: label
slug: Web/API/GPUCommandEncoder/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUCommandEncoder.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** read-only property of the
{{domxref("GPUCommandEncoder")}} interface is a string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUDevice.createCommandEncoder()")}} call, or you can get and set it directly on the `GPUCommandEncoder` object.

## Value

A string. If no label value has previously been set, getting the label returns an empty string.

## Examples

Setting and getting a label via `GPUCommandEncoder.label`:

```js
const commandEncoder = device.createCommandEncoder();
commandEncoder.label = "mycommandencoder";
console.log(commandEncoder.label); // "mycommandencoder";
```

Setting a label via the originating {{domxref("GPUDevice.createCommandEncoder()")}} call, and then getting it via `GPUCommandEncoder.label`:

```js
const commandEncoder = device.createCommandEncoder({
  label: "mycommandencoder",
});

console.log(commandEncoder.label); // "mycommandencoder";
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/copytexturetobuffer/index.md
---
title: "GPUCommandEncoder: copyTextureToBuffer() method"
short-title: copyTextureToBuffer()
slug: Web/API/GPUCommandEncoder/copyTextureToBuffer
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCommandEncoder.copyTextureToBuffer
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`copyTextureToBuffer()`** method of the
{{domxref("GPUCommandEncoder")}} interface encodes a command that copies data from a {{domxref("GPUTexture")}} to a {{domxref("GPUBuffer")}}.

## Syntax

```js-nolint
copyTextureToBuffer(source, destination, copySize)
```

### Parameters

- `source`

  - : An object defining the texture to copy the data from. Combined with `copySize`, defines the region of the source texture subresource. `source` can take the following properties:

    - `aspect` {{optional_inline}}

      - : An enumerated value defining which aspects of the texture to copy the data from. Possible values are:

        - `"all"`
          - : All available aspects of the texture format will be copied from, which can mean all or any of color, depth, and stencil, depending on what kind of format you are dealing with.
        - `"depth-only"`
          - : Only the depth aspect of a [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format) will be copied from.
        - `"stencil-only"`
          - : Only the stencil aspect of a depth-or-stencil format will be copied from.

        If omitted, `aspect` takes a value of `"all"`.

    - `mipLevel` {{optional_inline}}
      - : A number representing the mip-map level of the texture to copy the data from. If omitted, `mipLevel` defaults to 0.
    - `origin` {{optional_inline}}

      - : An object or array specifying the origin of the copy ‚Äî the minimum corner of the texture region to copy the data from. Together with `size`, this defines the full extent of the region to copy from. The `x`, `y`, and `z` values default to 0 if any of all of `origin` is omitted.

        What follows is a sample array:

        ```js
        [0, 0, 0];
        ```

        The object equivalent would look like this:

        ```js
        {
          x: 0,
          y: 0,
          z: 0
        }
        ```

    - `texture`
      - : A {{domxref("GPUTexture")}} object representing the texture to copy the data from.

- `destination`

  - : An object that defines the buffer to write to, plus the layout of the data to write to the buffer. Combined with `copySize`, it defines the region of the destination buffer. `source` can take the following properties:
    - `buffer`
      - : The {{domxref("GPUBuffer")}} to write to.
    - `offset` {{optional_inline}}
      - : The offset, in bytes, from the beginning of `data` to the start position to write the copied data to. If omitted, `offset` defaults to 0.
    - `bytesPerRow` {{optional_inline}}
      - : A number representing the stride, in bytes, between the start of each block row (i.e. a row of complete texel blocks) and the subsequent block row. This is required if there are multiple block rows (i.e. the copy height or depth is more than one block).
    - `rowsPerImage` {{optional_inline}}
      - : The number of block rows per single image inside the data. `bytesPerRow` &times; `rowsPerImage` will give you the stride, in bytes, between the start of each complete image. This is required if there are multiple images to copy.

- `copySize`

  - : An object or array specifying the width, height, and depth/array layer count of the copied data. The width value must always be specified, while the height and depth/array layer count values are optional and will default to 1 if omitted.

    What follows is a sample `copySize` array:

    ```js
    [16, 16, 2];
    ```

    The object equivalent would look like this:

    ```js
    {
      width: 16,
      height: 16,
      depthOrArrayLayers: 2
    }
    ```

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`copyTextureToBuffer()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUCommandEncoder")}} becomes invalid.

For the `source`:

- `mipLevel` is less than the {{domxref("GPUTexture.mipLevelCount")}}.
- `origin.x` is a multiple of the texel block width of the {{domxref("GPUTexture.format")}}.
- `origin.y` is a multiple of the texel block height of the {{domxref("GPUTexture.format")}}.
- If the {{domxref("GPUTexture.format")}} is a [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format) or {{domxref("GPUTexture.sampleCount")}} is more than 1, the subresource size is equal to `size`.
- The `source`'s {{domxref("GPUTexture.usage")}} includes the `GPUTextureUsage.COPY_SRC` flag.
- The `source`'s {{domxref("GPUTexture.sampleCount")}} is 1.
- `source.aspect` refers to a single aspect of the {{domxref("GPUTexture.format")}}.
- That aspect is a valid image copy source according to [depth-or-stencil formats](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format).
- The `source` is compatible with the `copySize`.

For the `destination`:

- `destination.bytesPerRow` is a multiple of 256.
- The `destination.buffer`'s {{domxref("GPUBuffer.usage")}} includes the `GPUBufferUsage.COPY_DST` flag.

## Examples

```js
commandEncoder.copyTextureToBuffer(
  {
    texture: sourceTexture,
  },
  {
    buffer: destinationBuffer,
  },
  {
    width: 16,
    height: 16,
    depthOrArrayLayers: 2,
  },
);
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/resolvequeryset/index.md
---
title: "GPUCommandEncoder: resolveQuerySet() method"
short-title: resolveQuerySet()
slug: Web/API/GPUCommandEncoder/resolveQuerySet
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCommandEncoder.resolveQuerySet
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`resolveQuerySet()`** method of the
{{domxref("GPUCommandEncoder")}} interface encodes a command that resolves a {{domxref("GPUQuerySet")}}, copying the results into a specified {{domxref("GPUBuffer")}}.

## Syntax

```js-nolint
resolveQuerySet(querySet, firstQuery, queryCount, destination, destinationOffset)
```

### Parameters

- `querySet`
  - : A {{domxref("GPUQuerySet")}} object representing the query set to be resolved.
- `firstQuery`
  - : The index number of the first query value to be copied over to the buffer.
- `queryCount`
  - : The number of queries to be copied over to the buffer, starting from `firstQuery`.
- `destination`
  - : A {{domxref("GPUBuffer")}} representing the buffer to copy the query values to.
- `destinationOffset`
  - : A number representing the offset, in bytes, from the start of the buffer to start writing the query values at.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`resolveQuerySet()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUCommandEncoder")}} becomes invalid:

- The `destination.buffer`'s {{domxref("GPUBuffer.usage")}} includes the `GPUBufferUsage.QUERY_RESOLVE` flag.
- `firstQuery` is smaller than the number of queries in `querySet`.
- `firstQuery` + `queryCount` is smaller than or equal to the number of queries in `querySet`.
- `destinationOffset` is a multiple of 256.
- `destinationOffset` + 8 √ó `queryCount` is less than or equal to `destination.size`.

## Examples

```js
// ...

const queryBuffer = device.createBuffer({
  size: 1024,
  usage: GPUBufferUsage.QUERY_RESOLVE,
});

const querySet = device.createQuerySet({
  type: "timestamp",
  count: 32,
});

// ...

const commandEncoder = device.createCommandEncoder();

// Write timestamps to querySet
commandEncoder.writeTimestamp(querySet, 0);
// ...
commandEncoder.writeTimestamp(querySet, 1);
// etc.

// ...

commandEncoder.resolveQuerySet(
  querySet,
  0, // First query to write
  16, // Number of queries to count
  queryBuffer,
  0, // Buffer offset
);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/insertdebugmarker/index.md
---
title: "GPUCommandEncoder: insertDebugMarker() method"
short-title: insertDebugMarker()
slug: Web/API/GPUCommandEncoder/insertDebugMarker
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCommandEncoder.insertDebugMarker
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`insertDebugMarker()`** method of the
{{domxref("GPUCommandEncoder")}} interface marks a specific point in a series of encoded commands with a label.

This could be used for telemetry, or may be utilized in {{domxref("GPUError")}} messages, browser dev tools, or other services in the future to help with debugging.

## Syntax

```js-nolint
insertDebugMarker(markerLabel)
```

### Parameters

- `markerLabel`
  - : A string representing the label to insert.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
// ...

commandEncoder.insertDebugMarker("mymarker");

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/index.md
---
title: GPUCommandEncoder
slug: Web/API/GPUCommandEncoder
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUCommandEncoder
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUCommandEncoder`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents a command encoder, used to encode commands to be issued to the GPU.

A `GPUCommandEncoder` object instance is created via the {{domxref("GPUDevice.createCommandEncoder()")}} property.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUCommandEncoder.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Instance methods

- {{domxref("GPUCommandEncoder.beginComputePass", "beginComputePass()")}} {{Experimental_Inline}}
  - : Starts encoding a compute pass, returning a {{domxref("GPUComputePassEncoder")}} that can be used to control computation.
- {{domxref("GPUCommandEncoder.beginRenderPass", "beginRenderPass()")}} {{Experimental_Inline}}
  - : Starts encoding a render pass, returning a {{domxref("GPURenderPassEncoder")}} that can be used to control rendering.
- {{domxref("GPUCommandEncoder.clearBuffer", "clearBuffer()")}} {{Experimental_Inline}}
  - : Encodes a command that fills a region of a {{domxref("GPUBuffer")}} with zeroes.
- {{domxref("GPUCommandEncoder.copyBufferToBuffer", "copyBufferToBuffer()")}} {{Experimental_Inline}}
  - : Encodes a command that copies data from one {{domxref("GPUBuffer")}} to another.
- {{domxref("GPUCommandEncoder.copyBufferToTexture", "copyBufferToTexture()")}} {{Experimental_Inline}}
  - : Encodes a command that copies data from a {{domxref("GPUBuffer")}} to a {{domxref("GPUTexture")}}.
- {{domxref("GPUCommandEncoder.copyTextureToBuffer", "copyTextureToBuffer()")}} {{Experimental_Inline}}
  - : Encodes a command that copies data from a {{domxref("GPUTexture")}} to a {{domxref("GPUBuffer")}}.
- {{domxref("GPUCommandEncoder.copyTextureToTexture", "copyTextureToTexture()")}} {{Experimental_Inline}}
  - : Encodes a command that copies data from one {{domxref("GPUTexture")}} to another.
- {{domxref("GPUCommandEncoder.finish", "finish()")}} {{Experimental_Inline}}

  - : Completes recording of the command sequence encoded on this `GPUCommandEncoder`, returning a corresponding {{domxref("GPUCommandBuffer")}}.

- {{domxref("GPUCommandEncoder.insertDebugMarker", "insertDebugMarker()")}} {{Experimental_Inline}}
  - : Marks a specific point in a series of encoded commands with a label.
- {{domxref("GPUCommandEncoder.popDebugGroup", "popDebugGroup()")}} {{Experimental_Inline}}
  - : Ends a debug group, which is begun with a {{domxref("GPUCommandEncoder.pushDebugGroup", "pushDebugGroup()")}} call.
- {{domxref("GPUCommandEncoder.pushDebugGroup", "pushDebugGroup()")}} {{Experimental_Inline}}

  - : Begins a debug group, which is marked with a specified label, and will contain all subsequent encoded commands up until a {{domxref("GPUCommandEncoder.popDebugGroup", "popDebugGroup()")}} method is invoked.

- {{domxref("GPUCommandEncoder.resolveQuerySet", "resolveQuerySet()")}} {{Experimental_Inline}}
  - : Encodes a command that resolves a {{domxref("GPUQuerySet")}}, copying the results into a specified {{domxref("GPUBuffer")}}.
- {{domxref("GPUCommandEncoder.writeTimestamp", "writeTimestamp()")}} {{Experimental_Inline}}
  - : Encodes a command that writes a timestamp into a {{domxref("GPUQuerySet")}} once the previous commands recorded into the same queued {{domxref("GPUCommandBuffer")}} have been executed by the GPU.

## Examples

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/), several commands are recorded via a {{domxref("GPUCommandEncoder")}}:

```js
// ...

// Create GPUCommandEncoder
const commandEncoder = device.createCommandEncoder();

// Create GPURenderPassDescriptor to tell WebGPU which texture to draw into, then initiate render pass

const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
};

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// Draw a triangle

passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

// End the render pass

passEncoder.end();

// ...
```

The commands encoded by the {{domxref("GPUCommandEncoder")}} are recoded into a {{domxref("GPUCommandBuffer")}} using the {{domxref("GPUCommandEncoder.finish()")}} method. The command buffer is then passed into the queue via a {{domxref("GPUQueue.submit", "submit()")}} call, ready to be processed by the GPU.

```js
device.queue.submit([commandEncoder.finish()]);
```

> **Note:** Study the [WebGPU samples](https://webgpu.github.io/webgpu-samples/) to find more command encoding examples.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/popdebuggroup/index.md
---
title: "GPUCommandEncoder: popDebugGroup() method"
short-title: popDebugGroup()
slug: Web/API/GPUCommandEncoder/popDebugGroup
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCommandEncoder.popDebugGroup
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`popDebugGroup()`** method of the
{{domxref("GPUCommandEncoder")}} interface ends a debug group, which is begun with a {{domxref("GPUCommandEncoder.pushDebugGroup", "pushDebugGroup()")}} call.

This could be used for telemetry, or may be utilized in {{domxref("GPUError")}} messages, browser dev tools, or other services in the future to help with debugging.

## Syntax

```js-nolint
popDebugGroup()
```

### Parameters

None.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`popDebugGroup()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUCommandEncoder")}} becomes invalid:

- The command encoder's debug stack is not empty (i.e. at least one debug group was previously started with {{domxref("GPUCommandEncoder.pushDebugGroup", "pushDebugGroup()")}}).

## Examples

```js
// ...

commandEncoder.pushDebugGroup("mygroupmarker"); // Start labeled debug group

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

passEncoder.end();

commandEncoder.popDebugGroup(); // End labeled debug group

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/finish/index.md
---
title: "GPUCommandEncoder: finish() method"
short-title: finish()
slug: Web/API/GPUCommandEncoder/finish
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCommandEncoder.finish
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`finish()`** method of the
{{domxref("GPUCommandEncoder")}} interface completes recording of the command sequence encoded on this `GPUCommandEncoder`, returning a corresponding {{domxref("GPUCommandBuffer")}}.

## Syntax

```js-nolint
finish()
finish(descriptor)
```

### Parameters

- `descriptor` {{optional_inline}}
  - : An object that can contain the following properties:
    - `label` {{optional_inline}}
      - : A string providing a label for the returned {{domxref("GPUCommandBuffer")}} that can be used to identify it, for example in {{domxref("GPUError")}} messages or console warnings.

### Return value

A {{domxref("GPUCommandBuffer")}} object instance.

### Validation

The following criteria must be met when calling **`finish()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUCommandEncoder")}} becomes invalid:

- There are no active debug groups (i.e. started via {{domxref("GPUCommandEncoder.pushDebugGroup", "pushDebugGroup()")}}).
- The {{domxref("GPUCommandEncoder")}} is in an open state ‚Äî this means that:
  - There are no child {{domxref("GPUComputePassEncoder")}} or {{domxref("GPURenderPassEncoder")}}s active that have not been `end()`ed.
  - The {{domxref("GPUCommandEncoder")}} has not already had `finish()` called on it (in which case it cannot be used to encode any more commands).

## Examples

```js
// ...

const commandBuffer = commandEncoder.finish();
device.queue.submit([commandBuffer]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/pushdebuggroup/index.md
---
title: "GPUCommandEncoder: pushDebugGroup() method"
short-title: pushDebugGroup()
slug: Web/API/GPUCommandEncoder/pushDebugGroup
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCommandEncoder.pushDebugGroup
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`pushDebugGroup()`** method of the
{{domxref("GPUCommandEncoder")}} interface begins a debug group, which is marked with a specified label, and will contain all subsequent encoded commands up until a {{domxref("GPUCommandEncoder.popDebugGroup", "popDebugGroup()")}} method is invoked.

This could be used for telemetry, or may be utilized in {{domxref("GPUError")}} messages, browser dev tools, or other services in the future to help with debugging.

## Syntax

```js-nolint
pushDebugGroup(groupLabel)
```

### Parameters

- `groupLabel`
  - : A string representing the label for the debug group.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
// ...

commandEncoder.pushDebugGroup("mygroupmarker"); // Start labeled debug group

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

passEncoder.end();

commandEncoder.popDebugGroup(); // End labeled debug group

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/clearbuffer/index.md
---
title: "GPUCommandEncoder: clearBuffer() method"
short-title: clearBuffer()
slug: Web/API/GPUCommandEncoder/clearBuffer
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCommandEncoder.clearBuffer
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`clearBuffer()`** method of the
{{domxref("GPUCommandEncoder")}} interface encodes a command that fills a region of a {{domxref("GPUBuffer")}} with zeroes.

## Syntax

```js-nolint
clearBuffer(buffer)
clearBuffer(buffer, offset)
clearBuffer(buffer, offset, size)
```

### Parameters

- `buffer`
  - : A {{domxref("GPUBuffer")}} object representing the buffer to clear.
- `offset` {{optional_inline}}
  - : A number representing the offset, in bytes, from the start of the `buffer` to the sub-region to clear. If omitted, `offset` defaults to 0.
- `size` {{optional_inline}}
  - : A number representing the size, in bytes, of the sub-region to clear. If omitted, `size` defaults to the `buffer` size - `offset`.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`clearBuffer()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUCommandEncoder")}} becomes invalid:

- The `buffer`'s {{domxref("GPUBuffer.usage")}} includes the `GPUBufferUsage.COPY_DST` flag.
- `offset` and `size` are both multiples of 4.
- The `buffer`'s {{domxref("GPUBuffer.size")}} is greater than or equal to `offset` + `size`.

## Examples

```js
// ...

const buffer = device.createBuffer({
  size: 1000,
  usage: GPUBufferUsage.MAP_READ | GPUBufferUsage.COPY_DST,
});

// Later on

const commandBuffer = device.createCommandEncoder();
commandEncoder.clearBuffer(buffer);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/beginrenderpass/index.md
---
title: "GPUCommandEncoder: beginRenderPass() method"
short-title: beginRenderPass()
slug: Web/API/GPUCommandEncoder/beginRenderPass
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCommandEncoder.beginRenderPass
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`beginRenderPass()`** method of the
{{domxref("GPUCommandEncoder")}} interface starts encoding a render pass, returning a {{domxref("GPURenderPassEncoder")}} that can be used to control rendering.

## Syntax

```js-nolint
beginRenderPass(descriptor)
```

### Parameters

- `descriptor`

  - : An object containing the following properties:

    - `colorAttachments`
      - : An array of objects (see [Color attachment object structure](#color_attachment_object_structure)) defining the color attachments that will be output to when executing this render pass.
    - `depthStencilAttachment` {{optional_inline}}
      - : An object (see [Depth/stencil attachment object structure](#depthstencil_attachment_object_structure)) defining the depth/stencil attachment that will be output to and tested against when executing this render pass.
    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
    - `maxDrawCount` {{optional_inline}}
      - : A number indicating the maximum number of draw calls that will be done in the render pass. This is used by some implementations to size work injected before the render pass. You should keep the default value ‚Äî 50000000 ‚Äî unless you know that more draw calls will be done.
    - `occlusionQuerySet` {{optional_inline}}
      - : The {{domxref("GPUQuerySet")}} that will store the occlusion query results for this pass.
    - `timestampWrites` {{optional_inline}}

      - : An array of objects defining where and when timestamp query values will be written for this pass. These objects have the following properties:

        - `location`: An enumerated value specifying when the timestamp will be executed. Available values are:
          - `"beginning"`: The timestamp is executed along with the other encoded commands in the compute pass once the corresponding {{domxref("GPUCommandBuffer")}} is submitted.
          - `"end"`: The timestamp is executed as part of a separate list of timestamp attachments once the pass ends.
        - `queryIndex`: A number specifying the index position in the `querySet` that the timestamp will be written to.
        - `querySet`: The {{domxref("GPUQuerySet")}} that the timestamp will be written to.

        > **Note:** To use timestamp queries, the `timestamp-query` {{domxref("GPUSupportedFeatures", "feature", "", "nocode")}} must be enabled in the {{domxref("GPUDevice")}}.

### Color attachment object structure

Color attachment objects can have the following properties:

- `clearValue` {{optional_inline}}

  - : A color value to clear the `view` texture to, prior to executing the render pass. This value is ignored if `loadOp` is not set to `"clear"`. `clearValue` takes an array or object representing the four color components `r`, `g`, `b`, and `a` as decimals.

    What follows is a sample array:

    ```js
    clearValue: [0.0, 0.5, 1.0, 1.0];
    ```

    The object equivalent would look like this:

    ```js
    clearValue: {
      r: 0.0,
      g: 0.5,
      b: 1.0,
      a: 1.0
    }
    ```

    If `clearValue` is omitted, it defaults to `{r: 0, g: 0, b: 0, a: 0}`.

- `loadOp`

  - : An enumerated value indicating the load operation to perform on `view` prior to executing the render pass. Possible values are:

    - `"clear"`: Loads the `clearValue` for this attachment into the render pass.
    - `"load"`: Loads the existing value for this attachment into the render pass.

    > **Note:** It is recommended to always use `"clear"` in cases where the initial value doesn't matter, as it will give better performance on some devices such as mobiles.

- `storeOp`
  - : An enumerated value indicating the store operation to perform on `view` after executing the render pass. Possible values are:
    - `"discard"`: Discards the resulting value of the render pass for this attachment.
    - `"store"`: Stores the resulting value of the render pass for this attachment.
- `resolveTarget` {{optional_inline}}
  - : A {{domxref("GPUTextureView")}} object representing the texture subresource that will receive the resolved output for this color attachment if `view` is multisampled.
- `view`

  - : A {{domxref("GPUTextureView")}} object representing the texture subresource that will be output to for this color attachment.

    > **Note:** Each color or depth/stencil attachment must be a unique texture subresource, and texture subresources used as attachments cannot be used inside the render pass.

### Depth/stencil attachment object structure

The `depthStencilAttachment` object can have the following properties:

- `depthClearValue` {{optional_inline}}

  - : A number indicating the value to clear `view`'s depth component prior to executing the render pass. This is ignored if `depthLoadOp` is not set to `"clear"`.

    The value must be between 0.0 and 1.0, inclusive.

- `depthLoadOp` {{optional_inline}}

  - : An enumerated value indicating the load operation to perform on `view`'s depth component prior to executing the render pass. Possible values are:

    - `"clear"`: Loads the `clearValue` for this attachment into the render pass.
    - `"load"`: Loads the existing value for this attachment into the render pass.

    > **Note:** It is recommended to always use `"clear"` in cases where the initial value doesn't matter, as it will give better performance on some devices such as mobiles.

- `depthReadOnly` {{optional_inline}}
  - : A boolean. Setting the value to `true` causes the depth component of `view` to be read-only. If `depthReadOnly` is omitted, it defaults to `false`.
- `depthStoreOp` {{optional_inline}}
  - : An enumerated value indicating the store operation to perform on `view`'s depth component after executing the render pass. Possible values are:
    - `"discard"`: Discards the resulting value of the render pass for this attachment.
    - `"store"`: Stores the resulting value of the render pass for this attachment.
- `stencilClearValue` {{optional_inline}}

  - : A number indicating the value to clear `view`'s stencil component to prior to executing the render pass. This is ignored if `stencilLoadOp` is not set to `"clear"`.

    If `stencilClearValue` is omitted, it defaults to 0.

- `stencilLoadOp` {{optional_inline}}

  - : An enumerated value indicating the load operation to perform on `view`'s stencil component prior to executing the render pass. Possible values are:

    - `"clear"`: Loads the `clearValue` for this attachment into the render pass.
    - `"load"`: Loads the existing value for this attachment into the render pass.

    > **Note:** It is recommended to always use `"clear"` in cases where the initial value doesn't matter, as it will give better performance on some devices such as mobiles.

- `stencilReadOnly` {{optional_inline}}
  - : A boolean. Setting the value to `true` causes the stencil component of `view` to be read-only. If `stencilReadOnly` is omitted, it defaults to `false`.
- `stencilStoreOp` {{optional_inline}}
  - : An enumerated value indicating the store operation to perform on `view`'s stencil component after executing the render pass. Possible values are:
    - `"discard"`: Discards the resulting value of the render pass for this attachment.
    - `"store"`: Stores the resulting value of the render pass for this attachment.
- `view`
  - : A {{domxref("GPUTextureView")}} object representing the texture subresource that will be output to and read from for this depth/stencil attachment.

### Return value

A {{domxref("GPURenderPassEncoder")}} object instance.

### Validation

The following criteria must be met when calling **`beginRenderPass()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPURenderPassEncoder")}} is returned.

General:

- `colorAttachments.length` is less than or equal to the {{domxref("GPUDevice")}}'s `maxColorAttachments` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- If `colorAttachments` contains only `null` values, `depthStencilAttachment` is provided.
- All `view`s in `colorAttachments` and `depthStencilAttachment` have equal {{domxref("GPUTexture.sampleCount")}} values and render extents ({{domxref("GPUTexture.height")}}, {{domxref("GPUTexture.width")}}, and {{domxref("GPUTexture.depthOrArrayLayers")}}).
- If `occlusionQuerySet` is set, the referenced {{domxref("GPUQuerySet")}} has a `type` of `"occlusion"`.

For color attachment objects

- The `view` is renderable, and the `view`'s format (i.e. specified in the descriptor of the originating {{domxref("GPUTexture.createView()")}} call) is a color renderable format.
- If `resolveTarget` is provided:
  - The `view`'s originating {{domxref("GPUTexture")}}'s {{domxref("GPUTexture.sampleCount", "sampleCount")}} is greater than 1.
  - The `resolveTarget`'s originating {{domxref("GPUTexture")}}'s {{domxref("GPUTexture.sampleCount", "sampleCount")}} is 1.
  - `resolveTarget` is renderable.
  - The sizes of the subresources that `view` and `resolveTarget` provide a view of match.
  - `view`'s and `resolveTarget`'s formats match.
- [Color attachments bytes per sample](https://gpuweb.github.io/gpuweb/#abstract-opdef-validating-gpurenderpassdescriptors-color-attachment-bytes-per-sample) is less than or equal to the {{domxref("GPUDevice")}}'s `maxColorAttachmentBytesPerSample` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.

For depth/stencil attachment objects:

- The `view` is renderable, and its format is a [depth-or-stencil](https://gpuweb.github.io/gpuweb/#depth-or-stencil-format) format.
- If `depthLoadOp` is set to `"clear"`, a valid `depthClearValue` is provided.
- If `view`'s format is a combined depth-or-stencil format, `depthReadOnly` matches `stencilReadOnly`.
- If `view`'s format has a depth aspect, and `depthReadOnly` is `false`, `depthLoadOp` and `depthStoreOp` are provided.
- If `view`'s format has a depth aspect, and `depthReadOnly` is `true`, `depthLoadOp` and `depthStoreOp` are not provided.
- If `view`'s format has a stencil aspect, and `stencilReadOnly` is `false`, `stencilLoadOp` and `stencilStoreOp` are provided.
- If `view`'s format has a stencil aspect, and `stencilReadOnly` is `true`, `stencilLoadOp` and `stencilStoreOp` are not provided.

For timestamp queries:

- The `timestamp-query` {{domxref("GPUSupportedFeatures", "feature", "", "nocode")}} is enabled in the {{domxref("GPUDevice")}}.
- No two `timestampWrites` objects have the same `location`. In effect, this means that you can only run two timestamp queries per render pass.
- For each timestamp query, the `querySet` {{domxref("GPUQuerySet.type")}} is `"timestamp"`, and the `queryIndex` value is less than the {{domxref("GPUQuerySet.count")}}.
- No two `timestampWrites` objects have the same `queryIndex` and `querySet` pair.

## Examples

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/), a number of commands are recorded via a {{domxref("GPUCommandEncoder")}}. These commands originate from the {{domxref("GPURenderPassEncoder")}} created via `beginRenderPass()` :

```js
// ...

// Create GPUCommandEncoder
const commandEncoder = device.createCommandEncoder();

// Create GPURenderPassDescriptor to tell WebGPU which texture to draw into, then initiate render pass

const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
};

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// Draw a triangle

passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

// End the render pass

passEncoder.end();

device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandencoder/copytexturetotexture/index.md
---
title: "GPUCommandEncoder: copyTextureToTexture() method"
short-title: copyTextureToTexture()
slug: Web/API/GPUCommandEncoder/copyTextureToTexture
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUCommandEncoder.copyTextureToTexture
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`copyTextureToTexture()`** method of the
{{domxref("GPUCommandEncoder")}} interface encodes a command that copies data from one {{domxref("GPUTexture")}} to another.

## Syntax

```js-nolint
copyTextureToTexture(source, destination, copySize)
```

### Parameters

- `source`
  - : An object (see [Copy texture object structure](#copy_texture_object_structure)) defining the texture to copy the data from. Combined with `copySize`, this defines the region of the source texture subresource.
- `destination`
  - : An object (see [Copy texture object structure](#copy_texture_object_structure)) defining the texture to write the data to. Combined with `copySize`, this defines the region of the destination texture subresource.
- `copySize`

  - : An object or array specifying the width, height, and depth/array layer count of the copied data. The width value must always be specified, while the height and depth/array layer count values are optional and will default to 1 if omitted.

    What follows is a sample `copySize` array:

    ```js
    [16, 16, 2];
    ```

    The object equivalent would look like this:

    ```js
    {
      width: 16,
      height: 16,
      depthOrArrayLayers: 2
    }
    ```

### Copy texture object structure

A copy texture object has the following structure:

- `aspect` {{optional_inline}}

  - : An enumerated value defining which aspects of the texture to copy the data from/to. Possible values are:

    - `"all"`
      - : All available aspects of the texture format will be copied from/to, which can mean all or any of color, depth, and stencil, depending on what kind of format you are dealing with.
    - `"depth-only"`
      - : Only the depth aspect of a [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format) will be copied from/to.
    - `"stencil-only"`
      - : Only the stencil aspect of a depth-or-stencil format will be copied from/to.

    If omitted, `aspect` takes a value of `"all"`.

- `mipLevel` {{optional_inline}}
  - : A number representing the mip-map level of the texture to copy the data from/to. If omitted, `mipLevel` defaults to 0.
- `origin` {{optional_inline}}

  - : An object or array specifying the origin of the copy/destination ‚Äî the minimum corner of the texture region to copy the data from/to. Together with `size`, this defines the full extent of the region to copy from/to. The `x`, `y`, and `z` values default to 0 if any of all of `origin` is omitted.

    What follows is a sample array:

    ```js
    [0, 0, 0];
    ```

    The object equivalent would look like this:

    ```js
    {
      x: 0,
      y: 0,
      z: 0
    }
    ```

- `texture`
  - : A {{domxref("GPUTexture")}} object representing the texture to copy the data from/to.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`copyTextureToTexture()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUCommandEncoder")}} becomes invalid.

For the `source`:

- The `source`'s {{domxref("GPUTexture.usage")}} includes the `GPUTextureUsage.COPY_SRC` flag.

For the `destination`:

- The `source`'s {{domxref("GPUTexture.usage")}} includes the `GPUTextureUsage.COPY_DST` flag.

For `source` and `destination`:

- `mipLevel` is less than the {{domxref("GPUTexture.mipLevelCount")}}.
- `origin.x` is a multiple of the texel block width of the {{domxref("GPUTexture.format")}}.
- `origin.y` is a multiple of the texel block height of the {{domxref("GPUTexture.format")}}.
- The source and destination `texture` {{domxref("GPUTexture.format")}}s are copy-compatible.
- The source and destination `texture` {{domxref("GPUTexture.sampleCount")}}s are equal.
- If the {{domxref("GPUTexture.format")}} is a [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format) or {{domxref("GPUTexture.sampleCount")}} is more than 1, the subresource size is equal to `size`.
- The `texture`'s {{domxref("GPUTexture.sampleCount")}} is 1.
- `aspect` refers to a single aspect of the {{domxref("GPUTexture.format")}}.
- That aspect is a valid image copy source/destination according to [depth-or-stencil formats](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format).
- The `texture` is compatible with the `copySize`.

## Examples

```js
commandEncoder.copyTextureToTexture(
  {
    texture: sourceTexture,
  },
  {
    texture: destinationTexture,
  },
  {
    width: 16,
    height: 16,
    depthOrArrayLayers: 2,
  },
);
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucompilationinfo/messages/index.md
---
title: "GPUCompilationInfo: messages property"
short-title: messages
slug: Web/API/GPUCompilationInfo/messages
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUCompilationInfo.messages
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`messages`** read-only property of the
{{domxref("GPUCompilationInfo")}} interface is an array of {{domxref("GPUCompilationMessage")}} objects, each one containing the details of an individual shader compilation message. Messages can be informational, warnings, or errors.

## Value

An array of {{domxref("GPUCompilationMessage")}} objects.

## Examples

See the main [`GPUCompilationInfo` page](/en-US/docs/Web/API/GPUCompilationInfo#examples) for an example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucompilationinfo/index.md
---
title: GPUCompilationInfo
slug: Web/API/GPUCompilationInfo
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUCompilationInfo
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUCompilationInfo`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents an array of {{domxref("GPUCompilationMessage")}} objects generated by the GPU shader module compiler to help diagnose problems with shader code.

`GPUCompilationInfo` is accessed via {{domxref("GPUShaderModule.getCompilationInfo()")}}.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUCompilationInfo.messages", "messages")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : An array of {{domxref("GPUCompilationMessage")}} objects, each one containing the details of an individual shader compilation message. Messages can be informational, warnings, or errors.

## Examples

In the example below, we have deliberately left a parenthesis out of a function declaration in our shader code:

```js
const shaders = `
struct VertexOut {
  @builtin(position) position : vec4f,
  @location(0) color : vec4f
}

@vertex
fn vertex_main(@location(0) position: vec4f,
               @location(1) color: vec4f -> VertexOut
{
  var output : VertexOut;
  output.position = position;
  output.color = color;
  return output;
}

@fragment
fn fragment_main(fragData: VertexOut) -> @location(0) vec4f
{
  return fragData.color;
}
`;
```

When we compile the shader module, we use `getCompilationInfo()` to grab some information about the resulting error:

```js
async function init() {
  // ...

  const shaderModule = device.createShaderModule({
    code: shaders,
  });

  const shaderInfo = await shaderModule.getCompilationInfo();
  const firstMessage = shaderInfo.messages[0];

  console.log(firstMessage.lineNum); // 9
  console.log(firstMessage.message); // "expected ')' for function declaration"
  console.log(firstMessage.type); // "error"
  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandbuffer/label/index.md
---
title: "GPUCommandBuffer: label property"
short-title: label
slug: Web/API/GPUCommandBuffer/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUCommandBuffer.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** read-only property of the
{{domxref("GPUCommandBuffer")}} interface is a string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUCommandEncoder.finish()")}} call, or you can get and set it directly on the `GPUCommandBuffer` object.

## Value

A string. If no label value has previously been set, getting the label returns an empty string.

## Examples

Setting and getting a label via `GPUCommandBuffer.label`:

```js
const commandBuffer = commandEncoder.finish();
commandBuffer.label = "mycommandbuffer";
console.log(commandBuffer.label); // "mycommandbuffer";
```

Setting a label via the originating {{domxref("GPUCommandEncoder.finish()")}} call, and then getting it via `GPUCommandBuffer.label`:

```js
const commandBuffer = commandEncoder.finish({
  label: "mycommandbuffer",
});

console.log(commandBuffer.label); // "mycommandbuffer";
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucommandbuffer/index.md
---
title: GPUCommandBuffer
slug: Web/API/GPUCommandBuffer
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUCommandBuffer
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUCommandBuffer`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents a pre-recorded list of GPU commands that can be submitted to a {{domxref("GPUQueue")}} for execution.

A `GPUCommandBuffer` is created via the {{domxref("GPUCommandEncoder.finish()")}} method; the GPU commands recorded within are submitted for execution by passing the `GPUCommandBuffer` into the parameter of a {{domxref("GPUQueue.submit()")}} call.

> **Note:** Once a `GPUCommandBuffer` object has been submitted, it cannot be used again.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUCommandBuffer.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Examples

```js
// ...

const commandBuffer = commandEncoder.finish();
device.queue.submit([commandBuffer]);
```

> **Note:** Study the [WebGPU samples](https://webgpu.github.io/webgpu-samples/) to find complete examples.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpusupportedfeatures/index.md
---
title: GPUSupportedFeatures
slug: Web/API/GPUSupportedFeatures
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUSupportedFeatures
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUSupportedFeatures`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} is a [`Set`-like object](/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set#set-like_browser_apis) that describes additional functionality supported by a {{domxref("GPUAdapter")}}.

The `GPUSupportedFeatures` object for the current adapter is accessed via the {{domxref("GPUAdapter.features")}} property.

You should note that not all features will be available to WebGPU in all browsers that support it, even if the features are supported by the underlying hardware. This could be due to constraints in the underlying system, browser, or adapter. For example:

- The underlying system might not be able to guarantee exposure of a feature in a way that is compatible with a certain browser.
- The browser vendor might not have found a secure way to implement support for that feature, or might just not have gotten round to it yet.

If you are hoping to take advantage of a specific additional feature in a WebGPU app, thorough testing is advised.

{{InheritanceDiagram}}

## Available features

We have not listed the exact set of additional features available to be used in WebGPU, as it will vary between implementations and physical devices, and will change over time. For a list, refer to the [Feature Index](https://gpuweb.github.io/gpuweb/#feature-index) in the specification.

## Instance properties

The following properties are available to all read-only [`Set`-like objects](/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set#set-like_browser_apis) (the links below are to the {{jsxref("Set")}} global object reference page).

- {{jsxref("Set.prototype.size", "size")}} {{Experimental_Inline}}
  - : Returns the number of values in the set.

## Instance methods

The following methods are available to all read-only [`Set`-like objects](/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set#set-like_browser_apis) (the below links are to the {{jsxref("Set")}} global object reference page).

- {{jsxref("Set.prototype.has()", "has()")}} {{Experimental_Inline}}
  - : Returns a boolean asserting whether an element is present with the given value in the set or not.
- {{jsxref("Set.prototype.values()", "values()")}} {{Experimental_Inline}}
  - : Returns a new iterator object that yields the **values** for each element in the set in insertion order.
- {{jsxref("Set.prototype.keys()", "keys()")}} {{Experimental_Inline}}
  - : An alias for {{jsxref("Set.prototype.values()", "values()")}}.
- {{jsxref("Set.prototype.entries()", "entries()")}} {{Experimental_Inline}}
  - : Returns a new iterator object that contains **an array of `[value, value]`** for each element in the set, in insertion order.
- {{jsxref("Set.prototype.forEach()", "forEach()")}} {{Experimental_Inline}}
  - : Calls a provided callback function once for each value present in the set, in insertion order.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const adapterFeatures = adapter.features;

  // Return the size of the set
  console.log(adapterFeatures.size);

  // Check whether a feature is supported by the adapter
  console.log(adapterFeatures.has("texture-compression-astc"));

  // Iterate through all the set values using values()
  const valueIterator = adapterFeatures.values();
  for (const value of valueIterator) {
    console.log(value);
  }

  // Iterate through all the set values using keys()
  const keyIterator = adapterFeatures.keys();
  for (const value of keyIterator) {
    console.log(value);
  }

  // Iterate through all the set values using entries()
  const entryIterator = adapterFeatures.entries();
  for (const entry of entryIterator) {
    console.log(entry[0]);
  }

  // Iterate through all the set values using forEach()
  adapterFeatures.forEach((value) => {
    console.log(value);
  });

  //...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuadapter/requestdevice/index.md
---
title: "GPUAdapter: requestDevice() method"
short-title: requestDevice()
slug: Web/API/GPUAdapter/requestDevice
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUAdapter.requestDevice
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`requestDevice()`** method of the
{{domxref("GPUAdapter")}} interface returns a {{jsxref("Promise")}} that fulfills with a {{domxref("GPUDevice")}} object, which is the primary interface for communicating with the GPU.

## Syntax

```js-nolint
requestDevice()
requestDevice(descriptor)
```

### Parameters

- `descriptor` {{optional_inline}}
  - : An object containing the following properties:
    - `defaultQueue` {{optional_inline}}
      - : An object that provides information for the device's default {{domxref("GPUQueue")}} (as returned by {{domxref("GPUDevice.queue")}}). This object has a single property ‚Äî `label` ‚Äî which provides the default queue with a {{domxref("GPUQueue.label", "label")}} value. If no value is provided, this defaults to an empty object, and the default queue's label will be an empty string.
    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the {{domxref("GPUDevice")}}, for example in {{domxref("GPUError")}} messages or console warnings.
    - `requiredFeatures` {{optional_inline}}
      - : An array of strings representing additional functionality that you want supported by the returned {{domxref("GPUDevice")}}. The `requestDevice()` call will fail if the `GPUAdapter` cannot provide these features. See {{domxref("GPUSupportedFeatures")}} for a full list of possible features. This defaults to an empty array if no value is provided.
    - `requiredLimits` {{optional_inline}}
      - : An object containing properties representing the limits that you want supported by the returned {{domxref("GPUDevice")}}. The `requestDevice()` call will fail if the `GPUAdapter` cannot provide these limits. Each key must be the name of a member of {{domxref("GPUSupportedLimits")}}. This defaults to an empty object if no value is provided.

> **Note:** Not all features and limits will be available to WebGPU in all browsers that support it, even if they are supported by the underlying hardware. See the {{domxref("GPUAdapter.features", "features")}} and {{domxref("GPUAdapter.limits", "limits")}} pages for more information.

### Return value

A {{jsxref("Promise")}} that fulfills with a {{domxref("GPUDevice")}} object instance.

If you make a duplicate call, i.e. call `requestDevice()` on a {{domxref("GPUAdapter")}} that `requestDevice()` was already called on, the promise fulfills with a device that is immediately lost. You can then get information on how the device was lost via {{domxref("GPUDevice.lost")}}.

### Exceptions

- `OperationError` {{domxref("DOMException")}}
  - : The promise rejects with an `OperationError` if the limits included in the `requiredLimits` property are not supported by the {{domxref("GPUAdapter")}}, either because they are not valid limits, or because their values are higher than the adapter's values for those limits.
- `TypeError` {{domxref("DOMException")}}
  - : The promise rejects with a `TypeError` if the features included in the `requiredFeatures` property are not supported by the {{domxref("GPUAdapter")}}.

## Examples

### Basic example

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const device = await adapter.requestDevice();

  // ...
}
```

### Requesting specific features and limits

In the following code we:

1. Check whether a {{domxref("GPUAdapter")}} has the `texture-compression-astc` feature available. If so, we push it into the array of `requiredFeatures`.
2. Query the `GPUAdapter.limits` value of `maxBindGroups` to see if it is equal to or greater than 6. Our theoretical example app ideally needs 6 bind groups, so if the returned value is >= 6, we add a maximum limit of 6 to the `requiredLimits` object.
3. Request a device with those feature and limit requirements, plus a `defaultQueue` label.

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const requiredFeatures = [];

  if (adapter.features.has("texture-compression-astc")) {
    requiredFeatures.push("texture-compression-astc");
  }

  const requiredLimits = {};

  // App ideally needs 6 bind groups, so we'll try to request what the app needs
  if (adapter.limits.maxBindGroups >= 6) {
    requiredLimits.maxBindGroups = 6;
  }

  const device = await adapter.requestDevice({
    defaultQueue: {
      label: "myqueue",
    },
    requiredFeatures,
    requiredLimits,
  });

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuadapter/isfallbackadapter/index.md
---
title: "GPUAdapter: isFallbackAdapter property"
short-title: isFallbackAdapter
slug: Web/API/GPUAdapter/isFallbackAdapter
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUAdapter.isFallbackAdapter
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`isFallbackAdapter`** read-only property of the
{{domxref("GPUAdapter")}} interface returns `true` if the adapter is a [fallback adapter](/en-US/docs/Web/API/GPU/requestAdapter#fallback_adapters), and `false` if not.

## Value

A boolean.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error('WebGPU not supported.');
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error('Couldn\'t request WebGPU adapter.');
  }

  const fallback = adapter.isFallbackAdapter;
  console.log(fallback);

  // ...

```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuadapter/features/index.md
---
title: "GPUAdapter: features property"
short-title: features
slug: Web/API/GPUAdapter/features
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUAdapter.features
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`features`** read-only property of the
{{domxref("GPUAdapter")}} interface returns a {{domxref("GPUSupportedFeatures")}} object that describes additional functionality supported by the adapter.

You should note that not all features will be available to WebGPU in all browsers that support it, even if the features are supported by the underlying hardware. This could be due to constraints in the underlying system, browser, or adapter. For example:

- The underlying system might not be able to guarantee exposure of a feature in a way that is compatible with a certain browser.
- The browser vendor might not have found a secure way to implement support for that feature, or might just not have gotten round to it yet.

If you are hoping to take advantage of a specific additional feature in a WebGPU app, thorough testing is advised.

## Value

A {{domxref("GPUSupportedFeatures")}} object instance. This is a [setlike](/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set) object.

## Examples

In the following code we check whether a {{domxref("GPUAdapter")}} has the `texture-compression-astc` feature available. If so, we push it into the array of `requiredFeatures`, and request a device with that feature requirement using {{domxref("GPUAdapter.requestDevice()")}}

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const requiredFeatures = [];

  if (adapter.features.has("texture-compression-astc")) {
    requiredFeatures.push("texture-compression-astc");
  }

  const device = await adapter.requestDevice({
    requiredFeatures,
  });

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuadapter/limits/index.md
---
title: "GPUAdapter: limits property"
short-title: limits
slug: Web/API/GPUAdapter/limits
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUAdapter.limits
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`limits`** read-only property of the
{{domxref("GPUAdapter")}} interface returns a {{domxref("GPUSupportedLimits")}} object that describes the limits supported by the adapter.

You should note that, rather than reporting the exact limits of each GPU, browsers will likely report different tier values of different limits to reduce the unique information available to drive-by fingerprinting. For example, the tiers of a certain limit might be 2048, 8192, and 32768. If your GPU's actual limit is 16384, the browser will still report 8192.

Given that different browsers will handle this differently and the tier values may change over time, it is hard to provide an accurate account of what limit values to expect ‚Äî thorough testing is advised.

## Value

A {{domxref("GPUSupportedLimits")}} object instance.

## Examples

In the following code we query the `GPUAdapter.limits` value of `maxBindGroups` to see if it is equal to or greater than 6. Our theoretical example app ideally needs 6 bind groups, so if the returned value is >= 6, we add a maximum limit of 6 to the `requiredLimits` object, and request a device with that limit requirement using {{domxref("GPUAdapter.requestDevice()")}}:

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const requiredLimits = {};

  // App ideally needs 6 bind groups, so we'll try to request what the app needs
  if (adapter.limits.maxBindGroups >= 6) {
    requiredLimits.maxBindGroups = 6;
  }

  const device = await adapter.requestDevice({
    requiredLimits,
  });

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuadapter/index.md
---
title: GPUAdapter
slug: Web/API/GPUAdapter
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUAdapter
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUAdapter`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents a GPU adapter. From this you can request a {{domxref("GPUDevice")}}, adapter info, features, and limits.

A `GPUAdapter` object is requested using the {{domxref("GPU.requestAdapter()")}} method.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUAdapter.features", "features")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A {{domxref("GPUSupportedFeatures")}} object that describes additional functionality supported by the adapter.
- {{domxref("GPUAdapter.isFallbackAdapter", "isFallbackAdapter")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A boolean value. Returns `true` if the adapter is a [fallback adapter](/en-US/docs/Web/API/GPU/requestAdapter#fallback_adapters), and `false` if not.
- {{domxref("GPUAdapter.limits", "limits")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A {{domxref("GPUSupportedLimits")}} object that describes the limits supported by the adapter.

## Instance methods

- {{domxref("GPUAdapter.requestAdapterInfo", "requestAdapterInfo()")}} {{Experimental_Inline}}
  - : Returns a {{jsxref("Promise")}} that fulfills with a {{domxref("GPUAdapterInfo")}} object containing identifying information about an adapter.
- {{domxref("GPUAdapter.requestDevice", "requestDevice()")}} {{Experimental_Inline}}
  - : Returns a {{jsxref("Promise")}} that fulfills with a {{domxref("GPUDevice")}} object, which is the primary interface for communicating with the GPU.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const device = await adapter.requestDevice();

  //...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuadapter/requestadapterinfo/index.md
---
title: "GPUAdapter: requestAdapterInfo() method"
short-title: requestAdapterInfo()
slug: Web/API/GPUAdapter/requestAdapterInfo
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUAdapter.requestAdapterInfo
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`requestAdapterInfo()`** method of the
{{domxref("GPUAdapter")}} interface returns a {{jsxref("Promise")}} that fulfills with a {{domxref("GPUAdapterInfo")}} object containing identifying information about an adapter.

The intention behind this method is to allow developers to request specific details about the user's GPU so that they can preemptively apply workarounds for GPU-specific bugs, or provide different codepaths to better suit different GPU architectures. Providing such information does present a security risk ‚Äî it could be used for fingerprinting ‚Äî therefore the information shared is to be kept at a minimum, and different browser vendors are likely to share different information types and granularities.

> **Note:** The specification includes an `unmaskHints` parameter for `requestAdapterInfo()`, which is intended to mitigate the security risk mentioned above. Once it is supported, developers will be able to specify the values they really need to know, and users will be given a permission prompt asking them if they are OK to share this information when the method is invoked. Browser vendors are likely to share more useful information if it is guarded by a permissions prompt, as it makes the method a less viable target for fingerprinting.

## Syntax

```js-nolint
requestAdapterInfo()
```

### Parameters

None.

### Return value

A {{jsxref("Promise")}} that fulfills with a {{domxref("GPUAdapterInfo")}} object instance.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const adapterInfo = await adapter.requestAdapterInfo();
  console.log(adapterInfo.vendor);
  console.log(adapterInfo.architecture);

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpupipelinelayout/label/index.md
---
title: "GPUPipelineLayout: label property"
short-title: label
slug: Web/API/GPUPipelineLayout/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUPipelineLayout.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** property of the
{{domxref("GPUPipelineLayout")}} interface provides a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUDevice.createPipelineLayout()")}} call, or you can get and set it directly on the `GPUPipelineLayout` object.

## Value

A string. If this has not been previously set as described above, it will be an empty string.

## Examples

Setting and getting a label via `GPUPipelineLayout.label`:

```js
// ...

const pipelineLayout = device.createPipelineLayout({
  bindGroupLayouts: [bindGroupLayout],
});

pipelineLayout.label = "mypipelinelayout";

console.log(pipelineLayout.label); // "mypipelinelayout";
```

Setting a label via the originating {{domxref("GPUDevice.createPipelineLayout()")}} call, and then getting it via `GPUPipelineLayout.label`:

```js
// ...

const pipelineLayout = device.createPipelineLayout({
  bindGroupLayouts: [bindGroupLayout],
  label: "mypipelinelayout",
});

console.log(pipelineLayout.label); // "mypipelinelayout";
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpupipelinelayout/index.md
---
title: GPUPipelineLayout
slug: Web/API/GPUPipelineLayout
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUPipelineLayout
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUPipelineLayout`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} defines the {{domxref("GPUBindGroupLayout")}}s used by a pipeline. {{domxref("GPUBindGroup")}}s used with the pipeline during command encoding must have compatible {{domxref("GPUBindGroupLayout")}}s.

A `GPUPipelineLayout` object instance is created using the {{domxref("GPUDevice.createPipelineLayout()")}} method.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUPipelineLayout.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Examples

> **Note:** The [WebGPU samples](https://webgpu.github.io/webgpu-samples/) feature many more examples.

### Basic pipeline layout example

The following snippet:

- Creates a {{domxref("GPUBindGroupLayout")}} that describes a binding with a buffer, a texture, and a sampler.
- Creates a {{domxref("GPUPipelineLayout")}} based on the {{domxref("GPUBindGroupLayout")}}.

```js
// ...

const bindGroupLayout = device.createBindGroupLayout({
  entries: [
    {
      binding: 0,
      visibility: GPUShaderStage.VERTEX | GPUShaderStage.FRAGMENT,
      buffer: {},
    },
    {
      binding: 1,
      visibility: GPUShaderStage.FRAGMENT,
      texture: {},
    },
    {
      binding: 2,
      visibility: GPUShaderStage.FRAGMENT,
      sampler: {},
    },
  ],
});

const pipelineLayout = device.createPipelineLayout({
  bindGroupLayouts: [bindGroupLayout],
});

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpupipelineerror/gpupipelineerror/index.md
---
title: "GPUPipelineError: GPUPipelineError() constructor"
short-title: GPUPipelineError()
slug: Web/API/GPUPipelineError/GPUPipelineError
page-type: web-api-constructor
status:
  - experimental
browser-compat: api.GPUPipelineError.GPUPipelineError
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUPipelineError()`** constructor creates a new
{{domxref("GPUPipelineError")}} object instance.

## Syntax

```js-nolint
new GPUPipelineError(message, options)
```

### Parameters

- `message` {{optional_inline}}
  - : A string providing a human-readable message that explains why the error occurred. If not specified, `message` defaults to an empty string (`""`).
- `options`
  - : An object, which can contain the following properties:
    - `reason`
      - : An enumerated value that defines the reason the pipeline creation failed in a machine-readable way. The value can be one of:
        - `"internal"`: Pipeline creation failed because of an internal error (see {{domxref("GPUInternalError")}} for more information about these kinds of error).
        - `"validation"`: Pipeline creation failed because of a validation error (see {{domxref("GPUValidationError")}} for more information about these kinds of error).

## Examples

A developer would not manually use the constructor to create a `GPUPipelineError` object. The user agent uses this constructor to create an appropriate object when a {{jsxref("Promise")}} returned by a {{domxref("GPUDevice.createComputePipelineAsync()")}} or {{domxref("GPUDevice.createRenderPipelineAsync()")}} call rejects, signalling a pipeline failure.

See the main [`GPUPipelineError`](/en-US/docs/Web/API/GPUPipelineError#examples) page for an example involving a `GPUPipelineError` object instance.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling)
-e 

File: /files/en-us/web/api/gpupipelineerror/index.md
---
title: GPUPipelineError
slug: Web/API/GPUPipelineError
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUPipelineError
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUPipelineError`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} describes a pipeline failure. This is the value received when a {{jsxref("Promise")}} returned by a {{domxref("GPUDevice.createComputePipelineAsync()")}} or {{domxref("GPUDevice.createRenderPipelineAsync()")}} call rejects.

{{InheritanceDiagram}}

## Constructor

- {{domxref("GPUPipelineError.GPUPipelineError", "GPUPipelineError()")}} {{Experimental_Inline}}
  - : Creates a new `GPUPipelineError` object instance.

## Instance properties

_Inherits properties from its parent, {{domxref("DOMException")}}._

- {{domxref("GPUPipelineError.reason", "reason")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : An enumerated value that defines the reason the pipeline creation failed in a machine-readable way.

## Examples

In the following snippet we are attempting to create a {{domxref("GPUComputePipeline")}} using {{domxref("GPUDevice.createComputePipelineAsync()")}}. However, we have misspelt our compute pipeline `entryPoint` as `"maijn"` (it should be `"main"`), therefore pipeline creation fails, and our `catch` block prints the resulting reason and error message to the console.

```js
// ...

let computePipeline;

try {
  computePipeline = await device.createComputePipelineAsync({
    layout: device.createPipelineLayout({
      bindGroupLayouts: [bindGroupLayout],
    }),
    compute: {
      module: shaderModule,
      entryPoint: "maijn",
    },
  });
} catch (error) {
  // error is a GPUPipelineError object instance
  console.error(error.reason);
  console.error(`Pipeline creation failed: ${error.message}`);
}

// ...
```

In this case, the given `reason` is `"Validation"`, and the `message` is `"Entry point "maijn" doesn't exist in the shader module [ShaderModule]."`

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling)
-e 

File: /files/en-us/web/api/gpupipelineerror/reason/index.md
---
title: "GPUPipelineError: reason property"
short-title: reason
slug: Web/API/GPUPipelineError/reason
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUPipelineError.reason
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`reason`** read-only property of the
{{domxref("GPUPipelineError")}} interface defines the reason the pipeline creation failed in a machine-readable way.

## Value

An enumerated value that can be one of:

- `"internal"`
  - : Pipeline creation failed because of an internal error (see {{domxref("GPUInternalError")}} for more information about these kinds of error.)
- `"validation"`
  - : Pipeline creation failed because of a validation error (see {{domxref("GPUValidationError")}} for more information about these kinds of error.)

## Examples

See the main [`GPUPipelineError`](/en-US/docs/Web/API/GPUPipelineError#examples) page for an example involving a `GPUPipelineError` object instance.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpipeline/label/index.md
---
title: "GPURenderPipeline: label property"
short-title: label
slug: Web/API/GPURenderPipeline/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPURenderPipeline.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** property of the
{{domxref("GPURenderPipeline")}} interface provides a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUDevice.createRenderPipeline()")}} or {{domxref("GPUDevice.createRenderPipelineAsync()")}} call, or you can get and set it directly on the `GPURenderPipeline` object.

## Value

A string. If this has not been previously set as described above, it will be an empty string.

## Examples

Setting and getting a label via `GPURenderPipeline.label`:

```js
// ...

const pipelineDescriptor = {
  vertex: {
    module: shaderModule,
    entryPoint: "vertex_main",
    buffers: vertexBuffers,
  },
  fragment: {
    module: shaderModule,
    entryPoint: "fragment_main",
    targets: [
      {
        format: navigator.gpu.getPreferredCanvasFormat(),
      },
    ],
  },
  primitive: {
    topology: "triangle-list",
  },
  layout: "auto",
};

const renderPipeline = device.createRenderPipeline(pipelineDescriptor);

renderPipeline.label = "myrenderpipeline";

console.log(renderPipeline.label); // "myrenderpipeline"
```

Setting a label via a {{domxref("GPUDevice.createRenderPipeline()")}} call, and then getting it via `GPURenderPipeline.label`:

```js
// ...

const pipelineDescriptor = {
  vertex: {
    module: shaderModule,
    entryPoint: "vertex_main",
    buffers: vertexBuffers,
  },
  fragment: {
    module: shaderModule,
    entryPoint: "fragment_main",
    targets: [
      {
        format: navigator.gpu.getPreferredCanvasFormat(),
      },
    ],
  },
  primitive: {
    topology: "triangle-list",
  },
  layout: "auto",
  label: "myrenderpipeline",
};

const renderPipeline = device.createRenderPipeline(pipelineDescriptor);

console.log(renderPipeline.label); // "myrenderpipeline"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpipeline/index.md
---
title: GPURenderPipeline
slug: Web/API/GPURenderPipeline
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPURenderPipeline
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPURenderPipeline`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents a pipeline that controls the vertex and fragment shader stages and can be used in a {{domxref("GPURenderPassEncoder")}} or {{domxref("GPURenderBundleEncoder")}}.

A `GPURenderPipeline` object instance can be created using the {{domxref("GPUDevice.createRenderPipeline()")}} or {{domxref("GPUDevice.createRenderPipelineAsync()")}} methods.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPURenderPipeline.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Instance methods

- {{domxref("GPURenderPipeline.getBindGroupLayout", "getBindGroupLayout()")}} {{Experimental_Inline}}
  - : Returns the pipeline's {{domxref("GPUBindGroupLayout")}} object with the given index (i.e. included in the originating {{domxref("GPUDevice.createRenderPipeline()")}} or {{domxref("GPUDevice.createRenderPipelineAsync()")}} call's pipeline layout).

## Examples

> **Note:** The [WebGPU samples](https://webgpu.github.io/webgpu-samples/) feature many more examples.

### Basic example

Our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/) provides a simple example of the construction of a valid render pipeline descriptor object, which is then used to create a `GPURenderPipeline` via a `createRenderPipeline()` call.

```js
// ...

const vertexBuffers = [
  {
    attributes: [
      {
        shaderLocation: 0, // position
        offset: 0,
        format: "float32x4",
      },
      {
        shaderLocation: 1, // color
        offset: 16,
        format: "float32x4",
      },
    ],
    arrayStride: 32,
    stepMode: "vertex",
  },
];

const pipelineDescriptor = {
  vertex: {
    module: shaderModule,
    entryPoint: "vertex_main",
    buffers: vertexBuffers,
  },
  fragment: {
    module: shaderModule,
    entryPoint: "fragment_main",
    targets: [
      {
        format: navigator.gpu.getPreferredCanvasFormat(),
      },
    ],
  },
  primitive: {
    topology: "triangle-list",
  },
  layout: "auto",
};

const renderPipeline = device.createRenderPipeline(pipelineDescriptor);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpipeline/getbindgrouplayout/index.md
---
title: "GPURenderPipeline: getBindGroupLayout() method"
short-title: getBindGroupLayout()
slug: Web/API/GPURenderPipeline/getBindGroupLayout
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPipeline.getBindGroupLayout
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`getBindGroupLayout()`** method of the
{{domxref("GPURenderPipeline")}} interface returns the pipeline's {{domxref("GPUBindGroupLayout")}} object with the given index (i.e. included in the originating {{domxref("GPUDevice.createRenderPipeline()")}} or {{domxref("GPUDevice.createRenderPipelineAsync()")}} call's pipeline layout).

If the {{domxref("GPURenderPipeline")}} was created with `layout: "auto"`, this method is the only way to retrieve the {{domxref("GPUBindGroupLayout")}}s generated by the pipeline.

## Syntax

```js-nolint
getBindGroupLayout(index)
```

### Parameters

- `index`

  - : A number representing the index of the {{domxref("GPUBindGroupLayout")}} to return.

### Return value

A {{domxref("GPUBindGroupLayout")}} object instance.

### Validation

The following criteria must be met when calling **`getBindGroupLayout()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPUBindGroupLayout")}} object is returned:

- `index` is less than the number of {{domxref("GPUBindGroupLayout")}} objects used in the pipeline layout.

## Examples

> **Note:** You can see complete working examples with `getBindGroupLayout()` in action in the [WebGPU samples](https://webgpu.github.io/webgpu-samples/).

```js
// ...

// Create a render pipeline using layout: "auto" to automatically generate
// appropriate bind group layouts
const fullscreenQuadPipeline = device.createRenderPipeline({
  layout: "auto",
  vertex: {
    module: device.createShaderModule({
      code: fullscreenTexturedQuadWGSL,
    }),
    entryPoint: "vert_main",
  },
  fragment: {
    module: device.createShaderModule({
      code: fullscreenTexturedQuadWGSL,
    }),
    entryPoint: "frag_main",
    targets: [
      {
        format: presentationFormat,
      },
    ],
  },
  primitive: {
    topology: "triangle-list",
  },
});

// ...

// Create a bind group with the auto-generated layout from the render pipeline
const showResultBindGroup = device.createBindGroup({
  layout: fullscreenQuadPipeline.getBindGroupLayout(0),
  entries: [
    {
      binding: 0,
      resource: sampler,
    },
    {
      binding: 1,
      resource: textures[1].createView(),
    },
  ],
});

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpusupportedlimits/index.md
---
title: GPUSupportedLimits
slug: Web/API/GPUSupportedLimits
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUSupportedLimits
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUSupportedLimits`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} describes the limits supported by a {{domxref("GPUAdapter")}}.

The `GPUSupportedLimits` object for the current adapter is accessed via the {{domxref("GPUAdapter.limits")}} property.

You should note that, rather than reporting the exact limits of each GPU, browsers will likely report different tier values of different limits to reduce the unique information available to drive-by fingerprinting. For example, the tiers of a certain limit might be 2048, 8192, and 32768. If your GPU's actual limit is 16384, the browser will still report 8192.

Given that different browsers will handle this differently and the tier values may change over time, it is hard to provide an accurate account of what limit values to expect ‚Äî thorough testing is advised.

{{InheritanceDiagram}}

## Instance properties

The following limits are represented by properties in a `GPUSupportedLimits` object. See the [Limits](https://gpuweb.github.io/gpuweb/#limits) section of the specification for detailed descriptions of what the limits relate to.

| Limit name                                  | Default value            |
| ------------------------------------------- | ------------------------ |
| `maxTextureDimension1D`                     | 8192                     |
| `maxTextureDimension2D`                     | 8192                     |
| `maxTextureDimension3D`                     | 2048                     |
| `maxTextureArrayLayers`                     | 256                      |
| `maxBindGroups`                             | 4                        |
| `maxBindingsPerBindGroup`                   | 640                      |
| `maxDynamicUniformBuffersPerPipelineLayout` | 8                        |
| `maxDynamicStorageBuffersPerPipelineLayout` | 4                        |
| `maxSampledTexturesPerShaderStage`          | 16                       |
| `maxSamplersPerShaderStage`                 | 16                       |
| `maxStorageBuffersPerShaderStage`           | 8                        |
| `maxStorageTexturesPerShaderStage`          | 4                        |
| `maxUniformBuffersPerShaderStage`           | 12                       |
| `maxUniformBufferBindingSize`               | 65536 bytes              |
| `maxStorageBufferBindingSize`               | 134217728 bytes (128 MB) |
| `minUniformBufferOffsetAlignment`           | 256 bytes                |
| `minStorageBufferOffsetAlignment`           | 256 bytes                |
| `maxVertexBuffers`                          | 8                        |
| `maxBufferSize`                             | 268435456 bytes (256 MB) |
| `maxVertexAttributes`                       | 16                       |
| `maxVertexBufferArrayStride`                | 2048 bytes               |
| `maxInterStageShaderComponents`             | 60                       |
| `maxInterStageShaderVariables`              | 16                       |
| `maxColorAttachments`                       | 8                        |
| `maxColorAttachmentBytesPerSample`          | 32                       |
| `maxComputeWorkgroupStorageSize`            | 16384 bytes              |
| `maxComputeInvocationsPerWorkgroup`         | 256                      |
| `maxComputeWorkgroupSizeX`                  | 256                      |
| `maxComputeWorkgroupSizeY`                  | 256                      |
| `maxComputeWorkgroupSizeZ`                  | 64                       |
| `maxComputeWorkgroupsPerDimension`          | 65535                    |

## Examples

In the following code we query the `GPUAdapter.limits` value of `maxBindGroups` to see if it is equal to or greater than 6. Our theoretical example app ideally needs 6 bind groups, so if the returned value is >= 6, we add a maximum limit of 6 to the `requiredLimits` object. We then request a device with that limit requirement using {{domxref("GPUAdapter.requestDevice()")}}:

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const requiredLimits = {};

  // App ideally needs 6 bind groups, so we'll try to request what the app needs
  if (adapter.limits.maxBindGroups >= 6) {
    requiredLimits.maxBindGroups = 6;
  }

  const device = await adapter.requestDevice({
    requiredLimits,
  });

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuqueue/writebuffer/index.md
---
title: "GPUQueue: writeBuffer() method"
short-title: writeBuffer()
slug: Web/API/GPUQueue/writeBuffer
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUQueue.writeBuffer
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`writeBuffer()`** method of the
{{domxref("GPUQueue")}} interface writes a provided data source into a given {{domxref("GPUBuffer")}}.

This is a convenience function, which provides an alternative to setting buffer data via buffer mapping and buffer-to-buffer copies. It lets the user agent determine the most efficient way to copy the data over.

## Syntax

```js-nolint
writeBuffer(buffer, bufferOffset, data, dataOffset, size)
```

### Parameters

- `buffer`
  - : A {{domxref("GPUBuffer")}} object representing the buffer to write data to.
- `bufferOffset`
  - : A number representing the offset, in bytes, to start writing the data at inside the {{domxref("GPUBuffer")}}.
- `data`
  - : An object representing the data source to write into the {{domxref("GPUBuffer")}}. This can be an {{jsxref("ArrayBuffer")}}, {{jsxref("TypedArray")}}, or {{jsxref("DataView")}}.
- `dataOffset` {{optional_inline}}
  - : A number representing the offset to start writing the data from inside the data source. This value is a number of elements if `data` is a {{jsxref("TypedArray")}}, and a number of bytes if not. If omitted, `dataOffset` defaults to 0.
- `size` {{optional_inline}}
  - : A number representing the size of the content to write from `data` to `buffer`. This value is a number of elements if `data` is a {{jsxref("TypedArray")}}, and a number of bytes if not. If omitted, `size` will be equal to the overall size of `data`, minus `dataOffset`.

### Return value

None ({{jsxref("Undefined")}}).

### Exceptions

- `OperationError` {{domxref("DOMException")}}
  - : The method throws an `OperationError` if the following criteria are not met:
    - The size of `data` is equal to or greater than 0.
    - `dataOffset` is equal to or smaller than the size of `data`.
    - The size of `data` (when converted to bytes, in the case of `TypedArray`s) is a multiple of 4.

### Validation

The following criteria must be met when calling **`writeBuffer()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUQueue")}} becomes invalid:

- `buffer` is available for use, i.e. not unavailable (`GPUBuffer`s are unavailable if they are currently {{domxref("GPUBuffer.mapAsync", "mapped", "", "nocode")}}) or destroyed (with the {{domxref("GPUBuffer.destroy()")}} method).
- The `buffer`'s {{domxref("GPUBuffer.usage")}} includes the `GPUBufferUsage.COPY_DST` flag.
- `bufferOffset`, when converted to bytes, is a multiple of 4.
- The size of `data` - `dataOffset` + `bufferOffset`, when converted to bytes, is equal to or less than the `buffer`'s {{domxref("GPUBuffer.size")}}.

## Examples

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/), we define some vertex data in a {{jsxref("Float32Array")}} that we'll use to draw a triangle:

```js
const vertices = new Float32Array([
  0.0, 0.6, 0, 1, 1, 0, 0, 1, -0.5, -0.6, 0, 1, 0, 1, 0, 1, 0.5, -0.6, 0, 1, 0,
  0, 1, 1,
]);
```

To use this data in a render pipeline, we need to put it into a {{domxref("GPUBuffer")}}. First we'll create the buffer:

```js
const vertexBuffer = device.createBuffer({
  size: vertices.byteLength, // make it big enough to store vertices in
  usage: GPUBufferUsage.VERTEX | GPUBufferUsage.COPY_DST,
});
```

To get the data into the buffer we can use `writeBuffer()`:

```js
device.queue.writeBuffer(vertexBuffer, 0, vertices, 0, vertices.length);
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuqueue/copyexternalimagetotexture/index.md
---
title: "GPUQueue: copyExternalImageToTexture() method"
short-title: copyExternalImageToTexture()
slug: Web/API/GPUQueue/copyExternalImageToTexture
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUQueue.copyExternalImageToTexture
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`copyExternalImageToTexture()`** method of the
{{domxref("GPUQueue")}} interface copies a snapshot taken from a source image, video, or canvas into a given {{domxref("GPUTexture")}}.

Using this function allows the user agent to determine the most efficient way to copy the data over for each source type.

## Syntax

```js-nolint
copyExternalImageToTexture(source, destination, copySize)
```

### Parameters

- `source`

  - : An object representing the source to write to the destination, and its origin. This can take the following properties:

    - `source`
      - : An object providing the source of the snapshot to copy. This can be an {{domxref("ImageBitmap")}}, {{domxref("HTMLVideoElement")}}, {{domxref("VideoFrame")}}, {{domxref("HTMLCanvasElement")}}, or {{domxref("OffscreenCanvas")}}. The image source data is captured at the exact moment `copyExternalImageToTexture()` is invoked.
    - `origin` {{optional_inline}}

      - : An object or array specifying the origin of the copy ‚Äî the top-left corner of the source sub-region to copy from. Together with `copySize`, this defines the full extent of the source sub-region. The `x` and `y` values default to 0 if any of all of `origin` is omitted.

        What follows is a sample array:

        ```js
        origin: [0, 0];
        ```

        The object equivalent would look like this:

        ```js
        origin: {
          x: 0,
          y: 0
        }
        ```

    - `flipY` {{optional_inline}}
      - : A boolean. If set to `true`, the image capture is flipped vertically. If omitted, `flipY` defaults to `false`.

- `destination`

  - : An object defining the texture subresource and origin to write the captured image to, plus encoding metadata. This can take the following properties:

    - `aspect` {{optional_inline}}

      - : An enumerated value defining which aspects of the texture to write the image to. Possible values are:

        - `"all"`
          - : All available aspects of the texture format will be written to, which can mean all or any of color, depth, and stencil, depending on what kind of format you are dealing with.
        - `"depth-only"`
          - : Only the depth aspect of a [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format) will be written to.
        - `"stencil-only"`
          - : Only the stencil aspect of a depth-or-stencil format will be written to.

        If omitted, `aspect` takes a value of `"all"`.

    - `colorSpace` {{optional_inline}}

      - : An enumerated value describing the color space and encoding used to encode data into the destination texture. Possible values are `"srgb"` and `"display-p3"`. If omitted, `colorSpace` defaults to `"srgb"`.

        > **Note:** The encoding may result in values outside of the range `[0, 1]` being written to the target texture, if its format can represent them. Otherwise, the results are clamped to the target texture format's range. Conversion may not be necessary if `colorSpace` matches the source image color space.

    - `mipLevel` {{optional_inline}}
      - : A number representing the mip-map level of the texture to write the image to. If omitted, `mipLevel` defaults to 0.
    - `origin` {{optional_inline}}

      - : An object or array specifying the origin of the copy ‚Äî the minimum corner of the texture region to write the image data to. Together with `copySize`, this defines the full extent of the region to copy to. The `x`, `y`, and `z` values default to 0 if any of all of `origin` is omitted.

        What follows is a sample array:

        ```js
        origin: [0, 0, 0];
        ```

        The object equivalent would look like this:

        ```js
        origin: {
          x: 0,
          y: 0,
          z: 0
        }
        ```

    - `premultipliedAlpha` {{optional_inline}}

      - : A boolean. If set to `true`, the image data written into the texture will have its RGB channels premultiplied by the alpha channel. If omitted, `premultipliedAlpha` defaults to `false`.

        > **Note:** If this option is set to `true` and the `source` is also premultiplied, the source RGB values must be preserved even if they exceed their corresponding alpha values.

    - `texture`
      - : A {{domxref("GPUTexture")}} object representing the texture to write the data to.

- `copySize`

  - : An object or array specifying `width`, `height`, and `depthOrArrayLayers` ‚Äî of the region to copy from/to.

    What follows is a sample array:

    ```js
    origin: [16, 1, 1];
    ```

    The object equivalent would look like this:

    ```js
    origin: {
      width: 16,
      height: 1,
      depthOrArrayLayers: 1
    }
    ```

    The `width` value has to be included. If the `height` or `depthOrArrayLayers` values are omitted, they default to 1.

### Return value

None ({{jsxref("Undefined")}}).

### Exceptions

- `OperationError` {{domxref("DOMException")}}
  - : The method throws an `OperationError` if the following criteria are not met:
    - `source.origin.x` + the width of the region to copy to is less than or equal to the width of the source image.
    - `source.origin.y` + the height of the region to copy to is less than or equal to the height of the source image.
    - `source.origin.z` + the depthOrArrayLayers of the region to copy to is less than or equal to 1.
    - `dataOffset` is equal to or smaller than the size of `data`.
    - The size of `data` (when converted to bytes, in the case of `TypedArray`s) is a multiple of 4.
- `SecurityError` {{domxref("DOMException")}}
  - : Thrown if the image source data is cross-origin.

### Validation

The following criteria must be met when calling **`writeTexture()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUQueue")}} becomes invalid:

- `mipLevel` is less than the destination {{domxref("GPUTexture.mipLevelCount")}}.
- `origin.x` is a multiple of the texel block width of the destination {{domxref("GPUTexture.format")}}.
- `origin.y` is a multiple of the texel block height of the destination {{domxref("GPUTexture.format")}}.
- If the destination {{domxref("GPUTexture.format")}} is a [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format), the image capture size is equal to `size`.
- The destination {{domxref("GPUTexture.usage")}} includes the `GPUTextureUsage.COPY_DST` and `GPUTextureUsage.RENDER_ATTACHMENT` flags.
- The destination {{domxref("GPUTexture.dimension")}} is `"2d"`.
- The destination {{domxref("GPUTexture.sampleCount")}} is 1.
- The destination {{domxref("GPUTexture.format")}} is one of the following (which support `GPUTextureUsage.RENDER_ATTACHMENT` usage):
  - `"r8unorm"`
  - `"r16float"`
  - `"r32float"`
  - `"rg8unorm"`
  - `"rg16float"`
  - `"rg32float"`
  - `"rgba8unorm"`
  - `"rgba8unorm-srgb"`
  - `"bgra8unorm"`
  - `"bgra8unorm-srgb"`
  - `"rgb10a2unorm"`
  - `"rgba16float"`
  - `"rgba32float"`
- `destination.origin.x` + `copySize.width` is less than or equal to the `destination` {{domxref("GPUTexture")}} {{domxref("GPUTexture.width", "width")}}.
- `destination.origin.y` + `copySize.height` is less than or equal to the `destination` {{domxref("GPUTexture")}} {{domxref("GPUTexture.height", "height")}}.
- `destination.origin.z` + `copySize.depthOrArrayLayers` is less than or equal to the `destination` {{domxref("GPUTexture")}} {{domxref("GPUTexture.depthOrArrayLayers", "depthOrArrayLayers")}}.
- The `destination` {{domxref("GPUTexture.width")}} is a multiple of the texel block width of the destination {{domxref("GPUTexture.format")}}.
- The `destination` {{domxref("GPUTexture.height")}} is a multiple of the texel block height of the destination {{domxref("GPUTexture.format")}}.

## Examples

In the WebGPU Samples [Textured Cube example](https://webgpu.github.io/webgpu-samples/samples/texturedCube), the following snippet is used to fetch an image and upload it into a {{domxref("GPUTexture")}}:

```js
let cubeTexture: GPUTexture; // TypeScript
{
  const img = document.createElement("img");
  img.src = new URL(
    "../../../assets/img/Di-3d.png",
    import.meta.url
  ).toString();
  await img.decode();
  const imageBitmap = await createImageBitmap(img);

  cubeTexture = device.createTexture({
    size: [imageBitmap.width, imageBitmap.height, 1],
    format: "rgba8unorm",
    usage:
      GPUTextureUsage.TEXTURE_BINDING |
      GPUTextureUsage.COPY_DST |
      GPUTextureUsage.RENDER_ATTACHMENT,
  });

  device.queue.copyExternalImageToTexture(
    { source: imageBitmap },
    { texture: cubeTexture },
    [imageBitmap.width, imageBitmap.height]
  );
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuqueue/submit/index.md
---
title: "GPUQueue: submit() method"
short-title: submit()
slug: Web/API/GPUQueue/submit
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUQueue.submit
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`submit()`** method of the
{{domxref("GPUQueue")}} interface schedules the execution of command buffers represented by one or more {{domxref("GPUCommandBuffer")}} objects by the GPU.

## Syntax

```js-nolint
submit(commandBuffers)
```

### Parameters

- `commandBuffers`
  - : An array of {{domxref("GPUCommandBuffer")}} objects containing the commands to be enqueued for processing by the GPU.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`submit()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUQueue")}} becomes invalid:

- Any {{domxref("GPUBuffer")}}, {{domxref("GPUTexture")}}, and {{domxref("GPUQuerySet")}} objects used in the encoded commands are available for use, i.e. not unavailable (`GPUBuffer`s are unavailable if they are currently {{domxref("GPUBuffer.mapAsync", "mapped", "", "nocode")}}) or destroyed (with the `destroy()` method).
- Any {{domxref("GPUExternalTexture")}} objects used in the encoded commands are not expired (they expire automatically shortly after being imported via {{domxref("GPUDevice.importExternalTexture", "importExternalTexture()")}}).
- If a {{domxref("GPUQuerySet")}} object used in an encoded command is of type `"occlusion"` query, it is not already used, except by {{domxref("GPURenderPassEncoder.beginOcclusionQuery()")}}.

## Examples

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/), a number of commands are recorded via a {{domxref("GPUCommandEncoder")}}:

```js
// ...

// Create GPUCommandEncoder
const commandEncoder = device.createCommandEncoder();

// Create GPURenderPassDescriptor to tell WebGPU which texture to draw into, then initiate render pass

const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
};

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// Draw a triangle

passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

// End the render pass

passEncoder.end();

// ...
```

The commands encoded by the {{domxref("GPUCommandEncoder")}} are recoded into a {{domxref("GPUCommandBuffer")}} using the {{domxref("GPUCommandEncoder.finish()")}} method. The command buffer is then passed into the queue via a {{domxref("GPUQueue.submit", "submit()")}} call, ready to be processed by the GPU.

```js
device.queue.submit([commandEncoder.finish()]);
```

> **Note:** Study the [WebGPU samples](https://webgpu.github.io/webgpu-samples/) to find more queue examples.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuqueue/writetexture/index.md
---
title: "GPUQueue: writeTexture() method"
short-title: writeTexture()
slug: Web/API/GPUQueue/writeTexture
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUQueue.writeTexture
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`writeTexture()`** method of the
{{domxref("GPUQueue")}} interface writes a provided data source into a given {{domxref("GPUTexture")}}.

This is a convenience function, which provides an alternative to setting texture data via buffer mapping and buffer-to-texture copies. It lets the user agent determine the most efficient way to copy the data over.

## Syntax

```js-nolint
writeTexture(destination, data, dataLayout, size)
```

### Parameters

- `destination`

  - : An object defining the texture subresource and origin to write the data source to, which can take the following properties:

    - `aspect` {{optional_inline}}

      - : An enumerated value defining which aspects of the texture to write the data to. Possible values are:

        - `"all"`
          - : All available aspects of the texture format will be written to, which can mean all or any of color, depth, and stencil, depending on what kind of format you are dealing with.
        - `"depth-only"`
          - : Only the depth aspect of a [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format) will be written to.
        - `"stencil-only"`
          - : Only the stencil aspect of a depth-or-stencil format will be written to.

        If omitted, `aspect` takes a value of `"all"`.

    - `mipLevel` {{optional_inline}}
      - : A number representing the mip-map level of the texture to write the data to. If omitted, `mipLevel` defaults to 0.
    - `origin` {{optional_inline}}

      - : An object or array specifying the origin of the copy ‚Äî the minimum corner of the texture region to write the data to. Together with `size`, this defines the full extent of the region to copy to. The `x`, `y`, and `z` values default to 0 if any of all of `origin` is omitted.

        What follows is a sample array:

        ```js
        origin: [0, 0, 0];
        ```

        The object equivalent would look like this:

        ```js
        origin: {
          x: 0,
          y: 0,
          z: 0
        }
        ```

    - `texture`
      - : A {{domxref("GPUTexture")}} object representing the texture to write the data to.

- `data`
  - : An object representing the data source to write into the {{domxref("GPUTexture")}}. This can be an {{jsxref("ArrayBuffer")}}, {{jsxref("TypedArray")}}, or {{jsxref("DataView")}}.
- `dataLayout`
  - : An object that defines the layout of the content contained in `data`. Possible values are:
    - `offset` {{optional_inline}}
      - : The offset, in bytes, from the beginning of `data` to the start of the image data to be copied. If omitted, `offset` defaults to 0.
    - `bytesPerRow` {{optional_inline}}
      - : A number representing the stride, in bytes, between the start of each block row (i.e. a row of complete texel blocks) and the subsequent block row. This is required if there are multiple block rows (i.e. the copy height or depth is more than one block).
    - `rowsPerImage` {{optional_inline}}
      - : The number of block rows per single image of the texture. `bytesPerRow` &times; `rowsPerImage` will give you the stride, in bytes, between the start of each complete image. This is required if there are multiple images to copy.
- `size`
  - : An object or array specifying the extent of the copy ‚Äî the far corner of the texture region to write the data to. Together with `destination.origin`, this defines the full extent of the region to copy to. See `destination.origin` for examples of the object/array structure.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`writeTexture()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUQueue")}} becomes invalid:

- `mipLevel` is less than the destination {{domxref("GPUTexture.mipLevelCount")}}.
- `origin.x` is a multiple of the texel block width of the destination {{domxref("GPUTexture.format")}}.
- `origin.y` is a multiple of the texel block height of the destination {{domxref("GPUTexture.format")}}.
- If the destination {{domxref("GPUTexture.format")}} is a [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format) or {{domxref("GPUTexture.sampleCount")}} is more than 1, the subresource size is equal to `size`.
- The destination {{domxref("GPUTexture.usage")}} includes the `GPUTextureUsage.COPY_DST` flag.
- The destination {{domxref("GPUTexture.sampleCount")}} is 1.
- `destination.origin.x` + the `destination` {{domxref("GPUTexture.width")}} is less than or equal to the width of the subresource to write to the `destination` {{domxref("GPUTexture")}}.
- `destination.origin.y` + the `destination` {{domxref("GPUTexture.height")}} is less than or equal to the height of the subresource to write to the `destination` {{domxref("GPUTexture")}}.
- `destination.origin.z` + the `destination` {{domxref("GPUTexture.depthOrArrayLayers")}} is less than or equal to the depthOrArrayLayers of the subresource to write to the `destination` {{domxref("GPUTexture")}}.
- The `destination` {{domxref("GPUTexture.width")}} is a multiple of the texel block width of the destination {{domxref("GPUTexture.format")}}.
- The `destination` {{domxref("GPUTexture.height")}} is a multiple of the texel block height of the destination {{domxref("GPUTexture.format")}}.
- `destination.aspect` refers to a single aspect of the destination {{domxref("GPUTexture.format")}}.
- That aspect is a valid image copy destination according to [depth-or-stencil formats](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format).
- The `destination` is otherwise compatible with the {{domxref("GPUTexture.format")}}.

## Examples

In [Efficiently rendering glTF models](https://toji.github.io/webgpu-gltf-case-study/), a function is defined for creating a solid color texture:

```js
function createSolidColorTexture(r, g, b, a) {
  const data = new Uint8Array([r * 255, g * 255, b * 255, a * 255]);
  const texture = device.createTexture({
    size: { width: 1, height: 1 },
    format: "rgba8unorm",
    usage: GPUTextureUsage.TEXTURE_BINDING | GPUTextureUsage.COPY_DST,
  });
  device.queue.writeTexture({ texture }, data, {}, { width: 1, height: 1 });
  return texture;
}
```

This can be used to define standard textures for use in material libraries:

```js
const opaqueWhiteTexture = createSolidColorTexture(1, 1, 1, 1);
const transparentBlackTexture = createSolidColorTexture(0, 0, 0, 0);
const defaultNormalTexture = createSolidColorTexture(0.5, 0.5, 1, 1);
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuqueue/label/index.md
---
title: "GPUQueue: label property"
short-title: label
slug: Web/API/GPUQueue/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUQueue.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** read-only property of the
{{domxref("GPUQueue")}} interface is a string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

You can get and set it directly on the `GPUQueue` object.

## Value

A string. If no label value has previously been set, getting the label returns an empty string.

## Examples

Setting and getting a label via `GPUQueue.label`:

```js
device.queue.label = "myqueue";
console.log(device.queue.label); // "myqueue"
```

You can also set the queue's label at the time you request the device, like this:

```js
const device = adapter.requestDevice({
  defaultQueue: { label: "myqueue" },
});
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuqueue/index.md
---
title: GPUQueue
slug: Web/API/GPUQueue
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUQueue
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUQueue`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} controls execution of encoded commands on the GPU.

A device's primary queue is accessed via the {{domxref("GPUDevice.queue")}} property.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUQueue.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Instance methods

- {{domxref("GPUQueue.copyExternalImageToTexture", "copyExternalImageToTexture()")}} {{Experimental_Inline}}
  - : Copies a snapshot taken from a source image, video, or canvas into a given {{domxref("GPUTexture")}}.
- {{domxref("GPUQueue.onSubmittedWorkDone", "onSubmittedWorkDone()")}} {{Experimental_Inline}}
  - : Returns a {{jsxref("Promise")}} that resolves when all the work submitted to the GPU via this `GPUQueue` at the point the method is called has been processed.
- {{domxref("GPUQueue.submit", "submit()")}} {{Experimental_Inline}}
  - : Schedules the execution of command buffers represented by one or more {{domxref("GPUCommandBuffer")}} objects by the GPU.
- {{domxref("GPUQueue.writeBuffer", "writeBuffer()")}} {{Experimental_Inline}}
  - : Writes a provided data source into a given {{domxref("GPUBuffer")}}.
- {{domxref("GPUQueue.writeTexture", "writeTexture()")}} {{Experimental_Inline}}
  - : Writes a provided data source into a given {{domxref("GPUTexture")}}.

## Examples

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/), we define some vertex data in a {{jsxref("Float32Array")}} that we'll use to draw a triangle:

```js
const vertices = new Float32Array([
  0.0, 0.6, 0, 1, 1, 0, 0, 1, -0.5, -0.6, 0, 1, 0, 1, 0, 1, 0.5, -0.6, 0, 1, 0,
  0, 1, 1,
]);
```

To use this data in a render pipeline, we need to put it into a {{domxref("GPUBuffer")}}. First we'll create the buffer:

```js
const vertexBuffer = device.createBuffer({
  size: vertices.byteLength, // make it big enough to store vertices in
  usage: GPUBufferUsage.VERTEX | GPUBufferUsage.COPY_DST,
});
```

To get the data into the buffer we can use the {{domxref("GPUQueue.writeBuffer", "writeBuffer()")}} function, which lets the user agent determine most efficient way to copy the data over:

```js
device.queue.writeBuffer(vertexBuffer, 0, vertices, 0, vertices.length);
```

Later on, a set of commands is encoded into a {{domxref("GPUCommandBuffer")}} using the {{domxref("GPUCommandEncoder.finish()")}} method. The command buffer is then passed into the queue via a {{domxref("GPUQueue.submit", "submit()")}} call, ready to be processed by the GPU.

```js
device.queue.submit([commandEncoder.finish()]);
```

> **Note:** Study the [WebGPU samples](https://webgpu.github.io/webgpu-samples/) to find more queue examples.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuqueue/onsubmittedworkdone/index.md
---
title: "GPUQueue: onSubmittedWorkDone() method"
short-title: onSubmittedWorkDone()
slug: Web/API/GPUQueue/onSubmittedWorkDone
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUQueue.onSubmittedWorkDone
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`onSubmittedWorkDone()`** method of the
{{domxref("GPUQueue")}} interface returns a {{jsxref("Promise")}} that resolves when all the work submitted to the GPU via this `GPUQueue` at the point the method is called has been processed.

This includes the completion of any {{domxref("GPUBuffer.mapAsync", "mapAsync()")}} calls made on `GPUBuffer`s used in commands submitted to the queue, before `onSubmittedWorkDone()` is called.

Note: In most cases, you do _not_ need to call `onSubmittedWorkDone()`. You do **_not_** need to call it for mapping a buffer. `mapAsync` guarantees work submitted
to the queue before calling `mapAsync` happens before the `mapAsync` returns (see [WebGPU spec: section 5.2](https://www.w3.org/TR/webgpu/#buffer-mapping))

The two use cases for `onSubmittedWorkDone`

1. Waiting for multiple buffer mapping (slow)

   ```js
   // good
   await Promise.all([
     buffer1.mapAsync(),
     buffer2.mapAsync(),
     buffer3.mapAsync(),
   ]);
   data1 = buffer1.getMappedRange();
   data2 = buffer2.getMappedRange();
   data3 = buffer3.getMappedRange();
   ```

   ```js
   // works but slow
   buffer1.mapAsync();
   buffer2.mapAsync();
   buffer3.mapAsync();
   await device.queue.onSubmittedWorkDone();
   data1 = buffer1.getMappedRange();
   data2 = buffer2.getMappedRange();
   data3 = buffer3.getMappedRange();
   ```

   The reason the second method is slow is, the implementation may be able to map the buffers before all the submitted work is done.
   For example, if all the buffers are finished being used, but more work (unrelated to the buffers) is already submitted, then
   you'll end up waiting longer using the second method than the first.

2. Throttling work

   If you are doing heavy compute work and you submit too much work at once, the browser may kill your work.
   You can throttle the work by only submitting more work when the work you've already submitted is done.

## Syntax

```js-nolint
device.queue.onSubmittedWorkDone()
```

### Parameters

None.

### Return value

A {{jsxref("Promise")}} that resolves with {{jsxref("Undefined")}}.

## Examples

```js
device.queue.submit([commandEncoder.finish()]);
device.queue.onSubmittedWorkDone().then(() => {
  console.log("All submitted commands processed.");
});
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpubuffer/destroy/index.md
---
title: "GPUBuffer: destroy() method"
short-title: destroy()
slug: Web/API/GPUBuffer/destroy
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUBuffer.destroy
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`destroy()`** method of the
{{domxref("GPUBuffer")}} interface destroys the `GPUBuffer`.

## Syntax

```js-nolint
destroy()
```

### Parameters

None.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
const output = device.createBuffer({
  size: 1000,
  usage: GPUBufferUsage.STORAGE | GPUBufferUsage.COPY_SRC,
});

// some time later

output.destroy();
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpubuffer/mapasync/index.md
---
title: "GPUBuffer: mapAsync() method"
short-title: mapAsync()
slug: Web/API/GPUBuffer/mapAsync
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUBuffer.mapAsync
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`mapAsync()`** method of the
{{domxref("GPUBuffer")}} interface maps the specified range of the `GPUBuffer`. It returns a {{jsxref("Promise")}} that resolves when the `GPUBuffer`'s content is ready to be accessed. While the `GPUBuffer` is mapped it cannot be used in any GPU commands.

Once the buffer is successfully mapped (which can be checked via {{domxref("GPUBuffer.mapState")}}), calls to {{domxref("GPUBuffer.getMappedRange()")}} will return an {{jsxref("ArrayBuffer")}} containing the `GPUBuffer`'s current values, to be read and updated by JavaScript as required.

When you have finished working with the `GPUBuffer` values, call {{domxref("GPUBuffer.unmap()")}} to unmap it, making it accessible to the GPU again.

## Syntax

```js-nolint
mapAsync(mode)
mapAsync(mode, offset, size)
```

### Parameters

- `mode`

  - : A {{glossary("bitwise flags", "bitwise flag")}} that specifies whether the `GPUBuffer` is mapped for reading or writing. Possible values are:

    - `GPUMapMode.READ`

      - : The `GPUBuffer` is mapped for reading. Values can be read, but any changes made to the {{jsxref("ArrayBuffer")}} returned by {{domxref("GPUBuffer.getMappedRange()")}} will be discarded once {{domxref("GPUBuffer.unmap()")}} is called.

        Read-mode mapping can only be used on `GPUBuffer`s that have a usage of `GPUBufferUsage.MAP_READ` set on them (i.e. when created with {{domxref("GPUDevice.createBuffer()")}}).

    - `GPUMapMode.WRITE`

      - : The `GPUBuffer` is mapped for writing. Values can be read and updated ‚Äî any changes made to the {{jsxref("ArrayBuffer")}} returned by {{domxref("GPUBuffer.getMappedRange()")}} will be saved to the `GPUBuffer` once {{domxref("GPUBuffer.unmap()")}} is called.

        Write-mode mapping can only be used on `GPUBuffer`s that have a usage of `GPUBufferUsage.MAP_WRITE` set on them (i.e. when created with {{domxref("GPUDevice.createBuffer()")}}).

- `offset` {{optional_inline}}
  - : A number representing the offset, in bytes, from the start of the buffer to the start of the range to be mapped. If `offset` is omitted, it defaults to 0.
- `size` {{optional_inline}}
  - : A number representing the size, in bytes, of the range to be mapped. If `size` is omitted, the range mapped extends to the end of the `GPUBuffer`.

### Return value

A {{jsxref("Promise")}} that resolves to {{jsxref("Undefined")}} when the `GPUBuffer`'s content is ready to be accessed.

### Validation

The following criteria must be met when calling **`mapSync()`**, otherwise an `OperationError` {{domxref("DOMException")}} is thrown, the promise is rejected, and a {{domxref("GPUValidationError")}} is generated:

- `offset` is a multiple of 8.
- The total range to be mapped (`size` if specified, or {{domxref("GPUBuffer.size")}} - `offset` if not) is a multiple of 4.
- The total range to be mapped is inside the bounds of the `GPUBuffer`.
- If mode is `GPUMapMode.READ`, the `GPUBuffer` has a usage of `GPUBufferUsage.MAP_READ`.
- If mode is `GPUMapMode.WRITE`, the `GPUBuffer` has a usage of `GPUBufferUsage.MAP_WRITE`.

## Examples

See the [main `GPUBuffer` page](/en-US/docs/Web/API/GPUBuffer#examples) for an example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpubuffer/unmap/index.md
---
title: "GPUBuffer: unmap() method"
short-title: unmap()
slug: Web/API/GPUBuffer/unmap
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUBuffer.unmap
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`unmap()`** method of the
{{domxref("GPUBuffer")}} interface unmaps the mapped range of the `GPUBuffer`, making its contents available for use by the GPU again after it has previously been mapped with {{domxref("GPUBuffer.mapAsync()")}} (the GPU cannot access a mapped `GPUBuffer`).

When `unmap()` is called, any {{jsxref("ArrayBuffer")}}s created via {{domxref("GPUBuffer.getMappedRange()")}} are detached.

## Syntax

```js-nolint
unmap()
```

### Parameters

None.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

See the [main `GPUBuffer` page](/en-US/docs/Web/API/GPUBuffer#examples) for an example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpubuffer/label/index.md
---
title: "GPUBuffer: label property"
short-title: label
slug: Web/API/GPUBuffer/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUBuffer.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** property of the
{{domxref("GPUBuffer")}} interface provides a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUDevice.createBuffer()")}} call, or you can get and set it directly on the `GPUBuffer` object.

## Value

A string. If this has not been previously set as described above, it will be an empty string.

## Examples

Setting and getting a label via `GPUBuffer.label`:

```js
const output = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.STORAGE | GPUBufferUsage.COPY_SRC,
});

output.label = "mybuffer";

console.log(output.label); // "mybuffer"
```

Setting a label via the originating {{domxref("GPUDevice.createBuffer()")}} call, and then getting it via `GPUBuffer.label`:

```js
const output = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.STORAGE | GPUBufferUsage.COPY_SRC,
  label: "mybuffer",
});

console.log(output.label); // "mybuffer"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpubuffer/mapstate/index.md
---
title: "GPUBuffer: mapState property"
short-title: mapState
slug: Web/API/GPUBuffer/mapState
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUBuffer.mapState
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`mapState`** read-only property of the
{{domxref("GPUBuffer")}} interface represents the mapped state of the `GPUBuffer`.

## Value

An enumerated value. Possible values are:

- `unmapped`
  - : The buffer is not mapped. {{domxref("GPUBuffer.getMappedRange()")}} cannot be used to access the contents of the `GPUBuffer` in JavaScript. This could be because:
    - {{domxref("GPUBuffer.mapAsync()")}} has not yet been called.
    - The `GPUBuffer` was previously mapped, and then unmapped again with {{domxref("GPUBuffer.unmap()")}}.
- `pending`
  - : The buffer is not yet mapped. {{domxref("GPUBuffer.mapAsync()")}} has been called, but its {{jsxref("Promise")}} is currently pending. {{domxref("GPUBuffer.getMappedRange()")}} cannot currently be used to access the contents of the `GPUBuffer` in JavaScript.
- `mapped`
  - : The buffer is mapped. The {{domxref("GPUBuffer.mapAsync()")}} {{jsxref("Promise")}} has fulfilled, and {{domxref("GPUBuffer.getMappedRange()")}} can now be used to access the contents of the `GPUBuffer` in JavaScript.

## Examples

```js
const stagingBuffer = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.MAP_READ | GPUBufferUsage.COPY_DST,
});

console.log(stagingBuffer.mapState); // "unmapped"

// ...

await stagingBuffer.mapAsync(
  GPUMapMode.READ,
  0, // Offset
  BUFFER_SIZE, // Length
);

console.log(stagingBuffer.mapState); // "mapped"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpubuffer/usage/index.md
---
title: "GPUBuffer: usage property"
short-title: usage
slug: Web/API/GPUBuffer/usage
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUBuffer.usage
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`usage`** read-only property of the
{{domxref("GPUBuffer")}} interface contains the {{glossary("bitwise flags")}} representing the allowed usages of the `GPUBuffer`.

`usage` is set via the `usage` property in the descriptor object passed into the originating {{domxref("GPUDevice.createBuffer()")}} call.

## Value

The bitwise flags representing the original usages set when the `GPUBuffer` was first created. The returned number is the sum of decimal values representing the different flags, as seen in the table below.

| Bitwise flag                   | Usage description                                                                                                                                                                                                                                                                                                                                    | Hex equiv. | Decimal equiv. |
| ------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | -------------- |
| `GPUBufferUsage.COPY_SRC`      | The buffer can be used as the source of a copy operation, for example the source argument of a {{domxref("GPUCommandEncoder.copyBufferToBuffer","copyBufferToBuffer()")}} call.                                                                                                                                                                      | 0x0004     | 4              |
| `GPUBufferUsage.COPY_DST`      | The buffer can be used as the destination of a copy/write operation, for example the destination argument of a {{domxref("GPUCommandEncoder.copyTextureToBuffer", "copyTextureToBuffer()")}} call.                                                                                                                                                   | 0x0008     | 8              |
| `GPUBufferUsage.INDEX`         | The buffer can be used as an index buffer, for example as the `buffer` argument passed to {{domxref("GPURenderPassEncoder.setIndexBuffer", "setIndexBuffer()")}}.                                                                                                                                                                                    | 0x0010     | 16             |
| `GPUBufferUsage.INDIRECT`      | The buffer can be used to store indirect command arguments, for example as the `indirectBuffer` argument of a {{domxref("GPURenderPassEncoder.drawIndirect", "drawIndirect()")}} or {{domxref("GPUComputePassEncoder.dispatchWorkgroupsIndirect", "dispatchWorkgroupsIndirect()")}} call.                                                            | 0x0100     | 256            |
| `GPUBufferUsage.MAP_READ`      | The buffer can be mapped for reading, for example when calling {{domxref("GPUBuffer.mapAsync", "mapAsync()")}} with a `mode` of `GPUMapMode.READ`. This flag may only be combined with `GPUBufferUsage.COPY_DST`.                                                                                                                                    | 0x0001     | 1              |
| `GPUBufferUsage.MAP_WRITE`     | The buffer can be mapped for writing, for example when calling {{domxref("GPUBuffer.mapAsync", "mapAsync()")}} with a `mode` of `GPUMapMode.WRITE`. This flag may only be combined with `GPUBufferUsage.COPY_SRC`.                                                                                                                                   | 0x0002     | 2              |
| `GPUBufferUsage.QUERY_RESOLVE` | The buffer can be used to capture query results, for example as the destination argument of a {{domxref("GPUCommandEncoder.resolveQuerySet", "resolveQuerySet()")}} call.                                                                                                                                                                            | 0x0200     | 512            |
| `GPUBufferUsage.STORAGE`       | The buffer can be used as a storage buffer, for example as a resource in a bind group entry when creating a {{domxref("GPUBindGroup")}} (via {{domxref("GPUDevice.createBindGroup", "createBindGroup()")}}), which adheres to a {{domxref("GPUBindGroupLayout")}} entry with a buffer binding layout `type` of `"storage"` or `"read-only-storage"`. | 0x0080     | 128            |
| `GPUBufferUsage.UNIFORM`       | The buffer can be used as a uniform buffer, for example as a resource in a bind group entry when creating a {{domxref("GPUBindGroup")}} (via {{domxref("GPUDevice.createBindGroup", "createBindGroup()")}}), which adheres to a {{domxref("GPUBindGroupLayout")}} entry with a buffer binding layout `type` of `"uniform"`.                          | 0x0040     | 64             |
| `GPUBufferUsage.VERTEX`        | The buffer can be used as a vertex buffer, for example as the `buffer` argument passed to {{domxref("GPURenderPassEncoder.setVertexBuffer", "setVertexBuffer()")}}.                                                                                                                                                                                  | 0x0020     | 32             |

## Examples

```js
const output = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.STORAGE | GPUBufferUsage.COPY_SRC,
});

console.log(output.usage); // 132

const stagingBuffer = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.MAP_READ | GPUBufferUsage.COPY_DST,
});

console.log(stagingBuffer.usage); // 9
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpubuffer/getmappedrange/index.md
---
title: "GPUBuffer: getMappedRange() method"
short-title: getMappedRange()
slug: Web/API/GPUBuffer/getMappedRange
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUBuffer.getMappedRange
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`getMappedRange()`** method of the
{{domxref("GPUBuffer")}} interface returns an {{jsxref("ArrayBuffer")}} containing the mapped contents of the `GPUBuffer` in the specified range.

This can only happen once the `GPUBuffer` has been successfully mapped with {{domxref("GPUBuffer.mapAsync()")}} (this can be checked via {{domxref("GPUBuffer.mapState")}}). While the `GPUBuffer` is mapped it cannot be used in any GPU commands.

When you have finished working with the `GPUBuffer` values, call {{domxref("GPUBuffer.unmap()")}} to unmap it, making it accessible to the GPU again.

## Syntax

```js-nolint
getMappedRange()
getMappedRange(offset)
getMappedRange(offset, size)
```

### Parameters

- `offset` {{optional_inline}}
  - : A number representing the offset, in bytes, from the start of the `GPUBuffer`'s mapped range to the start of the range to be returned in the {{jsxref("ArrayBuffer")}}. If `offset` is omitted, it defaults to 0.
- `size` {{optional_inline}}
  - : A number representing the size, in bytes, of the {{jsxref("ArrayBuffer")}} to return. If `size` is omitted, the range extends to the end of the `GPUBuffer`'s mapped range.

### Return value

An {{jsxref("ArrayBuffer")}}.

### Validation

The following criteria must be met when calling **`getMappedRange()`**, otherwise an `OperationError` {{domxref("DOMException")}} is thrown:

- `offset` is a multiple of 8.
- The total range to be mapped (`size` if specified, or mapped range length - `offset` if not) is a multiple of 4.
- The total range is inside the bounds of the mapped range and does not overlap with the {{jsxref("ArrayBuffer")}} ranges specified by any other active `getMappedRange()` calls.

### Exceptions

- `TypeError` {{domxref("DOMException")}}
  - : Thrown if an attempt is made to detach the {{jsxref("ArrayBuffer")}} in any way other than via {{domxref("GPUBuffer.unmap()")}}.

## Examples

See the [main `GPUBuffer` page](/en-US/docs/Web/API/GPUBuffer#examples) for an example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpubuffer/index.md
---
title: GPUBuffer
slug: Web/API/GPUBuffer
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUBuffer
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUBuffer`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents a block of memory that can be used to store raw data to use in GPU operations.

A `GPUBuffer` object instance is created using the {{domxref("GPUDevice.createBuffer()")}} method.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUBuffer.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in
    {{domxref("GPUError")}} messages or console warnings.
- {{domxref("GPUBuffer.mapState", "mapState")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : An enumerated value representing the mapped state of the `GPUBuffer`.
- {{domxref("GPUBuffer.size", "size")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A number representing the length of the `GPUBuffer`'s memory allocation, in bytes.
- {{domxref("GPUBuffer.usage", "usage")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : The {{glossary("bitwise flags")}} representing the allowed usages of the `GPUBuffer`.

## Instance methods

- {{domxref("GPUBuffer.destroy", "destroy()")}} {{Experimental_Inline}}
  - : Destroys the `GPUBuffer`.
- {{domxref("GPUBuffer.getMappedRange", "getMappedRange()")}} {{Experimental_Inline}}
  - : Returns an {{jsxref("ArrayBuffer")}} containing the mapped contents of the `GPUBuffer` in the specified range.
- {{domxref("GPUBuffer.mapAsync", "mapAsync()")}} {{Experimental_Inline}}
  - : Maps the specified range of the `GPUBuffer`. Returns a {{jsxref("Promise")}} that resolves when the `GPUBuffer`'s content is ready to be accessed with {{domxref("GPUBuffer.getMappedRange()")}}.
- {{domxref("GPUBuffer.unmap", "unmap()")}} {{Experimental_Inline}}
  - : Unmaps the mapped range of the `GPUBuffer`, making its contents available for use by the GPU again.

## Examples

In our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/), we create an output buffer to read GPU calculations to, and a staging buffer to be mapped for JavaScript access.

```js
const output = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.STORAGE | GPUBufferUsage.COPY_SRC,
});

const stagingBuffer = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.MAP_READ | GPUBufferUsage.COPY_DST,
});
```

Later on, once the `stagingBuffer` contains the results of the GPU computation, a combination of `GPUBuffer` methods are used to read the data back to JavaScript so that it can then be logged to the console:

- {{domxref("GPUBuffer.mapAsync()")}} is used to map the `GPUBuffer` for reading.
- {{domxref("GPUBuffer.getMappedRange()")}} is used to return an {{jsxref("ArrayBuffer")}} containing the `GPUBuffer`'s contents.
- {{domxref("GPUBuffer.unmap()")}} is used to unmap the `GPUBuffer` again, once we have read the content into JavaScript as needed.

```js
// map staging buffer to read results back to JS
await stagingBuffer.mapAsync(
  GPUMapMode.READ,
  0, // Offset
  BUFFER_SIZE, // Length
);

const copyArrayBuffer = stagingBuffer.getMappedRange(0, BUFFER_SIZE);
const data = copyArrayBuffer.slice(0);
stagingBuffer.unmap();
console.log(new Float32Array(data));
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpubuffer/size/index.md
---
title: "GPUBuffer: size property"
short-title: size
slug: Web/API/GPUBuffer/size
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUBuffer.size
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`size`** read-only property of the
{{domxref("GPUBuffer")}} interface represents the length of the `GPUBuffer`'s memory allocation, in bytes.

`size` is set via the `size` property in the descriptor object passed into the originating {{domxref("GPUDevice.createBuffer()")}} call.

## Value

A number.

## Examples

```js
// Define global buffer size
const BUFFER_SIZE = 1000;

// ...

const output = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.STORAGE | GPUBufferUsage.COPY_SRC,
});

console.log(output.size); // 1000
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucomputepipeline/label/index.md
---
title: "GPUComputePipeline: label property"
short-title: label
slug: Web/API/GPUComputePipeline/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUComputePipeline.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** property of the
{{domxref("GPUComputePipeline")}} interface provides a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUDevice.createComputePipeline()")}} or {{domxref("GPUDevice.createComputePipelineAsync()")}} call, or you can get and set it directly on the `GPUComputePipeline` object.

## Value

A string. If this has not been previously set as described above, it will be an empty string.

## Examples

Setting and getting a label via `GPUComputePipeline.label`:

```js
// ...

const computePipeline = device.createComputePipeline({
  layout: device.createPipelineLayout({
    bindGroupLayouts: [bindGroupLayout],
  }),
  compute: {
    module: shaderModule,
    entryPoint: "main",
  },
});

computePipeline.label = "mycomputepipeline";

console.log(computePipeline.label); // "mycomputepipeline"
```

Setting a label via a {{domxref("GPUDevice.createComputePipeline()")}} call, and then getting it via `GPUComputePipeline.label`:

```js
// ...

const computePipeline = device.createComputePipeline({
  layout: device.createPipelineLayout({
    bindGroupLayouts: [bindGroupLayout],
  }),
  compute: {
    module: shaderModule,
    entryPoint: "main",
  },
  label: "mycomputepipeline",
});

console.log(computePipeline.label); // "mycomputepipeline"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucomputepipeline/index.md
---
title: GPUComputePipeline
slug: Web/API/GPUComputePipeline
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUComputePipeline
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUComputePipeline`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents a pipeline that controls the compute shader stage and can be used in a {{domxref("GPUComputePassEncoder")}}.

A `GPUComputePipeline` object instance can be created using the {{domxref("GPUDevice.createComputePipeline()")}} or {{domxref("GPUDevice.createComputePipelineAsync()")}} methods.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUComputePipeline.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Instance methods

- {{domxref("GPUComputePipeline.getBindGroupLayout", "getBindGroupLayout()")}} {{Experimental_Inline}}
  - : Returns the pipeline's {{domxref("GPUBindGroupLayout")}} object with the given index (i.e. included in the originating {{domxref("GPUDevice.createComputePipeline()")}} or {{domxref("GPUDevice.createComputePipelineAsync()")}} call's pipeline layout).

## Examples

> **Note:** The [WebGPU samples](https://webgpu.github.io/webgpu-samples/) feature many more examples.

### Basic example

Our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/) shows a process of:

- Creating a bind group layout with {{domxref("GPUDevice.createBindGroupLayout()")}}.
- Feeding the `bindGroupLayout` into {{domxref("GPUDevice.createPipelineLayout()")}} to create a {{domxref("GPUPipelineLayout")}}.
- Using that value immediately in a `createComputePipeline()` call to create a {{domxref("GPUComputePipeline")}}.

```js
// ...

const bindGroupLayout = device.createBindGroupLayout({
  entries: [
    {
      binding: 0,
      visibility: GPUShaderStage.COMPUTE,
      buffer: {
        type: "storage",
      },
    },
  ],
});

const computePipeline = device.createComputePipeline({
  layout: device.createPipelineLayout({
    bindGroupLayouts: [bindGroupLayout],
  }),
  compute: {
    module: shaderModule,
    entryPoint: "main",
  },
});

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucomputepipeline/getbindgrouplayout/index.md
---
title: "GPUComputePipeline: getBindGroupLayout() method"
short-title: getBindGroupLayout()
slug: Web/API/GPUComputePipeline/getBindGroupLayout
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUComputePipeline.getBindGroupLayout
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`getBindGroupLayout()`** method of the
{{domxref("GPUComputePipeline")}} interface returns the pipeline's {{domxref("GPUBindGroupLayout")}} object with the given index (i.e. included in the originating {{domxref("GPUDevice.createComputePipeline()")}} or {{domxref("GPUDevice.createComputePipelineAsync()")}} call's pipeline layout).

If the {{domxref("GPUComputePipeline")}} was created with `layout: "auto"`, this method is the only way to retrieve the {{domxref("GPUBindGroupLayout")}}s generated by the pipeline.

## Syntax

```js-nolint
getBindGroupLayout(index)
```

### Parameters

- `index`

  - : A number representing the index of the {{domxref("GPUBindGroupLayout")}} to return.

### Return value

A {{domxref("GPUBindGroupLayout")}} object instance.

### Validation

The following criteria must be met when calling **`getBindGroupLayout()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPUBindGroupLayout")}} object is returned:

- `index` is less than the number of {{domxref("GPUBindGroupLayout")}} objects used in the pipeline layout.

## Examples

> **Note:** You can see complete working examples with `getBindGroupLayout()` in action in the [WebGPU samples](https://webgpu.github.io/webgpu-samples/).

```js
// ...

// Create a compute pipeline using layout: "auto" to automatically generate
// appropriate bind group layouts
const computePipeline = device.createComputePipeline({
  layout: "auto",
  compute: {
    module: shaderModule,
    entryPoint: "main",
  },
});

// Create a bind group with the auto-generated layout from the compute pipeline
const computeBindGroup = device.createBindGroup({
  layout: computePipeline.getBindGroupLayout(0),
  entries: [
    {
      binding: 0,
      resource: { buffer: storageBuffer },
    },
  ],
});

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuoutofmemoryerror/gpuoutofmemoryerror/index.md
---
title: "GPUOutOfMemoryError: GPUOutOfMemoryError() constructor"
short-title: GPUOutOfMemoryError()
slug: Web/API/GPUOutOfMemoryError/GPUOutOfMemoryError
page-type: web-api-constructor
status:
  - experimental
browser-compat: api.GPUOutOfMemoryError.GPUOutOfMemoryError
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUOutOfMemoryError()`** constructor creates a new
{{domxref("GPUOutOfMemoryError")}} object instance.

## Syntax

```js-nolint
new GPUOutOfMemoryError(message)
```

### Parameters

- `message`
  - : A string providing a human-readable message that explains why the error occurred.

## Examples

A developer would not manually use the constructor to create a `GPUOutOfMemoryError` object. The user agent uses this constructor to create an appropriate object when an out-of-memory error is surfaced by {{domxref("GPUDevice.popErrorScope")}} or the {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event.

See the main [`GPUOutOfMemoryError`](/en-US/docs/Web/API/GPUOutOfMemoryError#examples) page for a specific example involving a `GPUOutOfMemoryError` object instance.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling)
-e 

File: /files/en-us/web/api/gpuoutofmemoryerror/index.md
---
title: GPUOutOfMemoryError
slug: Web/API/GPUOutOfMemoryError
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUOutOfMemoryError
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUOutOfMemoryError`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} describes an out-of-memory (oom) error indicating that there was not enough free memory to complete the requested operation.

It represents one of the types of errors surfaced by {{domxref("GPUDevice.popErrorScope")}} and the {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event.

Out-of-memory errors should be relatively rare in a well-behaved app but are less predictable than {{domxref("GPUValidationError")}}s. This is because they are dependent on the device your app is running on as well as other apps that are using GPU resources at the time.

{{InheritanceDiagram}}

## Constructor

- {{domxref("GPUOutOfMemoryError.GPUOutOfMemoryError", "GPUOutOfMemoryError()")}} {{Experimental_Inline}}
  - : Creates a new `GPUOutOfMemoryError` object instance.

## Instance properties

The `message` property is inherited from its parent, {{domxref("GPUError")}}:

- {{domxref("GPUError.message", "message")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A string providing a human-readable message that explains why the error occurred.

## Examples

The following example uses an error scope to capture an out-of-memory error, logging it to the console.

```js
device.pushErrorScope("out-of-memory");

let buffer = device.createBuffer({
  size: 100_000_000_000, // 100GB; far too big
  usage: GPUBufferUsage.COPY_SRC | GPUBufferUsage.MAP_WRITE,
});

device.popErrorScope().then((error) => {
  if (error) {
    // error is a GPUOutOfMemoryError object instance
    buffer = null;
    console.error(`Out of memory, buffer too large. Error: ${error.message}`);
  }
});
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling)
-e 

File: /files/en-us/web/api/gpusampler/label/index.md
---
title: "GPUSampler: label property"
short-title: label
slug: Web/API/GPUSampler/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUSampler.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** property of the
{{domxref("GPUSampler")}} interface provides a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUDevice.createSampler()")}} call, or you can get and set it directly on the `GPUSampler` object.

## Value

A string. If this has not been previously set as described above, it will be an empty string.

## Examples

Setting and getting a label via `GPUSampler.label`:

```js
// ...

const sampler = device.createSampler({
  compare: "less",
});

sampler.label = "mysampler";

console.log(sampler.label); // "mysampler"
```

Setting a label via the originating {{domxref("GPUDevice.createSampler()")}} call, and then getting it via `GPUSampler.label`:

```js
// ...

const sampler = device.createSampler({
  compare: "less",
  label: "mysampler",
});

console.log(sampler.label); // "mysampler"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpusampler/index.md
---
title: GPUSampler
slug: Web/API/GPUSampler
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUSampler
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUSampler`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents an object that can control how shaders transform and filter texture resource data.

A `GPUSampler` object instance is created using the {{domxref("GPUDevice.createSampler()")}} method.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUSampler.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Examples

The following snippet creates a `GPUSampler` that does trilinear filtering and repeats texture coordinates:

```js
// ...
const sampler = device.createSampler({
  addressModeU: "repeat",
  addressModeV: "repeat",
  magFilter: "linear",
  minFilter: "linear",
  mipmapFilter: "linear",
});
```

The WebGPU samples [Shadow Mapping sample](https://webgpu.github.io/webgpu-samples/samples/shadowMapping) uses comparison samplers to sample from a depth texture to render shadows.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevicelostinfo/message/index.md
---
title: "GPUDeviceLostInfo: message property"
short-title: message
slug: Web/API/GPUDeviceLostInfo/message
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUDeviceLostInfo.message
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`message`** read-only property of the
{{domxref("GPUDeviceLostInfo")}} interface provides a human-readable message that explains why the device was lost.

## Value

A string.

## Examples

See the main [`GPUDevice.lost` page](/en-US/docs/Web/API/GPUDevice/lost#examples) for an example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevicelostinfo/index.md
---
title: GPUDeviceLostInfo
slug: Web/API/GPUDeviceLostInfo
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUDeviceLostInfo
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUDeviceLostInfo`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents the object returned when the {{domxref("GPUDevice.lost")}} {{jsxref("Promise")}} resolves. This provides information as to why a device has been lost.

See the {{domxref("GPUDevice.lost")}} page for more information about "lost" state.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUDeviceLostInfo.message", "message")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A string providing a human-readable message that explains why the device was lost.
- {{domxref("GPUDeviceLostInfo.reason", "reason")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : An enumerated value that defines the reason the device was lost in a machine-readable way.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }
  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  // Create a GPUDevice
  let device = await adapter.requestDevice(descriptor);

  // Use lost to handle lost devices
  device.lost.then((info) => {
    console.error(`WebGPU device was lost: ${info.message}`);
    device = null;
    if (info.reason !== "destroyed") {
      init();
    }
  });
  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevicelostinfo/reason/index.md
---
title: "GPUDeviceLostInfo: reason property"
short-title: reason
slug: Web/API/GPUDeviceLostInfo/reason
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUDeviceLostInfo.reason
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`reason`** read-only property of the
{{domxref("GPUDeviceLostInfo")}} interface defines the reason the device was lost in a machine-readable way.

## Value

An enumerated value. At the moment the only value defined in the spec is `"destroyed"`, which indicates that the device was destroyed by a call to {{domxref("GPUDevice.destroy()")}}.

If the device was lost because of an unknown reason not covered in the available enumerated values, `reason` returns `undefined`.

## Examples

See the main [`GPUDevice.lost` page](/en-US/docs/Web/API/GPUDevice/lost#examples) for an example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/drawindexedindirect/index.md
---
title: "GPURenderPassEncoder: drawIndexedIndirect() method"
short-title: drawIndexedIndirect()
slug: Web/API/GPURenderPassEncoder/drawIndexedIndirect
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.drawIndexedIndirect
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`drawIndexedIndirect()`** method of the
{{domxref("GPURenderPassEncoder")}} interface draws indexed primitives using parameters read from a {{domxref("GPUBuffer")}}.

## Syntax

```js-nolint
drawIndexedIndirect(indirectBuffer, indirectOffset)
```

### Parameters

- `indirectBuffer`

  - : A {{domxref("GPUBuffer")}} containing the `indexCount`, `instanceCount`, `firstIndex`, `baseVertex`, and `firstInstance` values needed to carry out the drawing operation. The buffer must contain a tightly packed block of five 32-bit unsigned integer values representing the values (20 bytes total), given in the same order as the arguments for {{domxref("GPURenderPassEncoder.drawIndexed()")}}. So for example:

    ```js
    const uint32 = new Uint32Array(5);
    uint32[0] = 3; // The indexCount value
    uint32[1] = 1; // The instanceCount value
    uint32[2] = 0; // The firstIndex value
    uint32[3] = 0; // The baseVertex value
    uint32[4] = 0; // The firstInstance value

    // Write values into a GPUBuffer
    device.queue.writeBuffer(buffer, 0, uint32, 0, uint32.length);
    ```

- `indirectOffset`
  - : The offset, in bytes, into `indirectBuffer` where the value data begins.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`drawIndirect()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderPassEncoder")}} becomes invalid:

- `indirectBuffer`'s {{domxref("GPUBuffer.usage")}} contains the `GPUBufferUsage.INDIRECT` flag.
- `indirectOffset` + the total size specified by the value parameters in the `indirectBuffer` is less than or equal to the `indirectBuffer`'s {{domxref("GPUBuffer.size")}}.
- `indirectOffset` is a multiple of 4.

## Examples

```js
// ...

// Create GPURenderPassEncoder
const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// Set pipeline and vertex buffer
passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.setIndexBuffer(indexBuffer, "uint16");

// Create drawIndexedIndirect values
const uint32 = new Uint32Array(5);
uint32[0] = 3;
uint32[1] = 1;
uint32[2] = 0;
uint32[3] = 0;
uint32[4] = 0;

// Create a GPUBuffer and write the draw values into it
const drawValues = device.createBuffer({
  size: 20,
  usage: GPUBufferUsage.COPY_DST | GPUBufferUsage.INDIRECT,
});
device.queue.writeBuffer(drawValues, 0, uint32, 0, uint32.length);

// Draw the vertices
passEncoder.drawIndexedIndirect(drawValues, 0);

// End the render pass
passEncoder.end();

// End frame by passing array of GPUCommandBuffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/setviewport/index.md
---
title: "GPURenderPassEncoder: setViewport() method"
short-title: setViewport()
slug: Web/API/GPURenderPassEncoder/setViewport
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.setViewport
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setViewport()`** method of the
{{domxref("GPURenderPassEncoder")}} interface sets the viewport used during the rasterization stage to linearly map from normalized device coordinates to viewport coordinates.

## Syntax

```js-nolint
setViewport(x, y, width, height, minDepth, maxDepth)
```

### Parameters

- `x`
  - : A number representing the minimum X value of the viewport, in pixels.
- `y`
  - : A number representing the minimum Y value of the viewport, in pixels.
- `width`
  - : A number representing the width of the viewport, in pixels.
- `height`
  - : A number representing the height of the viewport, in pixels.
- `minDepth`
  - : A number representing the minimum depth value of the viewport.
- `maxDepth`
  - : A number representing the maximum depth value of the viewport.

> **Note:** If a `setViewport()` call is not made, the default values are `(0, 0, attachment width, attachment height, 0, 1)` for each render pass.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`setViewport()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderPassEncoder")}} becomes invalid:

- `x`, `y`, `width`, and `height` are all greater than or equal to 0.
- `x` + `width` is less than or equal to the width of the render pass's render attachments (see note below).
- `y` + `height` is less than or equal to the height of the render pass's render attachments (see note below).
- `minDepth` and `maxDepth` are both inside the range 0.0‚Äì1.0 inclusive.
- `minDepth` is less than `maxDepth`.

> **Note:** See the color and depth/stencil attachments specified in the descriptor of {{domxref("GPUCommandEncoder.beginRenderPass()")}}; the width and height are based on that of the {{domxref("GPUTexture")}} that their `view`s originate from.

## Examples

### Basic snippet

In a typical canvas render, the following could be used to halve the width and height of the rendered graphics:

```js
passEncoder.setViewport(0, 0, canvas.width / 2, canvas.height / 2, 0, 1);
```

### In context

In the WebGPU Samples [reversedZ example](https://webgpu.github.io/webgpu-samples/samples/reversedZ), `setViewport` is used several times to set the viewport for the different render passes. Study the example code listing for the full context.

For example:

```js
// ...

colorPass.setViewport(
  (canvas.width * m) / 2,
  0,
  canvas.width / 2,
  canvas.height,
  0,
  1,
);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/drawindirect/index.md
---
title: "GPURenderPassEncoder: drawIndirect() method"
short-title: drawIndirect()
slug: Web/API/GPURenderPassEncoder/drawIndirect
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.drawIndirect
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`drawIndirect()`** method of the
{{domxref("GPURenderPassEncoder")}} interface draws primitives using parameters read from a {{domxref("GPUBuffer")}}.

## Syntax

```js-nolint
drawIndirect(indirectBuffer, indirectOffset)
```

### Parameters

- `indirectBuffer`

  - : A {{domxref("GPUBuffer")}} containing the `vertexCount`, `instanceCount`, `firstVertex`, and `firstInstance` values needed to carry out the drawing operation. The buffer must contain a tightly packed block of four 32-bit unsigned integer values representing the values (16 bytes total), given in the same order as the arguments for {{domxref("GPURenderPassEncoder.draw()")}}. So for example:

    ```js
    const uint32 = new Uint32Array(4);
    uint32[0] = 3; // The vertexCount value
    uint32[1] = 1; // The instanceCount value
    uint32[2] = 0; // The firstVertex value
    uint32[3] = 0; // The firstInstance value

    // Write values into a GPUBuffer
    device.queue.writeBuffer(buffer, 0, uint32, 0, uint32.length);
    ```

- `indirectOffset`
  - : The offset, in bytes, into `indirectBuffer` where the value data begins.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`drawIndirect()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderPassEncoder")}} becomes invalid:

- `indirectBuffer`'s {{domxref("GPUBuffer.usage")}} contains the `GPUBufferUsage.INDIRECT` flag.
- `indirectOffset` + the total size specified by the value parameters in the `indirectBuffer` is less than or equal to the `indirectBuffer`'s {{domxref("GPUBuffer.size")}}.
- `indirectOffset` is a multiple of 4.

## Examples

```js
// ...

// Create GPURenderPassEncoder
const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// Set pipeline and vertex buffer
passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);

// Create drawIndirect values
const uint32 = new Uint32Array(4);
uint32[0] = 3;
uint32[1] = 1;
uint32[2] = 0;
uint32[3] = 0;

// Create a GPUBuffer and write the draw values into it
const drawValues = device.createBuffer({
  size: 16,
  usage: GPUBufferUsage.COPY_DST | GPUBufferUsage.INDIRECT,
});
device.queue.writeBuffer(drawValues, 0, uint32, 0, uint32.length);

// Draw the vertices
passEncoder.drawIndirect(drawValues, 0);

// End the render pass
passEncoder.end();

// End frame by passing array of GPUCommandBuffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/setpipeline/index.md
---
title: "GPURenderPassEncoder: setPipeline() method"
short-title: setPipeline()
slug: Web/API/GPURenderPassEncoder/setPipeline
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.setPipeline
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setPipeline()`** method of the
{{domxref("GPURenderPassEncoder")}} interface sets the {{domxref("GPURenderPipeline")}} to use for subsequent render pass commands.

## Syntax

```js-nolint
setPipeline(pipeline)
```

### Parameters

- `pipeline`
  - : The {{domxref("GPURenderPipeline")}} to use for subsequent render pass commands.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`setPipeline()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderPassEncoder")}} becomes invalid:

- If the {{domxref("GPURenderPipeline")}} writes to the depth component of the depth/stencil attachment, `depthReadOnly` (as specified in the descriptor of the originating {{domxref("GPUCommandEncoder.beginRenderPass()")}} call) is `true`.
- If the {{domxref("GPURenderPipeline")}} writes to the stencil component of the depth/stencil attachment, `stencilReadOnly` (as specified in the descriptor of the originating {{domxref("GPUCommandEncoder.beginRenderPass()")}} call) is `true`.

## Examples

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/), several commands are recorded via a {{domxref("GPUCommandEncoder")}}. Most of these commands originate from the `GPURenderPassEncoder` created via {{domxref("GPUCommandEncoder.beginRenderPass()")}}. `setPipeline()` is called in an appropriate place to set the render pipeline.

```js
// ...

const renderPipeline = device.createRenderPipeline(pipelineDescriptor);

// Create GPUCommandEncoder to issue commands to the GPU
// Note: render pass descriptor, command encoder, etc. are destroyed after use, fresh one needed for each frame.
const commandEncoder = device.createCommandEncoder();

// Create GPURenderPassDescriptor to tell WebGPU which texture to draw into, then initiate render pass
const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
};

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// Draw the triangle
passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

// End the render pass
passEncoder.end();

// End frame by passing array of command buffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/setbindgroup/index.md
---
title: "GPURenderPassEncoder: setBindGroup() method"
short-title: setBindGroup()
slug: Web/API/GPURenderPassEncoder/setBindGroup
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.setBindGroup
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setBindGroup()`** method of the
{{domxref("GPURenderPassEncoder")}} interface sets the {{domxref("GPUBindGroup")}} to use for subsequent render commands, for a given index.

## Syntax

```js-nolint
setBindGroup(index, bindGroup)
setBindGroup(index, bindGroup, dynamicOffsets)
setBindGroup(index, bindGroup, dynamicOffsets, dynamicOffsetsStart,
             dynamicOffsetsLength)
```

#### Parameters

- `index`
  - : The index to set the bind group at. This matches the `n` index value of the corresponding [`@group(n)`](https://gpuweb.github.io/gpuweb/wgsl/#attribute-group) attribute in the shader code ({{domxref("GPUShaderModule")}}) used in the related pipeline.
- `bindGroup`
  - : The {{domxref("GPUBindGroup")}} to use for subsequent render commands.
- `dynamicOffsets` {{optional_inline}}
  - : A value specifying the offset, in bytes, for each entry in `bindGroup` with `hasDynamicOffset: true` set (i.e. in the descriptor of the {{domxref("GPUDevice.createBindGroupLayout()")}} call that created the {{domxref("GPUBindGroupLayout")}} object that the `bindGroup` is based on). This value can be:
    - An array of numbers specifying the different offsets.
    - A {{jsxref("Uint32Array")}} containing numbers specifying the offsets.

If a {{jsxref("Uint32Array")}} value is specified for `dynamicOffsets`, both of the following parameters are also required:

- `dynamicOffsetsStart`
  - : A number specifying the offset, in array elements, into `dynamicOffsetsData`, where the dynamic offset data begins.
- `dynamicOffsetsLength`
  - : A number specifying the number of dynamic offset values to be read from in `dynamicOffsetsData`.

### Return value

None ({{jsxref("Undefined")}}).

### Exceptions

For `setBindGroup()` calls that use a {{jsxref("Uint32Array")}} value for `dynamicOffsets`, the call will throw with a `RangeError` {{domxref("DOMException")}} if:

- `dynamicOffsetsStart` is less than 0.
- `dynamicOffsetsStart` + `dynamicOffsetsLength` is greater than `dynamicOffsets.length`.

### Validation

The following criteria must be met when calling **`setBindGroup()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderPassEncoder")}} becomes invalid:

- `index` is less than or equal to the {{domxref("GPUDevice")}}'s `maxBindGroups` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- `dynamicOffsets.length` is the same as the number of entries in `bindGroup` with `hasDynamicOffset: true` set.
- For `bindGroup` entries where the bound `buffer`'s `type` is `"uniform"` (see {{domxref("GPUDevice.createBindGroupLayout()")}}), each number in `dynamicOffsets` is a multiple of the {{domxref("GPUDevice")}}'s `minUniformBufferOffsetAlignment` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- For `bindGroup` entries where the bound `buffer`'s `type` is `"storage"` or `"read-only-storage"` (see {{domxref("GPUDevice.createBindGroupLayout()")}}), each number in `dynamicOffsets` is a multiple of the {{domxref("GPUDevice")}}'s `minStorageBufferOffsetAlignment` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- For each `bindGroup` entry, the bound `buffer`'s `offset`, plus the corresponding layout entry's `minBindingSize`, plus the corresponding dynamic offset specified in `dynamicOffsets`, is less than or equal to the bound `buffer`'s `size`.

## Examples

In the WebGPU Samples [Textured Cube example](https://webgpu.github.io/webgpu-samples/samples/texturedCube), `setBindGroup()` is used to bind the `uniformBindGroup` to index position 0. Check out the example for the full context.

```js
// ...

const commandEncoder = device.createCommandEncoder();
const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);
passEncoder.setPipeline(pipeline);
passEncoder.setBindGroup(0, uniformBindGroup);
passEncoder.setVertexBuffer(0, verticesBuffer);
passEncoder.draw(cubeVertexCount, 1, 0, 0);
passEncoder.end();
device.queue.submit([commandEncoder.finish()]);

// ...
```

> **Note:** Study the other [WebGPU Samples](https://webgpu.github.io/webgpu-samples) for more examples of `setBindGroup()` usage.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/setvertexbuffer/index.md
---
title: "GPURenderPassEncoder: setVertexBuffer() method"
short-title: setVertexBuffer()
slug: Web/API/GPURenderPassEncoder/setVertexBuffer
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.setVertexBuffer
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setVertexBuffer()`** method of the
{{domxref("GPURenderPassEncoder")}} interface sets or unsets the current {{domxref("GPUBuffer")}} for the given slot that will provide vertex data for subsequent drawing commands.

## Syntax

```js-nolint
setVertexBuffer(slot, buffer, offset, size)
```

### Parameters

- `slot`
  - : A number referencing the vertex buffer slot to set the vertex buffer for.
- `buffer`
  - : A {{domxref("GPUBuffer")}} representing the buffer containing the vertex data to use for subsequent drawing commands, or `null`, in which case any previously-set buffer in the given slot is unset.
- `offset` {{optional_inline}}
  - : A number representing the offset, in bytes, into `buffer` where the vertex data begins. If omitted, `offset` defaults to 0.
- `size` {{optional_inline}}
  - : A number representing the size, in bytes, of the vertex data contained in `buffer`. If omitted, `size` defaults to the `buffer`'s {{domxref("GPUBuffer.size")}} - `offset`.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`setVertexBuffer()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderPassEncoder")}} becomes invalid:

- `buffer`'s {{domxref("GPUBuffer.usage")}} contains the `GPUBufferUsage.VERTEX` flag.
- `slot` is less than the {{domxref("GPUDevice")}}'s `maxVertexBuffers` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- `offset` + `size` is less than or equal to the `buffer`'s {{domxref("GPUBuffer.size")}}.
- `offset` is a multiple of 4.

## Examples

### Set vertex buffer

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/), several commands are recorded via a {{domxref("GPUCommandEncoder")}}. Most of these commands originate from the `GPURenderPassEncoder` created via {{domxref("GPUCommandEncoder.beginRenderPass()")}}. `setVertexBuffer()` is used as appropriate to set the source of vertex data.

```js
// ...

const renderPipeline = device.createRenderPipeline(pipelineDescriptor);

// Create GPUCommandEncoder to issue commands to the GPU
// Note: render pass descriptor, command encoder, etc. are destroyed after use, fresh one needed for each frame.
const commandEncoder = device.createCommandEncoder();

// Create GPURenderPassDescriptor to tell WebGPU which texture to draw into, then initiate render pass
const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
};

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// Draw the triangle
passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

// End the render pass
passEncoder.end();

// End frame by passing array of command buffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

### Unset vertex buffer

```js
// Set vertex buffer in slot 0
passEncoder.setVertexBuffer(0, vertexBuffer);

// Later, unset vertex buffer in slot 0
passEncoder.setVertexBuffer(0, null);
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/beginocclusionquery/index.md
---
title: "GPURenderPassEncoder: beginOcclusionQuery() method"
short-title: beginOcclusionQuery()
slug: Web/API/GPURenderPassEncoder/beginOcclusionQuery
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.beginOcclusionQuery
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`beginOcclusionQuery()`** method of the
{{domxref("GPURenderPassEncoder")}} interface begins an occlusion query at the specified index of the relevant {{domxref("GPUQuerySet")}} (provided as the value of the `occlusionQuerySet` descriptor property when invoking {{domxref("GPUCommandEncoder.beginRenderPass()")}} to run the render pass).

## Syntax

```js-nolint
beginOcclusionQuery(queryIndex)
```

### Parameters

- `queryIndex`
  - : The index in the {{domxref("GPUQuerySet")}} to begin the occlusion query at.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`beginOcclusionQuery()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderPassEncoder")}} becomes invalid:

- A {{domxref("GPUQuerySet")}} was specified in the `occlusionQuerySet` descriptor property when invoking the originating {{domxref("GPUCommandEncoder.beginRenderPass()")}}.
- `queryIndex` is smaller than {{domxref("GPUQuerySet.count")}}.
- The `queryIndex` has not already been written to in the same render pass.
- An occlusion query is not already active for this render pass (i.e. via a previous `beginOcclusionQuery()` call).

## Examples

```js
// ...

// Create a query set to hold the occlusion queries
const querySet = device.createQuerySet({
  type: "occlusion",
  count: 32,
});

// Render pass descriptor object, including the querySet
const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
  occlusionQuerySet: querySet,
};

// Begin the render pass
const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// Begin an occlusion query at index 0
passEncoder.beginOcclusionQuery(0);

// Run some rendering commands
passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

// End the occlusion query
passEncoder.endOcclusionQuery();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/setindexbuffer/index.md
---
title: "GPURenderPassEncoder: setIndexBuffer() method"
short-title: setIndexBuffer()
slug: Web/API/GPURenderPassEncoder/setIndexBuffer
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.setIndexBuffer
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setIndexBuffer()`** method of the
{{domxref("GPURenderPassEncoder")}} interface sets the current {{domxref("GPUBuffer")}} that will provide index data for subsequent drawing commands.

## Syntax

```js-nolint
setIndexBuffer(buffer, indexFormat, offset, size)
```

### Parameters

- `buffer`
  - : A {{domxref("GPUBuffer")}} representing the buffer containing the index data to use for subsequent drawing commands.
- `indexFormat`
  - : An enumerated value that defines the format of the index data contained in `buffer`. Possible values are:
    - `"uint16"`
    - `"uint32"`
- `offset` {{optional_inline}}
  - : A number representing the offset, in bytes, into `buffer` where the index data begins. If omitted, `offset` defaults to 0.
- `size` {{optional_inline}}
  - : A number representing the size, in bytes, of the index data contained in `buffer`. If omitted, `size` defaults to the `buffer`'s {{domxref("GPUBuffer.size")}} - `offset`.

#### Note on indexFormat

`indexFormat` determines both the data type of index values in a buffer and, when used with a pipeline that specifies a strip primitive topology (`"line-strip"` or `"triangle-strip"`), also determines the primitive restart value. The primitive restart value is an index value indicating that a new primitive should be started rather than continuing to construct the strip with the prior indexed vertices. The value is `0xFFFF` for `"uint16"`, or `0xFFFFFFFF` for `"uint32"`.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`setIndexBuffer()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderPassEncoder")}} becomes invalid:

- `buffer`'s {{domxref("GPUBuffer.usage")}} contains the `GPUBufferUsage.INDEX` flag.
- `offset` + `size` is less than or equal to the `buffer`'s {{domxref("GPUBuffer.size")}}.
- `offset` is a multiple of `indexFormat`'s byte size (2 for `"uint16"`, 4 for `"uint32"`).

## Examples

In the WebGPU Samples [Shadow Mapping](https://webgpu.github.io/webgpu-samples/samples/shadowMapping) example, `setIndexBuffer()` is used in two separate render passes in each animation frame, one to draw the main model and one to draw its shadow. Study the example code listing for the full context.

```js
// ...

const commandEncoder = device.createCommandEncoder();
{
  const shadowPass = commandEncoder.beginRenderPass(shadowPassDescriptor);
  shadowPass.setPipeline(shadowPipeline);
  shadowPass.setBindGroup(0, sceneBindGroupForShadow);
  shadowPass.setBindGroup(1, modelBindGroup);
  shadowPass.setVertexBuffer(0, vertexBuffer);
  shadowPass.setIndexBuffer(indexBuffer, "uint16");
  shadowPass.drawIndexed(indexCount);

  shadowPass.end();
}
{
  const renderPass = commandEncoder.beginRenderPass(renderPassDescriptor);
  renderPass.setPipeline(pipeline);
  renderPass.setBindGroup(0, sceneBindGroupForRender);
  renderPass.setBindGroup(1, modelBindGroup);
  renderPass.setVertexBuffer(0, vertexBuffer);
  renderPass.setIndexBuffer(indexBuffer, "uint16");
  renderPass.drawIndexed(indexCount);

  renderPass.end();
}

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/setstencilreference/index.md
---
title: "GPURenderPassEncoder: setStencilReference() method"
short-title: setStencilReference()
slug: Web/API/GPURenderPassEncoder/setStencilReference
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.setStencilReference
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setStencilReference()`** method of the
{{domxref("GPURenderPassEncoder")}} interface sets the stencil reference value using during stencil tests with the `"replace"` stencil operation (as set in the descriptor of the {{domxref("GPUDevice.createRenderPipeline()")}} method, in the properties defining the various stencil operations).

## Syntax

```js-nolint
setStencilReference(reference)
```

### Parameters

- `reference`
  - : A number representing the new stencil reference value to set for the render pass.

> **Note:** If a `setStencilReference()` call is not made, the stencil reference value defaults to 0 for each render pass.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
// ...

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.setStencilReference(1);
passEncoder.draw(3);

passEncoder.end();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/label/index.md
---
title: "GPURenderPassEncoder: label property"
short-title: label
slug: Web/API/GPURenderPassEncoder/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** read-only property of the
{{domxref("GPURenderPassEncoder")}} interface is a string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUCommandEncoder.beginRenderPass()")}} call, or you can get and set it directly on the `GPURenderPassEncoder` object.

## Value

A string. If no label value has previously been set, getting the label returns an empty string.

## Examples

Setting and getting a label via `GPURenderPassEncoder.label`:

```js
const commandEncoder = device.createCommandEncoder();

const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
};

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);
passEncoder.label = "myrenderpassencoder";

console.log(passEncoder.label); // "myrenderpassencoder"
```

Setting a label via the originating {{domxref("GPUCommandEncoder.beginRenderPass()")}} call, and then getting it via `GPURenderPassEncoder.label`:

```js
const commandEncoder = device.createCommandEncoder();

const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
  label: "myrenderpassencoder",
};

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

console.log(passEncoder.label); // "myrenderpassencoder"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/endocclusionquery/index.md
---
title: "GPURenderPassEncoder: endOcclusionQuery() method"
short-title: endOcclusionQuery()
slug: Web/API/GPURenderPassEncoder/endOcclusionQuery
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.endOcclusionQuery
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`endOcclusionQuery()`** method of the
{{domxref("GPURenderPassEncoder")}} interface ends an active occlusion query previously started with {{domxref("GPURenderPassEncoder.beginOcclusionQuery", "beginOcclusionQuery()")}}.

## Syntax

```js-nolint
endOcclusionQuery()
```

### Parameters

None.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`endOcclusionQuery()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderPassEncoder")}} becomes invalid:

- An occlusion query is active for this render pass (i.e. via a previous `beginOcclusionQuery()` call).

## Examples

```js
// ...

// Create a query set to hold the occlusion queries
const querySet = device.createQuerySet({
  type: "occlusion",
  count: 32,
});

// Render pass descriptor object, including the querySet
const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
  occlusionQuerySet: querySet,
};

// Begin the render pass
const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// Begin an occlusion query at index 0
passEncoder.beginOcclusionQuery(0);

// Run some rendering commands
passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

// End the occlusion query
passEncoder.endOcclusionQuery();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/end/index.md
---
title: "GPURenderPassEncoder: end() method"
short-title: end()
slug: Web/API/GPURenderPassEncoder/end
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.end
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`end()`** method of the
{{domxref("GPURenderPassEncoder")}} interface completes recording of the current render pass command sequence.

## Syntax

```js-nolint
end()
```

### Parameters

None.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`end()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderPassEncoder")}} becomes invalid:

- The {{domxref("GPURenderPassEncoder")}} is open (i.e. not already ended via an `end()` call).
- There is no occlusion query (i.e. started via {{domxref("GPURenderPassEncoder.beginOcclusionQuery", "beginOcclusionQuery()")}}) active on the current render pass.
- The debug stack for the current render pass is empty (i.e. no render pass debug group is currently open, as opened by {{domxref("GPURenderPassEncoder.pushDebugGroup", "pushDebugGroup()")}}).
- The number of draw commands encoded in this render pass is less than or equal to the `maxDrawCount` property set in the {{domxref("GPUCommandEncoder.beginRenderPass()")}} descriptor.

## Examples

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/), several commands are recorded via a {{domxref("GPUCommandEncoder")}}. Most of these commands originate from the `GPURenderPassEncoder` created via {{domxref("GPUCommandEncoder.beginRenderPass()")}}. `end()` is called in an appropriate place to end the render pass.

```js
// ...

const renderPipeline = device.createRenderPipeline(pipelineDescriptor);

// Create GPUCommandEncoder to issue commands to the GPU
// Note: render pass descriptor, command encoder, etc. are destroyed after use, fresh one needed for each frame.
const commandEncoder = device.createCommandEncoder();

// Create GPURenderPassDescriptor to tell WebGPU which texture to draw into, then initiate render pass
const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
};

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// Draw the triangle
passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

// End the render pass
passEncoder.end();

// End frame by passing array of command buffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/insertdebugmarker/index.md
---
title: "GPURenderPassEncoder: insertDebugMarker() method"
short-title: insertDebugMarker()
slug: Web/API/GPURenderPassEncoder/insertDebugMarker
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.insertDebugMarker
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`insertDebugMarker()`** method of the
{{domxref("GPURenderPassEncoder")}} interface marks a specific point in a series of encoded render pass commands with a label.

This could be used for telemetry, or may be utilized in {{domxref("GPUError")}} messages, browser dev tools, or other services in the future to help with debugging.

## Syntax

```js-nolint
insertDebugMarker(markerLabel)
```

### Parameters

- `markerLabel`
  - : A string representing the label to insert.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
// ...

passEncoder.insertDebugMarker("mymarker");

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/setblendconstant/index.md
---
title: "GPURenderPassEncoder: setBlendConstant() method"
short-title: setBlendConstant()
slug: Web/API/GPURenderPassEncoder/setBlendConstant
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.setBlendConstant
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setBlendConstant()`** method of the
{{domxref("GPURenderPassEncoder")}} interface sets the constant blend color and alpha values used with `"constant"` and `"one-minus-constant"` blend factors (as set in the descriptor of the {{domxref("GPUDevice.createRenderPipeline()")}} method, in the `blend` property).

## Syntax

```js-nolint
setBlendConstant(color)
```

### Parameters

- `color`

  - : An object or array representing the color to use when blending ‚Äî the `r`, `g`, `b`, and `a` components are represented as floating point numbers between 0.0 and 1.0.

    What follows is an object example:

    ```js
    const color = { r: 0.0, g: 0.5, b: 1.0, a: 1.0 };
    ```

    The array equivalent would look like this:

    ```js
    const color = [0.0, 0.5, 1.0, 1.0];
    ```

> **Note:** If a `setBlendConstant()` call is not made, the blend constant color value defaults to `(0, 0, 0, 0)` for each render pass.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
// ...

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.setBlendConstant([1.0, 0.0, 0.0, 1.0]);
passEncoder.draw(3);

passEncoder.end();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/setscissorrect/index.md
---
title: "GPURenderPassEncoder: setScissorRect() method"
short-title: setScissorRect()
slug: Web/API/GPURenderPassEncoder/setScissorRect
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.setScissorRect
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setScissorRect()`** method of the
{{domxref("GPURenderPassEncoder")}} interface sets the scissor rectangle used during the rasterization stage. After transformation into viewport coordinates any fragments that fall outside the scissor rectangle will be discarded.

## Syntax

```js-nolint
setScissorRect(x, y, width, height)
```

### Parameters

- `x`
  - : A number representing the minimum X value of the scissor rectangle, in pixels.
- `y`
  - : A number representing the minimum Y value of the scissor rectangle, in pixels.
- `width`
  - : A number representing the width of the scissor rectangle, in pixels.
- `height`
  - : A number representing the height of the scissor rectangle, in pixels.

> **Note:** If a `setScissorRect()` call is not made, the default values are `(0, 0, attachment width, attachment height)` for each render pass.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`setViewport()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderPassEncoder")}} becomes invalid:

- `x` + `width` is less than or equal to the width of the render pass's render attachments (see note below).
- `y` + `height` is less than or equal to the height of the render pass's render attachments (see note below).

> **Note:** See the color and depth/stencil attachments specified in the descriptor of {{domxref("GPUCommandEncoder.beginRenderPass()")}}; the width and height are based on that of the {{domxref("GPUTexture")}} that their `view`s originate from.

## Examples

### Basic snippet

In a typical canvas render, the following could be used to discard any rendering outside of the top-left quarter of the canvas:

```js
passEncoder.setScissorRect(0, 0, canvas.width / 2, canvas.height / 2);
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/index.md
---
title: GPURenderPassEncoder
slug: Web/API/GPURenderPassEncoder
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPURenderPassEncoder
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPURenderPassEncoder`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} encodes commands related to controlling the vertex and fragment shader stages, as issued by a {{domxref("GPURenderPipeline")}}. It forms part of the overall encoding activity of a {{domxref("GPUCommandEncoder")}}.

A render pipeline renders graphics to {{domxref("GPUTexture")}} attachments, typically intended for display in a {{htmlelement("canvas")}} element, but it could also render to textures used for other purposes that never appear onscreen. It has two main stages:

- A vertex stage, in which a vertex shader takes positioning data fed into the GPU and uses it to position a series of vertices in 3D space by applying specified effects like rotation, translation, or perspective. The vertices are then assembled into primitives such as triangles (the basic building block of rendered graphics) and rasterized by the GPU to figure out what pixels each one should cover on the drawing canvas.

- A fragment stage, in which a fragment shader computes the color for each pixel covered by the primitives produced by the vertex shader. These computations frequently use inputs such as images (in the form of textures) that provide surface details and the position and color of virtual lights.

A `GPURenderPassEncoder` object instance is created via the {{domxref("GPUCommandEncoder.beginRenderPass()")}} property.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPURenderPassEncoder.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Instance methods

- {{domxref("GPURenderPassEncoder.beginOcclusionQuery", "beginOcclusionQuery()")}} {{Experimental_Inline}}
  - : Begins an occlusion query at the specified index of the relevant {{domxref("GPUQuerySet")}} (provided as the value of the `occlusionQuerySet` descriptor property when invoking {{domxref("GPUCommandEncoder.beginRenderPass()")}} to run the render pass).
- {{domxref("GPURenderPassEncoder.draw", "draw()")}} {{Experimental_Inline}}
  - : Draw primitives based on the vertex buffers provided by {{domxref("GPURenderPassEncoder.setVertexBuffer", "setVertexBuffer()")}}.
- {{domxref("GPURenderPassEncoder.drawIndexed", "drawIndexed()")}} {{Experimental_Inline}}
  - : Draw indexed primitives based on the vertex and index buffers provided by {{domxref("GPURenderPassEncoder.setVertexBuffer", "setVertexBuffer()")}} and {{domxref("GPURenderPassEncoder.setIndexBuffer", "setIndexBuffer()")}}
- {{domxref("GPURenderPassEncoder.drawIndirect", "drawIndirect()")}} {{Experimental_Inline}}
  - : Draw primitives using parameters read from a {{domxref("GPUBuffer")}}.
- {{domxref("GPURenderPassEncoder.drawIndexedIndirect", "drawIndexedIndirect()")}} {{Experimental_Inline}}

  - : Draw indexed primitives using parameters read from a {{domxref("GPUBuffer")}}.

- {{domxref("GPURenderPassEncoder.end", "end()")}} {{Experimental_Inline}}
  - : Completes recording of the current render pass command sequence.
- {{domxref("GPURenderPassEncoder.endOcclusionQuery", "endOcclusionQuery()")}} {{Experimental_Inline}}
  - : Ends an active occlusion query previously started with {{domxref("GPURenderPassEncoder.beginOcclusionQuery", "beginOcclusionQuery()")}}.
- {{domxref("GPURenderPassEncoder.executeBundles", "executeBundles()")}} {{Experimental_Inline}}
  - : Executes commands previously recorded into the referenced {{domxref("GPURenderBundle")}}s, as part of this render pass.
- {{domxref("GPURenderPassEncoder.insertDebugMarker", "insertDebugMarker()")}} {{Experimental_Inline}}
  - : Marks a specific point in a series of encoded commands with a label.
- {{domxref("GPURenderPassEncoder.popDebugGroup", "popDebugGroup()")}} {{Experimental_Inline}}
  - : Ends a debug group, which is begun with a {{domxref("GPURenderPassEncoder.pushDebugGroup", "pushDebugGroup()")}} call.
- {{domxref("GPURenderPassEncoder.pushDebugGroup", "pushDebugGroup()")}} {{Experimental_Inline}}
  - : Begins a debug group, which is marked with a specified label, and will contain all subsequent encoded commands up until a {{domxref("GPURenderPassEncoder.popDebugGroup", "popDebugGroup()")}} method is invoked.
- {{domxref("GPURenderPassEncoder.setBindGroup", "setBindGroup()")}} {{Experimental_Inline}}
  - : Sets the {{domxref("GPUBindGroup")}} to use for subsequent render commands, for a given index.
- {{domxref("GPURenderPassEncoder.setBlendConstant", "setBlendConstant()")}} {{Experimental_Inline}}

  - : Sets the constant blend color and alpha values used with `"constant"` and `"one-minus-constant"` blend factors (as set in the descriptor of the {{domxref("GPUDevice.createRenderPipeline()")}} method, in the `blend` property).

- {{domxref("GPURenderPassEncoder.setIndexBuffer", "setIndexBuffer()")}} {{Experimental_Inline}}

  - : Sets the current {{domxref("GPUBuffer")}} that will provide index data for subsequent drawing commands.

- {{domxref("GPURenderPassEncoder.setPipeline", "setPipeline()")}} {{Experimental_Inline}}
  - : Sets the {{domxref("GPURenderPipeline")}} to use for this render pass.
- {{domxref("GPURenderPassEncoder.setScissorRect", "setScissorRect()")}} {{Experimental_Inline}}
  - : Sets the scissor rectangle used during the rasterization stage. After transformation into viewport coordinates any fragments that fall outside the scissor rectangle will be discarded.
- {{domxref("GPURenderPassEncoder.setStencilReference", "setStencilReference()")}} {{Experimental_Inline}}

  - : Sets the stencil reference value using during stencil tests with the `"replace"` stencil operation (as set in the descriptor of the {{domxref("GPUDevice.createRenderPipeline()")}} method, in the properties defining the various stencil operations).

- {{domxref("GPURenderPassEncoder.setVertexBuffer", "setVertexBuffer()")}} {{Experimental_Inline}}
  - : Sets or unsets the current {{domxref("GPUBuffer")}} that will provide vertex data for subsequent drawing commands.
- {{domxref("GPURenderPassEncoder.setViewport", "setViewport()")}} {{Experimental_Inline}}
  - : Sets the viewport used during the rasterization stage to linearly map from normalized device coordinates to viewport coordinates.

## Examples

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/), several commands are recorded via a {{domxref("GPUCommandEncoder")}}. Most of these commands originate from the `GPURenderPassEncoder` created via {{domxref("GPUCommandEncoder.beginRenderPass()")}}.

```js
// ...

const renderPipeline = device.createRenderPipeline(pipelineDescriptor);

// Create GPUCommandEncoder to issue commands to the GPU
// Note: render pass descriptor, command encoder, etc. are destroyed after use, fresh one needed for each frame.
const commandEncoder = device.createCommandEncoder();

// Create GPURenderPassDescriptor to tell WebGPU which texture to draw into, then initiate render pass
const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
};

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// Draw the triangle
passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

// End the render pass
passEncoder.end();

// End frame by passing array of command buffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/popdebuggroup/index.md
---
title: "GPURenderPassEncoder: popDebugGroup() method"
short-title: popDebugGroup()
slug: Web/API/GPURenderPassEncoder/popDebugGroup
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.popDebugGroup
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`popDebugGroup()`** method of the
{{domxref("GPURenderPassEncoder")}} interface ends a render pass debug group, which is begun with a {{domxref("GPURenderPassEncoder.pushDebugGroup", "pushDebugGroup()")}} call.

This could be used for telemetry, or may be utilized in {{domxref("GPUError")}} messages, browser dev tools, or other services in the future to help with debugging.

## Syntax

```js-nolint
popDebugGroup()
```

### Parameters

None.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`popDebugGroup()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderPassEncoder")}} becomes invalid:

- The render pass encoder's debug stack is not empty (i.e. at least one render pass debug group was previously started with {{domxref("GPURenderPassEncoder.pushDebugGroup", "pushDebugGroup()")}}).

## Examples

```js
// ...

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

passEncoder.pushDebugGroup("mygroupmarker"); // Start labeled debug group

passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

passEncoder.popDebugGroup();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/executebundles/index.md
---
title: "GPURenderPassEncoder: executeBundles() method"
short-title: executeBundles()
slug: Web/API/GPURenderPassEncoder/executeBundles
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.executeBundles
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`executeBundles()`** method of the
{{domxref("GPURenderPassEncoder")}} interface executes commands previously recorded into the referenced {{domxref("GPURenderBundle")}}s, as part of this render pass.

> **Note:** After calling `executeBundles()` the currently set vertex buffers, index buffers, bind groups, and pipeline are all cleared, even if no bundles are actually executed.

## Syntax

```js-nolint
executeBundles(bundles)
```

### Parameters

- `bundles`
  - : An array of {{domxref("GPURenderBundle")}} objects, containing the pre-recorded commands to execute.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`executeBundles()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderPassEncoder")}} becomes invalid.

For each {{domxref("GPURenderBundle")}}:

- If the render pass's `depthReadOnly` property (as specified in the descriptor of the originating {{domxref("GPUCommandEncoder.beginRenderPass()")}} call) is `true`, then the bundle's `depthReadOnly` property (as specified in the descriptor of the {{domxref("GPUDevice.createRenderBundleEncoder()")}} call that created the originating {{domxref("GPURenderBundleEncoder")}}) is also `true`.
- If the render pass's `stencilReadOnly` property (as specified in the descriptor of the originating {{domxref("GPUCommandEncoder.beginRenderPass()")}} call) is `true`, then the bundle's `stencilReadOnly` property (as specified in the descriptor of the {{domxref("GPUDevice.createRenderBundleEncoder()")}} call that created the originating {{domxref("GPURenderBundleEncoder")}}) is also `true`.
- The layout of the render pipeline specified in {{domxref("GPURenderPassEncoder.setPipeline()")}} (as defined in the descriptor of the originating {{domxref("GPUDevice.createRenderPipeline()")}} call) equals the layout of the render bundle pipeline specified in {{domxref("GPURenderBundleEncoder.setPipeline()")}}.

## Examples

In the WebGPU Samples [Animometer example](https://webgpu.github.io/webgpu-samples/samples/animometer), a lot of like operations are done on many different objects simultaneously. `executeBundles()` is used to reuse the work on multiple render passes to improve performance. Study the example code listing for the full context.

```js
// ...

return function doDraw(timestamp) {
  if (startTime === undefined) {
    startTime = timestamp;
  }
  uniformTime[0] = (timestamp - startTime) / 1000;
  device.queue.writeBuffer(uniformBuffer, timeOffset, uniformTime.buffer);

  renderPassDescriptor.colorAttachments[0].view = context
    .getCurrentTexture()
    .createView();

  const commandEncoder = device.createCommandEncoder();
  const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

  if (settings.renderBundles) {
    passEncoder.executeBundles([renderBundle]);
  } else {
    recordRenderPass(passEncoder);
  }

  passEncoder.end();
  device.queue.submit([commandEncoder.finish()]);
};

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/drawindexed/index.md
---
title: "GPURenderPassEncoder: drawIndexed() method"
short-title: drawIndexed()
slug: Web/API/GPURenderPassEncoder/drawIndexed
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.drawIndexed
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`drawIndexed()`** method of the
{{domxref("GPURenderPassEncoder")}} interface draws indexed primitives based on the vertex and index buffers provided by {{domxref("GPURenderPassEncoder.setVertexBuffer", "setVertexBuffer()")}} and {{domxref("GPURenderPassEncoder.setIndexBuffer", "setIndexBuffer()")}}.

## Syntax

```js-nolint
drawIndexed(indexCount)
drawIndexed(indexCount, instanceCount)
drawIndexed(indexCount, instanceCount, firstIndex)
drawIndexed(indexCount, instanceCount, firstIndex, baseVertex)
drawIndexed(indexCount, instanceCount, firstIndex, baseVertex, firstInstance)
```

### Parameters

- `indexCount`
  - : A number defining the number of indices to draw.
- `instanceCount` {{optional_inline}}
  - : A number defining the number of instances to draw. If omitted, `instanceCount` defaults to 1.
- `firstIndex` {{optional_inline}}
  - : A number defining the offset into the index buffer, in indices, to begin drawing from. If omitted, `firstIndex` defaults to 0.
- `baseVertex` {{optional_inline}}
  - : A number added to each index value before indexing into the vertex buffers. If omitted, `baseVertex` defaults to 0.
- `firstInstance` {{optional_inline}}
  - : A number defining the first instance to draw. If omitted, `firstInstance` defaults to 0.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

In the WebGPU Samples [Shadow Mapping](https://webgpu.github.io/webgpu-samples/samples/shadowMapping) example, `drawIndexed()` is used in two separate render passes in each animation frame, one to populate the shadow buffer and one to draw the primary view of the scene. Study the example code listing for the full context.

```js
// ...

const commandEncoder = device.createCommandEncoder();
{
  const shadowPass = commandEncoder.beginRenderPass(shadowPassDescriptor);
  shadowPass.setPipeline(shadowPipeline);
  shadowPass.setBindGroup(0, sceneBindGroupForShadow);
  shadowPass.setBindGroup(1, modelBindGroup);
  shadowPass.setVertexBuffer(0, vertexBuffer);
  shadowPass.setIndexBuffer(indexBuffer, "uint16");
  shadowPass.drawIndexed(indexCount);

  shadowPass.end();
}
{
  const renderPass = commandEncoder.beginRenderPass(renderPassDescriptor);
  renderPass.setPipeline(pipeline);
  renderPass.setBindGroup(0, sceneBindGroupForRender);
  renderPass.setBindGroup(1, modelBindGroup);
  renderPass.setVertexBuffer(0, vertexBuffer);
  renderPass.setIndexBuffer(indexBuffer, "uint16");
  renderPass.drawIndexed(indexCount);

  renderPass.end();
}

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/pushdebuggroup/index.md
---
title: "GPURenderPassEncoder: pushDebugGroup() method"
short-title: pushDebugGroup()
slug: Web/API/GPURenderPassEncoder/pushDebugGroup
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.pushDebugGroup
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`pushDebugGroup()`** method of the
{{domxref("GPURenderPassEncoder")}} interface begins a render pass debug group, which is marked with a specified label, and will contain all subsequent encoded commands up until a {{domxref("GPURenderPassEncoder.popDebugGroup", "popDebugGroup()")}} method is invoked.

This could be used for telemetry, or may be utilized in {{domxref("GPUError")}} messages, browser dev tools, or other services in the future to help with debugging.

## Syntax

```js-nolint
pushDebugGroup(groupLabel)
```

### Parameters

- `groupLabel`
  - : A string representing the label for the debug group.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
// ...

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

passEncoder.pushDebugGroup("mygroupmarker"); // Start labeled debug group

passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

passEncoder.popDebugGroup();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderpassencoder/draw/index.md
---
title: "GPURenderPassEncoder: draw() method"
short-title: draw()
slug: Web/API/GPURenderPassEncoder/draw
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderPassEncoder.draw
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`draw()`** method of the
{{domxref("GPURenderPassEncoder")}} interface draws primitives based on the vertex buffers provided by {{domxref("GPURenderPassEncoder.setVertexBuffer", "setVertexBuffer()")}}.

## Syntax

```js-nolint
draw(vertexCount)
draw(vertexCount, instanceCount)
draw(vertexCount, instanceCount, firstVertex)
draw(vertexCount, instanceCount, firstVertex, firstInstance)
```

### Parameters

- `vertexCount`
  - : A number defining the number of vertices to draw.
- `instanceCount` {{optional_inline}}
  - : A number defining the number of instances to draw. If omitted, `instanceCount` defaults to 1.
- `firstVertex` {{optional_inline}}
  - : A number defining the offset into the vertex buffers, in vertices, to begin drawing from. If omitted, `firstVertex` defaults to 0.
- `firstInstance` {{optional_inline}}
  - : A number defining the first instance to draw. If omitted, `firstInstance` defaults to 0.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/), several commands are recorded via a {{domxref("GPUCommandEncoder")}}. Most of these commands originate from the `GPURenderPassEncoder` created via {{domxref("GPUCommandEncoder.beginRenderPass()")}}. `draw()` is used to specify that three vertices should be drawn to create our triangle.

```js
// ...

const renderPipeline = device.createRenderPipeline(pipelineDescriptor);

// Create GPUCommandEncoder to issue commands to the GPU
// Note: render pass descriptor, command encoder, etc. are destroyed after use, fresh one needed for each frame.
const commandEncoder = device.createCommandEncoder();

// Create GPURenderPassDescriptor to tell WebGPU which texture to draw into, then initiate render pass
const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
};

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// Draw the triangle
passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

// End the render pass
passEncoder.end();

// End frame by passing array of command buffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuvalidationerror/index.md
---
title: GPUValidationError
slug: Web/API/GPUValidationError
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUValidationError
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUValidationError`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} describes an application error indicating that an operation did not pass the WebGPU API's validation constraints.

It represents one of the types of errors surfaced by {{domxref("GPUDevice.popErrorScope")}} and the {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event.

Validation errors occur whenever invalid inputs are given to a WebGPU call. These are consistent, predictable, and should not occur provided your app is well-formed. They will occur in the same way on every device your code runs on, so once you've fixed any errors that show up during development you probably don't need to observe them directly most of the time. An exception to that rule is if you're consuming user-supplied assets, shaders, etc., in which case watching for validation errors while loading could be helpful.

> **Note:** We have attempted to provide useful information to help you understand why validation errors are occurring in your WebGPU code in "Validation" sections where appropriate, which list criteria to meet to avoid validation errors. See for example the [`GPUDevice.createBindGroup()` Validation section](/en-US/docs/Web/API/GPUDevice/createBindGroup#validation).

{{InheritanceDiagram}}

## Constructor

- {{domxref("GPUValidationError.GPUValidationError", "GPUValidationError()")}} {{Experimental_Inline}}
  - : Creates a new `GPUValidationError` object instance.

## Instance properties

The `message` property is inherited from its parent, {{domxref("GPUError")}}:

- {{domxref("GPUError.message", "message")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A string providing a human-readable message that explains why the error occurred.

## Examples

The following example uses an error scope to capture a suspected validation error, logging it to the console.

```js
device.pushErrorScope("validation");

let sampler = device.createSampler({
  maxAnisotropy: 0, // Invalid, maxAnisotropy must be at least 1.
});

device.popErrorScope().then((error) => {
  if (error) {
    // error is a GPUValidationError object instance
    sampler = null;
    console.error(`An error occurred while creating sampler: ${error.message}`);
  }
});
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling)
-e 

File: /files/en-us/web/api/gpuvalidationerror/gpuvalidationerror/index.md
---
title: "GPUValidationError: GPUValidationError() constructor"
short-title: GPUValidationError()
slug: Web/API/GPUValidationError/GPUValidationError
page-type: web-api-constructor
status:
  - experimental
browser-compat: api.GPUValidationError.GPUValidationError
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUValidationError()`** constructor creates a new
{{domxref("GPUValidationError")}} object instance.

## Syntax

```js-nolint
new GPUValidationError(message)
```

### Parameters

- `message`
  - : A string providing a human-readable message that explains why the error occurred.

## Examples

A developer would not manually use the constructor to create a `GPUValidationError` object. The user agent uses this constructor to create an appropriate object when a validation error is surfaced by {{domxref("GPUDevice.popErrorScope")}} or the {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event.

See the main [`GPUValidationError`](/en-US/docs/Web/API/GPUValidationError#examples) page for a specific example involving a `GPUValidationError` object instance.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling)
-e 

File: /files/en-us/web/api/gpudevice/destroy/index.md
---
title: "GPUDevice: destroy() method"
short-title: destroy()
slug: Web/API/GPUDevice/destroy
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.destroy
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`destroy()`** method of the
{{domxref("GPUDevice")}} interface destroys the device, preventing further operations on it.

Note that:

- Any commands currently enqueued on the device's {{domxref("GPUQueue")}} will be executed before the device is destroyed.
- Any WebGPU resources created using the device (buffers, textures, etc.) are also destroyed.
- Any mapped buffers created using the device will be unmapped.

## Syntax

```js-nolint
destroy()
```

### Parameters

None.

### Return value

None ({{jsxref("undefined")}}).

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  let device = await adapter.requestDevice();

  // Some time later

  device.destroy();
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/createbindgroup/index.md
---
title: "GPUDevice: createBindGroup() method"
short-title: createBindGroup()
slug: Web/API/GPUDevice/createBindGroup
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createBindGroup
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createBindGroup()`** method of the
{{domxref("GPUDevice")}} interface creates a {{domxref("GPUBindGroup")}} based on a {{domxref("GPUBindGroupLayout")}} that defines a set of resources to be bound together in a group and how those resources are used in shader stages.

## Syntax

```js-nolint
createBindGroup(descriptor)
```

### Parameters

- `descriptor`
  - : An object containing the following properties:
    - `entries`
      - : An array of entry objects describing the resources to expose to the shader. There will be one for each corresponding entry described by the {{domxref("GPUBindGroupLayout")}} referenced in `layout`. Each entry object has the following properties:
        - `binding`
          - : A number representing a unique identifier for this resource binding, which matches the `binding` value of a corresponding {{domxref("GPUBindGroupLayout")}} entry. In addition, it matches the `n` index value of the corresponding [`@binding(n)`](https://gpuweb.github.io/gpuweb/wgsl/#attribute-binding) attribute in the shader ({{domxref("GPUShaderModule")}}) used in the related pipeline.
        - `resource`
          - : The resource to bind. This can be one of the following:
            - `GPUBufferBinding` (which wraps a {{domxref("GPUBuffer")}}; see [GPUBufferBinding objects](#gpubufferbinding_objects) for a definition)
            - {{domxref("GPUExternalTexture")}}
            - {{domxref("GPUSampler")}}
            - {{domxref("GPUTextureView")}}
    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
    - `layout`
      - : The {{domxref("GPUBindGroupLayout")}} that the `entries` of this bind group will conform to.

### GPUBufferBinding objects

A `GPUBufferBinding` object can contain the following properties:

- `buffer`
  - : The {{domxref("GPUBuffer")}} object you want to bind.
- `offset` {{optional_inline}}
  - : The offset, in bytes, from the beginning of the `buffer` to the beginning of the range exposed to the shader by the buffer binding. If omitted, `offset` defaults to 0.
- `size` {{optional_inline}}
  - : The size, in bytes, of the buffer binding. If omitted, `size` will be the range starting at `offset` and ending at the end of the `buffer`. If both `offset` and `size` are omitted, the entire buffer is exposed to the shader.

### Return value

A {{domxref("GPUBindGroup")}} object instance.

### Validation

The following criteria must be met when calling **`createBindGroup()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPUBindGroup")}} object is returned:

- The number of entries in the `layout` {{domxref("GPUBindGroupLayout")}} equals the number of entry objects in `entries`.
- For each entry in the `layout` {{domxref("GPUBindGroupLayout")}}, the corresponding entry object in `entries` binds the correct resource type. For example, a `buffer` resource layout object has a `GPUBufferBinding` object specified in the corresponding binding.
- If the resource layout object is a `buffer`:
  - The corresponding bound {{domxref("GPUBuffer")}}:
    - Has its bound part (as specified by `offset` and `size`) contained inside it completely, with a non-zero size.
    - Has a size bigger than the `buffer` resource layout's `minBindingSize`.
  - If the resource layout object `type` is `"uniform"`:
    - The bound {{domxref("GPUBuffer")}} has a `usage` that includes `GPUBufferUsage.UNIFORM`.
    - The effective size of the bound buffer segment is less than or equal to the {{domxref("GPUDevice")}}'s `maxUniformBufferBindingSize` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
    - The specified `GPUBufferBinding` `offset` is a multiple of the {{domxref("GPUDevice")}}'s `minUniformBufferOffsetAlignment` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
  - If the resource layout object `type` is `"storage"` or `"read-only-storage"`:
    - The bound {{domxref("GPUBuffer")}} has a `usage` that includes `GPUBufferUsage.STORAGE`.
    - The effective size of the bound buffer segment is less than or equal to the {{domxref("GPUDevice")}}'s `maxStorageBufferBindingSize` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
    - The effective size of the bound buffer segment is a multiple of 4.
    - The specified `GPUBufferBinding` `offset` is a multiple of the {{domxref("GPUDevice")}}'s `minStorageBufferOffsetAlignment` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- If the resource layout object is a `storageTexture`, the corresponding bound {{domxref("GPUTextureView")}}:
  - Has a `dimension` equal to the resource layout object's `viewDimension` (see {{domxref("GPUTexture.createView()")}} for more details of a texture view's settings).
  - Has a `format` equal to the resource layout object's `sampleType`.
  - Has a `mipLevelCount` equal to 1.
  - Is a view of a {{domxref("GPUTexture")}} with a `usage` that includes `GPUTextureUsage.STORAGE_BINDING`.
- If the resource layout object is a `texture`, the corresponding bound {{domxref("GPUTextureView")}}:
  - Has a `dimension` equal to the resource layout object's `viewDimension` (see {{domxref("GPUTexture.createView()")}} for more details of a texture view's settings).
  - Has a `format` compatible with the resource layout object's `sampleType`.
  - Is a view of a {{domxref("GPUTexture")}} with a `usage` that includes `GPUTextureUsage.TEXTURE_BINDING`.
  - is a view of a {{domxref("GPUTexture")}} with a `sampleCount` greater than 1 if the resource layout object's `multisampled` property is `true`, or equal to 1 if it is `false`.

## Examples

> **Note:** The [WebGPU samples](https://webgpu.github.io/webgpu-samples/) feature many more examples.

### Basic example

Our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/) shows an example of creating a bind group layout and then using that as a template when creating a bind group.

```js
// ...

const bindGroupLayout = device.createBindGroupLayout({
  entries: [
    {
      binding: 0,
      visibility: GPUShaderStage.COMPUTE,
      buffer: {
        type: "storage",
      },
    },
  ],
});

const bindGroup = device.createBindGroup({
  layout: bindGroupLayout,
  entries: [
    {
      binding: 0,
      resource: {
        buffer: output,
      },
    },
  ],
});

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/uncapturederror_event/index.md
---
title: "GPUDevice: uncapturederror event"
short-title: uncapturederror
slug: Web/API/GPUDevice/uncapturederror_event
page-type: web-api-event
status:
  - experimental
browser-compat: api.GPUDevice.uncapturederror_event
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`uncapturederror`** event of the {{domxref("GPUDevice")}} interface is fired when an error is thrown that has not been observed by a GPU error scope, to provide a way to report unexpected errors.

Known error cases should be handled using {{domxref("GPUDevice.pushErrorScope", "pushErrorScope()")}} and {{domxref("GPUDevice.popErrorScope", "popErrorScope()")}}.

## Syntax

Use the event name in methods like {{domxref("EventTarget.addEventListener", "addEventListener()")}}, or set an event handler property.

```js
addEventListener("uncapturederror", (event) => {});

onuncapturederror = (event) => {};
```

## Event type

An {{domxref("GPUUncapturedErrorEvent")}}. Inherits from {{domxref("Event")}}.

{{InheritanceDiagram("GPUUncapturedErrorEvent")}}

## Examples

You could use something like the following as a global mechanism to pick up any errors that aren't handled by error scopes and capture them.

```js
device.addEventListener("uncapturederror", (event) => {
  // Re-surface the error.
  console.error("A WebGPU error was not captured:", event.error);

  reportErrorToServer({
    type: event.error.constructor.name,
    message: event.error.message,
  });
});
```

See [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling) for more examples and information.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/lost/index.md
---
title: "GPUDevice: lost property"
short-title: lost
slug: Web/API/GPUDevice/lost
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUDevice.lost
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`lost`** read-only property of the
{{domxref("GPUDevice")}} interface contains a {{jsxref("Promise")}} that remains pending throughout the device's lifetime and resolves with a {{domxref("GPUDeviceLostInfo")}} object when the device is lost.

{{domxref("GPUAdapter.requestDevice()")}} will never return `null`, and it will reject only if the request is invalid, i.e. it exceeds the capabilities of the {{domxref("GPUAdapter")}}. If a valid device request can't be fulfilled for some reason however it may resolve to a device that has already been lost. Additionally, devices can be lost at any time after creation for a variety of reasons (such as browser resource management or driver updates), so it's a good idea to always handle lost devices gracefully.

Many causes for lost devices are transient, so you should try getting a new device once a previous one has been lost unless the loss was caused by the application intentionally destroying the device (i.e. with {{domxref("GPUDevice.destroy()")}}). Note that any WebGPU resources created with a previous device (buffers, textures, etc.) will need to be re-created with the new one.

> **Note:** Also bear in mind that a `GPUAdapter` may become unavailable, e.g. if the physical GPU is unplugged from the system or disabled to save power. From then on, the adapter can no longer return valid devices, and will always return already-lost devices.

## Value

A promise that resolves with a {{domxref("GPUDeviceLostInfo")}} object when the device is lost.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  // Create a GPUDevice
  let device = await adapter.requestDevice(descriptor);

  // Use lost to handle lost devices
  device.lost.then((info) => {
    console.error(`WebGPU device was lost: ${info.message}`);
    device = null;

    if (info.reason !== "destroyed") {
      init();
    }
  });

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/features/index.md
---
title: "GPUDevice: features property"
short-title: features
slug: Web/API/GPUDevice/features
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUDevice.features
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`features`** read-only property of the
{{domxref("GPUDevice")}} interface returns a {{domxref("GPUSupportedFeatures")}} object that describes additional functionality supported by the device. Only features requested during the creation of the device (i.e. when {{domxref("GPUAdapter.requestDevice()")}} is called) are included.

> **Note:** Not all features will be available to WebGPU in all browsers that support it, even if the features are supported by the underlying hardware. See {{domxref("GPUAdapter.features")}} for more details.

## Value

A {{domxref("GPUSupportedFeatures")}} object instance. This is a [setlike](/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set) object.

## Examples

In the following code we check whether a {{domxref("GPUAdapter")}} has the `texture-compression-astc` feature available. If so, we push it into the array of `requiredFeatures`, and request a device with that feature requirement using {{domxref("GPUAdapter.requestDevice()")}}.

We then log all items in the `GPUDevice.features` set to the console. This set should only contain a single item ‚Äî `texture-compression-astc` ‚Äî as that was the only feature requested when the device was created.

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const requiredFeatures = [];

  if (adapter.features.has("texture-compression-astc")) {
    requiredFeatures.push("texture-compression-astc");
  }

  const device = await adapter.requestDevice({
    requiredFeatures,
  });

  device.features.forEach((value) => {
    console.log(value);
  });

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/label/index.md
---
title: "GPUDevice: label property"
short-title: label
slug: Web/API/GPUDevice/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUDevice.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** read-only property of the
{{domxref("GPUDevice")}} interface is a string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Value

A string. If no label value has previously been set, getting the label returns an empty string.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  // Create a GPUDevice
  const device = await adapter.requestDevice();

  // Set a label
  device.label = "mylabel";

  // Get a label
  console.log(device.label);

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/createbuffer/index.md
---
title: "GPUDevice: createBuffer() method"
short-title: createBuffer()
slug: Web/API/GPUDevice/createBuffer
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createBuffer
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createBuffer()`** method of the
{{domxref("GPUDevice")}} interface creates a {{domxref("GPUBuffer")}} in which to store raw data to use in GPU operations.

## Syntax

```js-nolint
createBuffer(descriptor)
```

### Parameters

- `descriptor`

  - : An object containing the following properties:

    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
    - `mappedAtCreation` {{optional_inline}}

      - : A boolean. If set to `true`, the buffer will be mapped upon creation, meaning that you can set the values inside the buffer immediately by calling {{domxref("GPUBuffer.getMappedRange()")}}. The default value is `false`.

        Note that it is valid to set `mappedAtCreation: true` so you can set the buffer's initial data, even if the `GPUBufferUsage.MAP_READ` or `GPUBufferUsage.MAP_WRITE` usage flags are not set.

    - `size`
      - : A number representing the size of the buffer, in bytes.
    - `usage`

      - : The {{glossary("Bitwise flags", "bitwise flags")}} representing the allowed usages for the `GPUBuffer`. The possible values are in the [`GPUBuffer.usage` value table](/en-US/docs/Web/API/GPUBuffer/usage#value).

        Note that multiple possible usages can be specified by separating values with pipe symbols, for example:

        ```js
        usage: GPUBufferUsage.COPY_SRC | GPUBufferUsage.MAP_WRITE;
        ```

### Return value

A {{domxref("GPUBuffer")}} object instance.

### Validation

The following criteria must be met when calling **`createBuffer()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPUBuffer")}} object is returned:

- A valid `usage` is specified.
- `GPUBufferUsage.MAP_READ` is specified, and no additional flags are specified other than `GPUBufferUsage.COPY_DST`.
- `GPUBufferUsage.MAP_WRITE` is specified, and no additional flags are specified other than `GPUBufferUsage.COPY_SRC`.
- `mappedAtCreation: true` is specified, and the specified `size` is a multiple of 4.

> **Note:** If the buffer allocation fails without any specific side-effects, a {{domxref("GPUOutOfMemoryError")}} object is generated.

## Examples

In our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/), we create an output buffer to read GPU calculations to, and a staging buffer to be mapped for JavaScript access.

```js
const output = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.STORAGE | GPUBufferUsage.COPY_SRC,
});

const stagingBuffer = device.createBuffer({
  size: BUFFER_SIZE,
  usage: GPUBufferUsage.MAP_READ | GPUBufferUsage.COPY_DST,
});
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/limits/index.md
---
title: "GPUDevice: limits property"
short-title: limits
slug: Web/API/GPUDevice/limits
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUDevice.limits
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`limits`** read-only property of the
{{domxref("GPUDevice")}} interface returns a {{domxref("GPUSupportedLimits")}} object that describes the limits supported by the device. All limit values will be included, and the limits requested during the creation of the device (i.e. when {{domxref("GPUAdapter.requestDevice()")}} is called) will be reflected in those values.

> **Note:** Not all limits will be reported as expected, even if they are supported by the underlying hardware. See {{domxref("GPUAdapter.limits")}} for more details.

## Value

A {{domxref("GPUSupportedLimits")}} object instance.

## Examples

In the following code we query the `GPUAdapter.limits` value of `maxBindGroups` to see if it is equal to or greater than 6. Our theoretical example app ideally needs 6 bind groups, so if the returned value is >= 6, we add a maximum limit of 6 to the `requiredLimits` object.

We then check that the expected limit has been set on the resulting device by logging its value to the console.

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const requiredLimits = {};

  // App ideally needs 6 bind groups, so we'll try to request what the app needs
  if (adapter.limits.maxBindGroups >= 6) {
    requiredLimits.maxBindGroups = 6;
  }

  const device = await adapter.requestDevice({
    requiredLimits,
  });

  console.log(device.limits.maxBindGroups);

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/createrenderpipelineasync/index.md
---
title: "GPUDevice: createRenderPipelineAsync() method"
short-title: createRenderPipelineAsync()
slug: Web/API/GPUDevice/createRenderPipelineAsync
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createRenderPipelineAsync
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createRenderPipelineAsync()`** method of the
{{domxref("GPUDevice")}} interface returns a {{jsxref("Promise")}} that fulfills with a {{domxref("GPURenderPipeline")}}, which can control the vertex and fragment shader stages and be used in a {{domxref("GPURenderPassEncoder")}} or {{domxref("GPURenderBundleEncoder")}}, once the pipeline can be used without any stalling.

> **Note:** It is generally preferable to use this method over {{domxref("GPUDevice.createRenderPipeline()")}} whenever possible, as it prevents blocking of GPU operation execution on pipeline compilation.

## Syntax

```js-nolint
createRenderPipelineAsync(descriptor)
```

### Parameters

- `descriptor`
  - : See the descriptor definition for the [`GPUDevice.createRenderPipeline()`](/en-US/docs/Web/API/GPUDevice/createRenderPipeline#syntax) method.

### Return value

A {{jsxref("Promise")}} that fulfills with a {{domxref("GPURenderPipeline")}} object instance when the created pipeline is ready to be used without additional delay.

### Validation

If pipeline creation fails and the resulting pipeline becomes invalid as a result, the returned promise rejects with a {{domxref("GPUPipelineError")}}:

- If this is due to an internal error, the {{domxref("GPUPipelineError")}} will have a `reason` of `"internal"`.
- If this is due to a validation error, the {{domxref("GPUPipelineError")}} will have a `reason` of `"validation"`.

A validation error can occur if any of the following are false:

- For `depthStencil` objects:
  - `format` is a [`depth-or-stencil`](https://gpuweb.github.io/gpuweb/#depth-or-stencil-format) format.
  - If `depthWriteEnabled` is `true` or `depthCompare` is not `"always"`, `format` has a depth component.
  - If `stencilFront` or `stencilBack`'s properties are not at their default values, `format` has a stencil component.
- For `fragment` objects:
  - `targets.length` is less than or equal to the {{domxref("GPUDevice")}}'s `maxColorAttachments` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
  - For each `target`, `writeMask`'s numeric equivalent is less than 16.
  - If any of the used blend factor operations use the source alpha channel (for example `"src-alpha-saturated"`), the output has an alpha channel (that is, it must be a `vec4`).

## Examples

> **Note:** The [WebGPU samples](https://webgpu.github.io/webgpu-samples/) feature many more examples.

### Basic example

The following example shows a basic example of the construction of a valid render pipeline descriptor object, which is then used to create a {{domxref("GPURenderPipeline")}} via a `createRenderPipelineAsync()` call.

```js
async function init() {
  // ...

  const vertexBuffers = [
    {
      attributes: [
        {
          shaderLocation: 0, // position
          offset: 0,
          format: "float32x4",
        },
        {
          shaderLocation: 1, // color
          offset: 16,
          format: "float32x4",
        },
      ],
      arrayStride: 32,
      stepMode: "vertex",
    },
  ];

  const pipelineDescriptor = {
    vertex: {
      module: shaderModule,
      entryPoint: "vertex_main",
      buffers: vertexBuffers,
    },
    fragment: {
      module: shaderModule,
      entryPoint: "fragment_main",
      targets: [
        {
          format: navigator.gpu.getPreferredCanvasFormat(),
        },
      ],
    },
    primitive: {
      topology: "triangle-list",
    },
    layout: "auto",
  };

  const renderPipeline =
    await device.createRenderPipelineAsync(pipelineDescriptor);

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/createqueryset/index.md
---
title: "GPUDevice: createQuerySet() method"
short-title: createQuerySet()
slug: Web/API/GPUDevice/createQuerySet
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createQuerySet
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createQuerySet()`** method of the
{{domxref("GPUDevice")}} interface creates a {{domxref("GPUQuerySet")}} that can be used to record the results of queries on passes, such as occlusion or timestamp queries.

## Syntax

```js-nolint
createQuerySet(descriptor)
```

### Parameters

- `descriptor`

  - : An object containing the following properties:

    - `count`
      - : A number specifying the number of queries to be managed by the resulting {{domxref("GPUQuerySet")}}.
    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
    - `type`

      - : An enumerated value specifying the type of queries to be managed by the resulting {{domxref("GPUQuerySet")}}. Possible values are:

        - `"occlusion"`
          - : Occlusion queries are available on render passes to query the number of fragment samples that pass all the per-fragment tests for a set of drawing commands (including scissor, sample mask, alpha to coverage, stencil, and depth tests). To run an occlusion query, an appropriate {{domxref("GPUQuerySet")}} must be provided as the value of the `occlusionQuerySet` descriptor property when invoking {{domxref("GPUCommandEncoder.beginRenderPass()")}} to run a render pass.
        - `"timestamp"`

          - : Timestamp queries allow applications to write timestamps to a {{domxref("GPUQuerySet")}}. To run a timestamp query, appropriate {{domxref("GPUQuerySet")}}s must be provided inside the value of the `timestampWrites` descriptor property when invoking {{domxref("GPUCommandEncoder.beginRenderPass()")}} to run a render pass, or {{domxref("GPUCommandEncoder.beginComputePass()")}} to run a compute pass. Alternatively, you can run a single timestamp query at any time by invoking {{domxref("GPUCommandEncoder.writeTimeStamp()")}} with an appropriate {{domxref("GPUQuerySet")}} as a parameter.

            To use timestamp queries, the `timestamp-query` {{domxref("GPUSupportedFeatures", "feature", "", "nocode")}} must be enabled in the {{domxref("GPUDevice")}}.

### Return value

A {{domxref("GPUQuerySet")}} object instance.

### Validation

The following criteria must be met when calling **`createQuerySet()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPUQuerySet")}} object is returned:

- `count` is less than or equal to 4096.

## Examples

The following snippet creates a {{domxref("GPUQuerySet")}} that holds 32 occlusion query results:

```js
const querySet = device.createQuerySet({
  type: "occlusion",
  count: 32,
});
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/createpipelinelayout/index.md
---
title: "GPUDevice: createPipelineLayout() method"
short-title: createPipelineLayout()
slug: Web/API/GPUDevice/createPipelineLayout
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createPipelineLayout
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createPipelineLayout()`** method of the
{{domxref("GPUDevice")}} interface creates a {{domxref("GPUPipelineLayout")}} that defines the {{domxref("GPUBindGroupLayout")}}s used by a pipeline. {{domxref("GPUBindGroup")}}s used with the pipeline during command encoding must have compatible {{domxref("GPUBindGroupLayout")}}s.

## Syntax

```js-nolint
createPipelineLayout(descriptor)
```

### Parameters

- `descriptor`
  - : An object containing the following properties:
    - `bindGroupLayouts`
      - : An array of {{domxref("GPUBindGroupLayout")}} objects (which are in turn created via calls to {{domxref("GPUDevice.createBindGroupLayout()")}}). Each one corresponds to a [`@group`](https://gpuweb.github.io/gpuweb/wgsl/#attribute-binding) attribute in the shader code contained in the {{domxref("GPUShaderModule")}} used in a related pipeline.
    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

### Return value

A {{domxref("GPUPipelineLayout")}} object instance.

### Validation

The following criteria must be met when calling **`createPipelineLayout()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPUPipelineLayout")}} object is returned:

- The {{domxref("GPUBindGroupLayout")}} objects in `bindGroupLayouts` are valid.
- The number of {{domxref("GPUBindGroupLayout")}} objects in `bindGroupLayouts` is less than the {{domxref("GPUDevice")}}'s `maxBindGroups` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.

## Examples

> **Note:** The [WebGPU samples](https://webgpu.github.io/webgpu-samples/) feature many more examples.

### Multiple bind group layouts, bind group, and pipeline layout

The following snippet:

- Creates a {{domxref("GPUBindGroupLayout")}} that describes a binding with a buffer, a texture, and a sampler.
- Creates a {{domxref("GPUPipelineLayout")}} based on the {{domxref("GPUBindGroupLayout")}}.

```js
// ...

const bindGroupLayout = device.createBindGroupLayout({
  entries: [
    {
      binding: 0,
      visibility: GPUShaderStage.VERTEX | GPUShaderStage.FRAGMENT,
      buffer: {},
    },
    {
      binding: 1,
      visibility: GPUShaderStage.FRAGMENT,
      texture: {},
    },
    {
      binding: 2,
      visibility: GPUShaderStage.FRAGMENT,
      sampler: {},
    },
  ],
});

const pipelineLayout = device.createPipelineLayout({
  bindGroupLayouts: [bindGroupLayout],
});

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/createbindgrouplayout/index.md
---
title: "GPUDevice: createBindGroupLayout() method"
short-title: createBindGroupLayout()
slug: Web/API/GPUDevice/createBindGroupLayout
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createBindGroupLayout
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createBindGroupLayout()`** method of the
{{domxref("GPUDevice")}} interface creates a {{domxref("GPUBindGroupLayout")}} that defines the structure and purpose of related GPU resources such as buffers that will be used in a pipeline, and is used as a template when creating {{domxref("GPUBindGroup")}}s.

## Syntax

```js-nolint
createBindGroupLayout(descriptor)
```

### Parameters

- `descriptor`
  - : An object containing the following properties:
    - `entries`
      - : An array of [entry objects](#entry_objects), each one of which describes a single shader resource binding to be included in the {{domxref("GPUBindGroupLayout")}}. Each entry will correspond to an entry defined in a {{domxref("GPUBindGroup")}} (created via a {{domxref("GPUDevice.createBindGroup()")}} call) that uses this {{domxref("GPUBindGroupLayout")}} object as a template.
    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

### Entry objects

An entry object includes the following properties:

- `binding`
  - : A number representing a unique identifier for this particular entry, which matches the `binding` value of a corresponding {{domxref("GPUBindGroup")}} entry. In addition, it matches the `n` index value of the corresponding [`@binding(n)`](https://gpuweb.github.io/gpuweb/wgsl/#attribute-binding) attribute in the shader ({{domxref("GPUShaderModule")}}) used in the related pipeline.
- `visibility`

  - : One or more {{glossary("Bitwise_flags", "bitwise flags")}} defining the shader stages that a {{domxref("GPUBindGroup")}} entry corresponding to this entry will be visible to. Possible values are:

    - `GPUShaderStage.COMPUTE`: The bind group entry will be accessible to compute shaders.
    - `GPUShaderStage.FRAGMENT`: The bind group entry will be accessible to fragment shaders.
    - `GPUShaderStage.VERTEX`: The bind group entry will be accessible to vertex shaders.

    Note that multiple stages can be specified by separating values with pipe symbols, for example:

    ```js
    visibility: GPUShaderStage.FRAGMENT | GPUShaderStage.VERTEX;
    ```

- "Resource layout object"
  - : An object that defines the required binding resource type and structure of the {{domxref("GPUBindGroup")}} entry corresponding to this entry. This property can be one of `buffer`, `externalTexture`, `sampler`, `storageTexture`, or `texture`, the object structures of which are described in the next section.

### Resource layout objects

The resource layout object can be one of the following (see also {{domxref("GPUDevice.createBindGroup()")}} for details of how the required resources for each entry are structured):

- `buffer`: Indicates that the corresponding {{domxref("GPUBindGroup")}} entry will be a `GPUBufferBinding` object, which contains a {{domxref("GPUBuffer")}} plus `offset` and `size` values. A `buffer` resource layout object can contain the following properties:

  - `hasDynamicOffset` {{optional_inline}}

    - : A boolean. If set to `true`, it indicates that this binding requires a dynamic offset, for example as set during a {{domxref("GPURenderPassEncoder.setBindGroup()")}} call. If omitted, `hasDynamicOffset` defaults to `false`.

  - `minBindingSize` {{optional_inline}}

    - : A number indicating the minimum allowed size, in bytes, of bound buffers. If omitted, `minBindingSize` defaults to 0. If the value is 0, minimum buffer size is ignored during pipeline creation and is instead validated by issued draw/dispatch commands.

  - `type` {{optional_inline}}

    - : An enumerated value specifying the required type for {{domxref("GPUBuffer")}}s bound to this binding (see {{domxref("GPUDevice.createBuffer()")}} for more information on buffer types). Possible values are:

      - `"read-only-storage"`: A read-only buffer created with a `usage` of `GPUBufferUsage.STORAGE`.
      - `"storage"`: A writable buffer created with a `usage` of `GPUBufferUsage.STORAGE`.
      - `"uniform"`: A buffer created with a `usage` of `GPUBufferUsage.UNIFORM`.

      If omitted, `type` defaults to `"uniform"`.

- `externalTexture`: Indicates that the corresponding {{domxref("GPUBindGroup")}} entry will be a {{domxref("GPUExternalTexture")}} object. An `externalTexture` resource layout object is empty ‚Äî `{}`.

- `sampler`: Indicates that the corresponding {{domxref("GPUBindGroup")}} entry will be a {{domxref("GPUSampler")}} object. A `sampler` resource layout object can contain the following properties:

  - `type` {{optional_inline}}

    - : An enumerated value specifying the required type for {{domxref("GPUSampler")}}s bound to this binding (see {{domxref("GPUDevice.createSampler()")}} for more information on sampler types). Possible values are:

      - `"comparison"`: A comparison sampler.
      - `"filtering"`: A filtering sampler.
      - `"non-filtering"`: A non-filtering sampler.

      If omitted, `type` defaults to `"filtering"`.

- `storageTexture`: Indicates that the corresponding {{domxref("GPUBindGroup")}} entry will be a {{domxref("GPUTextureView")}} object. A `storageTexture` resource layout object can contain the following properties:

  - `access` {{optional_inline}}
    - : An enumerated value specifying whether texture views bound to this binding will be bound for read and/or write access. Possible values are currently `"write-only"` and `undefined`, with the intention to add more access modes in the future. If omitted, the default value is `"write-only"`.
  - `format`
    - : An enumerated value specifying the required format of texture views bound to this binding. See the specification's [Texture Formats](https://gpuweb.github.io/gpuweb/#enumdef-gputextureformat) section for all the available `format` values.
  - `viewDimension` {{optional_inline}}

    - : An enumerated value specifying the required dimension for texture views bound to this binding. Possible values are:

      - `"1d"`: The texture is viewed as a one-dimensional image.
      - `"2d"`: The texture is viewed as a single two-dimensional image.
      - `"2d-array"`: The texture is viewed as an array of two-dimensional images.
      - `"cube"`: The texture is viewed as a cubemap. The view has 6 array layers, corresponding to the `[+X, -X, +Y, -Y, +Z, -Z]` faces of the cube. Sampling is done seamlessly across the faces of the cubemap.
      - `"cube-array"`: The texture is viewed as a packed array of `n` cubemaps, each with 6 array layers corresponding to the `[+X, -X, +Y, -Y, +Z, -Z]` faces of the cube. Sampling is done seamlessly across the faces of the cubemaps.
      - `"3d"`: The texture is viewed as a three-dimensional image.

      If omitted, `viewDimension` defaults to `"2d"`.

- `texture`: Indicates that the corresponding {{domxref("GPUBindGroup")}} entry will be a {{domxref("GPUTextureView")}} object. A `texture` resource layout object can contain the following properties:

  - `multisampled` {{optional_inline}}

    - : A boolean. A value of `true` indicates that texture views bound to this binding must be multi-sampled. If omitted, `multisampled` defaults to `false`.

  - `sampleType` {{optional_inline}}

    - : An enumerated value specifying the sample type required for texture views bound to this binding (see {{domxref("GPUDevice.createTexture()")}} for more information on texture view types). Possible values are:

      - `"depth"`
      - `"float"`
      - `"sint"`
      - `"uint"`
      - `"unfilterable-float"`

      If omitted, `sampleType` defaults to `"float"`.

  - `viewDimension` {{optional_inline}}
    - : An enumerated value specifying the required dimension for texture views bound to this binding. Possible and default values are the same as for `storageTexture` resource layout objects ‚Äî see above.

### Return value

A {{domxref("GPUBindGroupLayout")}} object instance.

### Validation

The following criteria must be met when calling **`createBindGroupLayout()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPUBindGroupLayout")}} object is returned:

- Each entry's `binding` value is unique.
- Each entry's `binding` value is less than the {{domxref("GPUDevice")}}'s `maxBindingsPerBindGroup` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- The number of entries does not exceed the [binding slot limits](https://gpuweb.github.io/gpuweb/#exceeds-the-binding-slot-limits).
- Only 1 resource layout object is defined per entry.
- If an entry's `visibility` includes `GPUShaderStage.VERTEX`:
  - If its resource layout object is a `buffer`, its `type` is not `"storage"`.
  - Its resource layout object is not a `storageTexture`.
- If an entry's resource layout object is a `texture`, and its `multisampled` value is `true`:
  - Its `viewDimension` is `"2d"`.
  - Its `sampleType` is not `"float"`.
- If an entry's resource layout object is a `storageTexture`:
  - Its `viewDimension` is not `"cube"` or `"cube-array"`.
  - Its `format` is a format that supports storage usage.

## Examples

> **Note:** The [WebGPU samples](https://webgpu.github.io/webgpu-samples/) feature many more examples.

### Basic example

Our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/) shows an example of creating a bind group layout and then using that as a template when creating a bind group.

```js
// ...

const bindGroupLayout = device.createBindGroupLayout({
  entries: [
    {
      binding: 0,
      visibility: GPUShaderStage.COMPUTE,
      buffer: {
        type: "storage",
      },
    },
  ],
});

const bindGroup = device.createBindGroup({
  layout: bindGroupLayout,
  entries: [
    {
      binding: 0,
      resource: {
        buffer: output,
      },
    },
  ],
});

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/createrenderpipeline/index.md
---
title: "GPUDevice: createRenderPipeline() method"
short-title: createRenderPipeline()
slug: Web/API/GPUDevice/createRenderPipeline
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createRenderPipeline
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createRenderPipeline()`** method of the
{{domxref("GPUDevice")}} interface creates a {{domxref("GPURenderPipeline")}} that can control the vertex and fragment shader stages and be used in a {{domxref("GPURenderPassEncoder")}} or {{domxref("GPURenderBundleEncoder")}}.

## Syntax

```js-nolint
createRenderPipeline(descriptor)
```

### Parameters

- `descriptor`
  - : An object containing the following properties:
    - `depthStencil` {{optional_inline}}
      - : An object (see [`depthStencil` object structure](#depthstencil_object_structure)) describing depth-stencil properties including testing, operations, and bias.
    - `fragment` {{optional_inline}}
      - : An object (see [`fragment` object structure](#fragment_object_structure)) describing the fragment shader entry point of the pipeline and its output colors. If no fragment shader entry point is defined, the pipeline will not produce any color attachment outputs, but it still performs rasterization and produces depth values based on the vertex position output. Depth testing and stencil operations can still be used.
    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
    - `layout`
      - : Defines the layout (structure, purpose, and type) of all the GPU resources (buffers, textures, etc.) used during the execution of the pipeline. Possible values are:
        - A {{domxref("GPUPipelineLayout")}} object, created using {{domxref("GPUDevice.createPipelineLayout()")}}, which allows the GPU to figure out how to run the pipeline most efficiently ahead of time.
        - A string of `"auto"`, which causes the pipeline to generate an implicit bind group layout based on any bindings defined in the shader code. If `"auto"` is used, the generated bind group layouts may only be used with the current pipeline.
    - `multisample` {{optional_inline}}
      - : An object (see [`multisample` object structure](#multisample_object_structure)) describing how the pipeline interacts with a render pass's multisampled attachments.
    - `primitive` {{optional_inline}}
      - : An object (see [`primitive` object structure](#primitive_object_structure)) describing how a pipeline constructs and rasterizes primitives from its vertex inputs.
    - `vertex`
      - : An object (see [`vertex` object structure](#vertex_object_structure)) describing the vertex shader entry point of the pipeline and its input buffer layouts.

### `depthStencil` object structure

The `depthStencil` object can contain the following properties:

- `depthBias` {{optional_inline}}
  - : A number representing a constant depth bias that is added to each fragment. If omitted, `depthBias` defaults to 0.
- `depthBiasClamp` {{optional_inline}}
  - : A number representing the maximum depth bias of a fragment. If omitted, `depthBiasClamp` defaults to 0.
- `depthBiasSlopeScale` {{optional_inline}}
  - : A number representing a depth bias that scales with the fragment's slope. If omitted, `depthBiasSlopeScale` defaults to 0.
- `depthCompare`

  - : An enumerated value specifying the comparison operation used to test fragment depths against `depthStencilAttachment` depth values. Possible values are:

    - `"never"`: Comparison tests never pass.
    - `"less"`: A provided value passes the comparison test if it is less than the sampled value.
    - `"equal"`: A provided value passes the comparison test if it is equal to the sampled value.
    - `"less-equal"`: A provided value passes the comparison test if it is less than or equal to the sampled value.
    - `"greater"`: A provided value passes the comparison test if it is greater than the sampled value.
    - `"not-equal"`: A provided value passes the comparison test if it is not equal to the sampled value.
    - `"greater-equal"`: A provided value passes the comparison test if it is greater than or equal to the sampled value.
    - `"always"`: Comparison tests always pass.

- `depthWriteEnabled`
  - : A boolean. A value of `true` specifies that the {{domxref("GPURenderPipeline")}} can modify `depthStencilAttachment` depth values after creation. Setting it to `false` means it cannot.
- `format`
  - : An enumerated value specifying the `depthStencilAttachment` format that the {{domxref("GPURenderPipeline")}} will be compatible with. See the specification's [Texture Formats](https://gpuweb.github.io/gpuweb/#enumdef-gputextureformat) section for all the available `format` values.
- `stencilBack` {{optional_inline}}

  - : An object that defines how stencil comparisons and operations are performed for back-facing primitives. Its properties can include:

    - `compare` {{optional_inline}}
      - : An enumerated value specifying the comparison operation used when testing fragments against `depthStencilAttachment` stencil values. Possible values are the same as for the `depthCompare` property; see above. If omitted, `compare` defaults to `"always"`.
    - `depthFailOp` {{optional_inline}}

      - : An enumerated value specifying the stencil operation performed if the fragment depth comparison described by `depthCompare` fails. Possible values are:

        - `"decrement-clamp"`: Decrement the current render state stencil value, clamping it to 0.
        - `"decrement-wrap"`: Decrement the current render state stencil value, wrapping it to the maximum representable value of the `depthStencilAttachment`'s stencil aspect if the value goes below 0.
        - `"invert"`: Bitwise-invert the current render state stencil value.
        - `"increment-clamp"`: Increments the current render state stencil value, clamping it to the maximum representable value of the `depthStencilAttachment`'s stencil aspect.
        - `"increment-wrap"`: Increments the current render state stencil value, wrapping it to zero if the value exceeds the maximum representable value of the `depthStencilAttachment`'s stencil aspect.
        - `"keep"`: Keep the current stencil value.
        - `"replace"`: Set the stencil value to the current render state stencil value.
        - `"zero"`: Set the stencil value to 0.

        If omitted, `depthFailOp` defaults to `"keep"`.

        > **Note:**: The render state stencil value is initialized to 0 at the start of a render pass.

    - `failOp` {{optional_inline}}
      - : An enumerated value specifying the stencil operation performed if the fragment stencil comparison test described by `compare` fails. Possible and default values are the same as for `depthFailOp`.
    - `passOp` {{optional_inline}}
      - : An enumerated value specifying the stencil operation performed if the fragment stencil comparison test described by `compare` passes. Possible and default values are the same as for `depthFailOp`.

- `stencilFront` {{optional_inline}}
  - : An object that defines how stencil comparisons and operations are performed for front-facing primitives. Its properties are the same as for `stencilBack`.
- `stencilReadMask` {{optional_inline}}
  - : A bitmask controlling which `depthStencilAttachment` stencil value bits are read when performing stencil comparison tests. If omitted, `stencilReadMask` defaults to `0xFFFFFFFF`.
- `stencilWriteMask` {{optional_inline}}
  - : A bitmask controlling which `depthStencilAttachment` stencil value bits are written to when performing stencil operations. If omitted, `stencilWriteMask` defaults to `0xFFFFFFFF`.

> **Note:** `depthStencilAttachment` values are specified during {{domxref("GPUCommandEncoder.beginRenderPass()")}} calls, when the {{domxref("GPURenderPipeline")}} is actually used to perform a render pass.

### `fragment` object structure

The `fragment` object contains an array of objects, each of which can contain the following properties:

- `constants` {{optional_inline}}

  - : A sequence of record types, with the structure `(id, value)`, representing override values for [WGSL constants that can be overridden in the pipeline](https://gpuweb.github.io/gpuweb/#typedefdef-gpupipelineconstantvalue). These behave like [ordered maps](/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map). In each case, the `id` is a key used to identify or select the record, and the `constant` is an enumerated value representing a WGSL.

    Depending on which constant you want to override, the `id` may take the form of the numeric ID of the constant, if one is specified, or otherwise the constant's identifier name.

    A code snippet providing override values for several overridable constants might look like this:

    ```js
    {
      // ...
      constants: {
        0: false,
        1200: 3.0,
        1300: 2.0,
        width: 20,
        depth: -1,
        height: 15,
      }
    }
    ```

- `entryPoint`
  - : The name of the function in the `module` that this stage will use to perform its work. The corresponding shader function must have the `@fragment` attribute to be identified as this entry point. See [Entry Point Declaration](https://gpuweb.github.io/gpuweb/wgsl/#entry-point-decl) for more information.
- `module`
  - : A {{domxref("GPUShaderModule")}} object containing the [WGSL](https://gpuweb.github.io/gpuweb/wgsl/) code that this programmable stage will execute.
- `targets`

  - : an array of objects representing color states that represent configuration details for the colors output by the fragment shader stage. These objects can include the following properties:

    - `blend` {{optional_inline}}

      - : A object that describes a blend mode to be applied to the output color. `blend` has two properties:

        - `alpha`
          - : Describes the alpha channel value.
        - `color`
          - : Describes the color value.

        `alpha` and `color` both take an object as a value that can include the following properties:

        - `dstFactor` {{optional_inline}}

          - : An enumerated value that defines the blend factor operation to be performed on values from the target attachment. Possible values are:

            - `"constant"`
            - `"dst"`
            - `"dst-alpha"`
            - `"one"`
            - `"one-minus-dst"`
            - `"one-minus-src"`
            - `"one-minus-src-alpha"`
            - `"one-minus-dst-alpha"`
            - `"one-minus-constant"`
            - `"src"`
            - `"src-alpha"`
            - `"src-alpha-saturated"`
            - `"zero"`

            If omitted, `dstFactor` defaults to `"zero"`.

        - `operation` {{optional_inline}}

          - : An enumerated value that defines the algorithm used to combine source and destination blend factors, to calculate the final values written to the target attachment components. Possible values are:

            - `"add"`
            - `"max"`
            - `"min"`
            - `"reverse-subtract"`
            - `"subtract"`

            If omitted, `operation` defaults to `"add"`.

        - `srcFactor` {{optional_inline}}
          - : An enumerated value that defines the blend factor operation to be performed on values from the fragment shader. Possible values are the same as for `dstFactor`. If omitted, `srcFactor` defaults to `"one"`.

        > **Note:** For a detailed explanation of the algorithms defined by each `dstFactor`/`srcFactor` and `operation` enumerated value, see the [Blend State](https://gpuweb.github.io/gpuweb/#blend-state) section of the specification.

    - `format`
      - : An enumerated value specifying the required format for output colors. See the specification's [Texture Formats](https://gpuweb.github.io/gpuweb/#enumdef-gputextureformat) section for all the available `format` values.
    - `writeMask` {{optional_inline}}

      - : One or more {{glossary("bitwise flags")}} defining the write mask to apply to the color target state. Possible flag values are:

        - `GPUFlagsConstant.RED`
        - `GPUFlagsConstant.GREEN`
        - `GPUFlagsConstant.BLUE`
        - `GPUFlagsConstant.ALPHA`
        - `GPUFlagsConstant.ALL`

        If omitted, `writeMask` defaults to `GPUFlagsConstant.ALL`.

        Note that multiple flags can be specified by separating values with pipe symbols, for example:

        ```js
        writeMask: GPUFlagsConstant.RED | GPUFlagsConstant.ALPHA;
        ```

### `multisample` object structure

The `multisample` object can contain the following properties:

- `alphaToCoverageEnabled` {{optional_inline}}
  - : A boolean. A value of `true` indicates that a fragment's alpha channel should be used to generate a sample coverage mask. If omitted, `alphaToCoverageEnabled` defaults to `false`.
- `count` {{optional_inline}}

  - : A number that defines the number of samples per pixel. The pipeline will be compatible only with attachment textures (`colorAttachment`s and `depthStencilAttachment`s) with matching `sampleCounts` (see {{domxref("GPUTexture")}}).

    If omitted, `count` defaults to 1.

- `mask` {{optional_inline}}
  - : A bitmask that determines which samples are written to. If omitted, `mask` defaults to `0xFFFFFFFF`.

> **Note:** `colorAttachment` and `depthStencilAttachment` values are specified during {{domxref("GPUCommandEncoder.beginRenderPass()")}} calls, when the {{domxref("GPURenderPipeline")}} is actually used to perform a render pass.

### `primitive` object structure

The `primitive` object can contain the following properties:

- `cullMode` {{optional_inline}}

  - : An enumerated value that defines which polygon orientation will be culled, if any. Possible values are:

    - `"back"`: Back-facing polygons are culled.
    - `"front"`: Front-facing polygons are culled.
    - `"none"`: No polygons are culled.

    If omitted, `cullMode` defaults to `"none"`.

- `frontFace` {{optional_inline}}

  - : An enumerated value that defines which polygons are considered front-facing. Possible values are:

    - `"ccw"`: Polygons with vertices whose framebuffer coordinates are given in counter-clockwise order.
    - `"cw"`: Polygons with vertices whose framebuffer coordinates are given in clockwise order.

    If omitted, `frontFace` defaults to `"ccw"`.

- `stripIndexFormat` {{optional_inline}}

  - : An enumerated value that determines the index buffer format and primitive restart value in the case of pipelines with strip topologies (`"line-strip"` or `"triangle-strip"`). The primitive restart value specifies which index value indicates that a new primitive should be started rather than continuing to construct the strip with the prior indexed vertices. Possible values are:

    - `"uint16"`: Indicates a byte size of 2 and a primitive restart value of `0xFFFF`.
    - `"uint32"`: Indicates a byte size of 4 and a primitive restart value of `0xFFFFFFFF`.

    GPU primitive states that specify a strip primitive topology must specify a strip index format if they are used for indexed draws (for example, via {{domxref("GPURenderPassEncoder.drawIndexed()")}}) so that the primitive restart value that will be used is known at pipeline creation time. Pipelines with list primitive topologies (`"line-list"`, `"point-list"`, or `"triangle-list"`) should not specify a `stripIndexFormat` value. They will instead use the index format passed to, for example, {{domxref("GPURenderPassEncoder.setIndexBuffer()")}} when doing indexed rendering.

- `topology` {{optional_inline}}

  - : An enumerated value that defines the type of primitive to be constructed from the specified `vertex` inputs. Possible values are:

    - `"line-list"`: Each consecutive pair of two vertices defines a line primitive.
    - `"line-strip"`: Each vertex after the first defines a line primitive between it and the previous vertex.
    - `"point-list"`: Each vertex defines a point primitive.
    - `"triangle-list"`: Each consecutive triplet of three vertices defines a triangle primitive.
    - `"triangle-strip"`: Each vertex after the first two defines a triangle primitive between it and the previous two vertices.

    If omitted, `topology` defaults to `"triangle-list"`.

- `unclippedDepth` {{optional_inline}}
  - : A boolean. A value of `true` indicates that depth clipping is disabled. If omitted, `unclippedDepth` defaults to `false`. Note that to control depth clipping, the `depth-clip-control` {{domxref("GPUSupportedFeatures", "feature", "", "nocode")}} must be enabled in the {{domxref("GPUDevice")}}.

> **Note:** `frontFace` and `cullMode` have no effect on `"point-list"`, `"line-list"`, or `"line-strip"` topologies.

### `vertex` object structure

The `vertex` object can contain the following properties:

- `constants` {{optional_inline}}

  - : A sequence of record types, with the structure `(id, value)`, representing override values for [WGSL constants that can be overridden in the pipeline](https://gpuweb.github.io/gpuweb/#typedefdef-gpupipelineconstantvalue). These behave like [ordered maps](/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map). In each case, the `id` is a key used to identify or select the record, and the `constant` is an enumerated value representing a WGSL.

    Depending on which constant you want to override, the `id` may take the form of the numeric ID of the constant, if one is specified, or otherwise the constant's identifier name.

    A code snippet providing override values for several overridable constants might look like this:

    ```js
    {
      // ...
      constants: {
        0: false,
        1200: 3.0,
        1300: 2.0,
        width: 20,
        depth: -1,
        height: 15,
      }
    }
    ```

- `entryPoint`
  - : The name of the function in the `module` that this stage will use to perform its work. The corresponding shader function must have the `@vertex` attribute to be identified as this entry point. See [Entry Point Declaration](https://gpuweb.github.io/gpuweb/wgsl/#entry-point-decl) for more information.
- `module`
  - : A {{domxref("GPUShaderModule")}} object containing the [WGSL](https://gpuweb.github.io/gpuweb/wgsl/) code that this programmable stage will execute.
- `buffers` {{optional_inline}}

  - : An array of objects, each representing the expected layout of a vertex buffer used in the pipeline. Each object can contain the following properties:

    - `arrayStride`
      - : A number representing the stride, in bytes, between the different structures (e.g. vertices) inside the buffer.
    - `attributes`
      - : An array of objects defining the layout of the vertex attributes within each structure. Each object has the following properties:
        - `format`
          - : An enumerated value that specifies the format of the vertex. For all the available values, see the [`GPUVertexFormat`](https://gpuweb.github.io/gpuweb/#enumdef-gpuvertexformat) definition in the specification.
        - `offset`
          - : A number specifying the offset, in bytes, from the beginning of the structure to the data for the attribute.
        - `shaderLocation`
          - : The numeric location associated with this attribute, which will correspond with a [`@location`](https://gpuweb.github.io/gpuweb/wgsl/#input-output-locations) attribute declared in the WGSL code of the associated {{domxref("GPUShaderModule")}} referenced in the `vertex` object's `module` property.
    - `stepMode` {{optional_inline}}

      - : An enumerated value that defines whether the separate structures inside the buffer represent vertices or instances. Possible values are:

        - `"instance"`: Each structure is an instance ‚Äî the address is advanced by `arrayStride` for each instance.
        - `"vertex"`: Each structure is a vertex ‚Äî the address is advanced by `arrayStride` for each vertex, and reset between instances.

        If omitted, `stepMode` defaults to `"vertex"`.

### Return value

A {{domxref("GPURenderPipeline")}} object instance.

### Validation

The following criteria must be met when calling **`createRenderPipeline()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPURenderPipeline")}} object is returned:

- For `depthStencil` objects:
  - `format` is a [`depth-or-stencil`](https://gpuweb.github.io/gpuweb/#depth-or-stencil-format) format.
  - If `depthWriteEnabled` is `true` or `depthCompare` is not `"always"`, `format` has a depth component.
  - If `stencilFront` or `stencilBack`'s properties are not at their default values, `format` has a stencil component.
- For `fragment` objects:
  - `targets.length` is less than or equal to the {{domxref("GPUDevice")}}'s `maxColorAttachments` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
  - For each `target`, `writeMask`'s numeric equivalent is less than 16.
  - If any of the used blend factor operations use the source alpha channel (for example `"src-alpha-saturated"`), the output has an alpha channel (that is, it must be a `vec4`).

## Examples

> **Note:** The [WebGPU samples](https://webgpu.github.io/webgpu-samples/) feature many more examples.

### Basic example

Our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/) provides a simple example of the construction of a valid render pipeline descriptor object, which is then used to create a {{domxref("GPURenderPipeline")}} via a `createRenderPipeline()` call.

```js
// ...

const vertexBuffers = [
  {
    attributes: [
      {
        shaderLocation: 0, // position
        offset: 0,
        format: "float32x4",
      },
      {
        shaderLocation: 1, // color
        offset: 16,
        format: "float32x4",
      },
    ],
    arrayStride: 32,
    stepMode: "vertex",
  },
];

const pipelineDescriptor = {
  vertex: {
    module: shaderModule,
    entryPoint: "vertex_main",
    buffers: vertexBuffers,
  },
  fragment: {
    module: shaderModule,
    entryPoint: "fragment_main",
    targets: [
      {
        format: navigator.gpu.getPreferredCanvasFormat(),
      },
    ],
  },
  primitive: {
    topology: "triangle-list",
  },
  layout: "auto",
};

const renderPipeline = device.createRenderPipeline(pipelineDescriptor);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/importexternaltexture/index.md
---
title: "GPUDevice: importExternalTexture() method"
short-title: importExternalTexture()
slug: Web/API/GPUDevice/importExternalTexture
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.importExternalTexture
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`importExternalTexture()`** method of the
{{domxref("GPUDevice")}} interface takes an {{domxref("HTMLVideoElement")}} or a {{domxref("VideoFrame")}} object as an input and returns a {{domxref("GPUExternalTexture")}} wrapper object containing a snapshot of the video that can be used as a frame in GPU rendering operations.

## Syntax

```js-nolint
importExternalTexture(descriptor)
```

### Parameters

- `descriptor`
  - : An object containing the following properties:
    - `colorSpace` {{optional_inline}}
      - : An enumerated value specifying the color space to use for the video frame. Possible values are `"srgb"` and `"display-p3"`. If omitted, `colorSpace` defaults to `"srgb"`.
    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
    - `source`
      - : The {{domxref("HTMLVideoElement")}} or {{domxref("VideoFrame")}} source of the video snapshot.

### Return value

A {{domxref("GPUExternalTexture")}} object instance.

Note that the moment when the {{domxref("GPUExternalTexture")}} object expires (is destroyed) depends on what its source is:

- {{domxref("GPUExternalTexture")}} objects with an {{domxref("HTMLVideoElement")}} source expire as soon as they are used (for example in a bind group).
- {{domxref("GPUExternalTexture")}} objects with an {{domxref("VideoFrame")}} source expire only when the `VideoFrame` is closed, for example via a {{domxref("VideoFrame.close()")}} call.

### Validation

The following criteria must be met when calling **`importExternalTexture()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPUExternalTexture")}} object is returned:

- The video snapshot is usable (e.g. the video source is loaded properly, and doesn't have a width or height of 0).

### Exceptions

- `SecurityError` {{domxref("DOMException")}}
  - : Thrown if the video source data is cross-origin.

## Examples

In the WebGPU samples [Video Uploading sample](https://webgpu.github.io/webgpu-samples/samples/videoUploading), an `importExternalTexture()` call is used as the value of a bind group entry `resource`, specified when creating a {{domxref("GPUBindGroup")}} via a {{domxref("GPUDevice.createBindGroup()")}} call:

```js
//...

const uniformBindGroup = device.createBindGroup({
  layout: pipeline.getBindGroupLayout(0),
  entries: [
    {
      binding: 1,
      resource: sampler,
    },
    {
      binding: 2,
      resource: device.importExternalTexture({
        source: video,
      }),
    },
  ],
});

//...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/index.md
---
title: GPUDevice
slug: Web/API/GPUDevice
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUDevice
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUDevice`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents a logical GPU device. This is the main interface through which the majority of WebGPU functionality is accessed.

A `GPUDevice` object is requested using the {{domxref("GPUAdapter.requestDevice()")}} method.

{{InheritanceDiagram}}

## Instance properties

_Inherits properties from its parent, {{DOMxRef("EventTarget")}}._

- {{domxref("GPUDevice.features", "features")}} {{Experimental_Inline}} {{ReadOnlyInline}}

  - : A {{domxref("GPUSupportedFeatures")}} object that describes additional functionality supported by the device.

- {{domxref("GPUDevice.label", "label")}} {{Experimental_Inline}}

  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

- {{domxref("GPUDevice.limits", "limits")}} {{Experimental_Inline}} {{ReadOnlyInline}}

  - : A {{domxref("GPUSupportedLimits")}} object that describes the limits supported by the device.

- {{domxref("GPUDevice.lost", "lost")}} {{Experimental_Inline}} {{ReadOnlyInline}}

  - : Contains a {{jsxref("Promise")}} that remains pending throughout the device's lifetime and resolves with a {{domxref("GPUDeviceLostInfo")}} object when the device is lost.

- {{domxref("GPUDevice.queue", "queue")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : Returns the primary {{domxref("GPUQueue")}} for the device.

## Instance methods

_Inherits methods from its parent, {{DOMxRef("EventTarget")}}._

- {{domxref("GPUDevice.createBindGroup", "createBindGroup()")}} {{Experimental_Inline}}

  - : Creates a {{domxref("GPUBindGroup")}} based on a {{domxref("GPUBindGroupLayout")}} that defines a set of resources to be bound together in a group and how those resources are used in shader stages.

- {{domxref("GPUDevice.createBindGroupLayout", "createBindGroupLayout()")}} {{Experimental_Inline}}

  - : Creates a {{domxref("GPUBindGroupLayout")}} that defines the structure and purpose of related GPU resources such as buffers that will be used in a pipeline, and is used as a template when creating {{domxref("GPUBindGroup")}}s.

- {{domxref("GPUDevice.createBuffer", "createBuffer()")}} {{Experimental_Inline}}

  - : Creates a {{domxref("GPUBuffer")}} in which to store raw data to use in GPU operations.

- {{domxref("GPUDevice.createCommandEncoder", "createCommandEncoder()")}} {{Experimental_Inline}}

  - : Creates a {{domxref("GPUCommandEncoder")}}, which is used to encode commands to be issued to the GPU.

- {{domxref("GPUDevice.createComputePipeline", "createComputePipeline()")}} {{Experimental_Inline}}

  - : Creates a {{domxref("GPUComputePipeline")}} that can control the compute shader stage and be used in a {{domxref("GPUComputePassEncoder")}}.

- {{domxref("GPUDevice.createComputePipelineAsync", "createComputePipelineAsync()")}} {{Experimental_Inline}}

  - : Returns a {{jsxref("Promise")}} that fulfills with a {{domxref("GPUComputePipeline")}}, which can control the compute shader stage and be used in a {{domxref("GPUComputePassEncoder")}}, once the pipeline can be used without any stalling.

- {{domxref("GPUDevice.createPipelineLayout", "createPipelineLayout()")}} {{Experimental_Inline}}

  - : Creates a {{domxref("GPUPipelineLayout")}} that defines the {{domxref("GPUBindGroupLayout")}}s used by a pipeline. {{domxref("GPUBindGroup")}}s used with the pipeline during command encoding must have compatible {{domxref("GPUBindGroupLayout")}}s.

- {{domxref("GPUDevice.createQuerySet", "createQuerySet()")}} {{Experimental_Inline}}

  - : Creates a {{domxref("GPUQuerySet")}} that can be used to record the results of queries on passes, such as occlusion or timestamp queries.

- {{domxref("GPUDevice.createRenderBundleEncoder", "createRenderBundleEncoder()")}} {{Experimental_Inline}}

  - : Creates a {{domxref("GPURenderBundleEncoder")}} that can be used to pre-record bundles of commands. These can be reused in {{domxref("GPURenderPassEncoder")}}s via the {{domxref("GPURenderPassEncoder.executeBundles", "executeBundles()")}} method, as many times as required.

- {{domxref("GPUDevice.createRenderPipeline", "createRenderPipeline()")}} {{Experimental_Inline}}

  - : Creates a {{domxref("GPURenderPipeline")}} that can control the vertex and fragment shader stages and be used in a {{domxref("GPURenderPassEncoder")}} or {{domxref("GPURenderBundleEncoder")}}.

- {{domxref("GPUDevice.createRenderPipelineAsync", "createRenderPipelineAsync()")}} {{Experimental_Inline}}

  - : Returns a {{jsxref("Promise")}} that fulfills with a {{domxref("GPURenderPipeline")}}, which can control the vertex and fragment shader stages and be used in a {{domxref("GPURenderPassEncoder")}} or {{domxref("GPURenderBundleEncoder")}}, once the pipeline can be used without any stalling.

- {{domxref("GPUDevice.createSampler", "createSampler()")}} {{Experimental_Inline}}

  - : Creates a {{domxref("GPUSampler")}}, which controls how shaders transform and filter texture resource data.

- {{domxref("GPUDevice.createShaderModule", "createShaderModule()")}} {{Experimental_Inline}}

  - : Creates a {{domxref("GPUShaderModule")}} from a string of WGSL source code.

- {{domxref("GPUDevice.createTexture", "createTexture()")}} {{Experimental_Inline}}

  - : Creates a {{domxref("GPUTexture")}} in which to store texture data to use in GPU rendering operations.

- {{domxref("GPUDevice.destroy", "destroy()")}} {{Experimental_Inline}}

  - : Destroys the device, preventing further operations on it.

- {{domxref("GPUDevice.importExternalTexture", "importExternalTexture()")}} {{Experimental_Inline}}

  - : Takes an {{domxref("HTMLVideoElement")}} as an input and returns a {{domxref("GPUExternalTexture")}} wrapper object containing a snapshot of the video that can be used in GPU rendering operations.

- {{domxref("GPUDevice.popErrorScope", "popErrorScope()")}} {{Experimental_Inline}}

  - : Pops an existing GPU error scope from the error scope stack and returns a {{jsxref("Promise")}} that resolves to an object ({{domxref("GPUInternalError")}}, {{domxref("GPUOutOfMemoryError")}}, or {{domxref("GPUValidationError")}}) describing the first error captured in the scope, or `null` if no error occurred.

- {{domxref("GPUDevice.pushErrorScope", "pushErrorScope()")}} {{Experimental_Inline}}
  - : Pushes a new GPU error scope onto the device's error scope stack, allowing you to capture errors of a particular type.

## Events

- {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} {{Experimental_Inline}}
  - : Fired when an error is thrown that has not been observed by a GPU error scope, to provide a way to report unexpected errors. Known error cases should be handled using {{domxref("GPUDevice.pushErrorScope", "pushErrorScope()")}} and {{domxref("GPUDevice.popErrorScope", "popErrorScope()")}}.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const device = await adapter.requestDevice();

  const shaderModule = device.createShaderModule({
    code: shaders,
  });

  //...
}
```

See the individual member pages listed above and the following demo sites for a lot more examples of `GPUDevice` usage:

- [Basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/)
- [Basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/)
- [WebGPU samples](https://webgpu.github.io/webgpu-samples/)

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/createcommandencoder/index.md
---
title: "GPUDevice: createCommandEncoder() method"
short-title: createCommandEncoder()
slug: Web/API/GPUDevice/createCommandEncoder
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createCommandEncoder
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createCommandEncoder()`** method of the
{{domxref("GPUDevice")}} interface creates a {{domxref("GPUCommandEncoder")}}, used to encode commands to be issued to the GPU.

## Syntax

```js-nolint
createCommandEncoder()
createCommandEncoder(descriptor)
```

### Parameters

- `descriptor` {{optional_inline}}
  - : An object containing the following properties:
    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

### Return value

A {{domxref("GPUCommandEncoder")}} object instance.

## Examples

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/), several commands are recorded via a {{domxref("GPUCommandEncoder")}} created via `createCommandEncoder()`:

```js
// ...

// Create GPUCommandEncoder
const commandEncoder = device.createCommandEncoder();

// Create GPURenderPassDescriptor to tell WebGPU which texture to draw into, then initiate render pass
const renderPassDescriptor = {
  colorAttachments: [
    {
      clearValue: clearColor,
      loadOp: "clear",
      storeOp: "store",
      view: context.getCurrentTexture().createView(),
    },
  ],
};

const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// Draw a triangle
passEncoder.setPipeline(renderPipeline);
passEncoder.setVertexBuffer(0, vertexBuffer);
passEncoder.draw(3);

// End the render pass
passEncoder.end();

// ...
```

The commands encoded by the {{domxref("GPUCommandEncoder")}} are recoded into a {{domxref("GPUCommandBuffer")}} using the {{domxref("GPUCommandEncoder.finish()")}} method. The command buffer is then passed into the queue via a {{domxref("GPUQueue.submit", "submit()")}} call, ready to be processed by the GPU.

```js
device.queue.submit([commandEncoder.finish()]);
```

> **Note:** Study the [WebGPU samples](https://webgpu.github.io/webgpu-samples/) to find more command encoding examples.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/queue/index.md
---
title: "GPUDevice: queue property"
short-title: queue
slug: Web/API/GPUDevice/queue
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUDevice.queue
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`queue`** read-only property of the
{{domxref("GPUDevice")}} interface returns the primary {{domxref("GPUQueue")}} for the device.

## Value

A {{domxref("GPUQueue")}} object instance.

## Examples

Basic {{domxref("GPUQueue")}} access:

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  // Create a GPUDevice
  const device = await adapter.requestDevice();

  // ...

  // Common queue use ‚Äî end current frame by passing array of
  // command buffers to queue for execution
  device.queue.submit([commandEncoder.finish()]);

  // ...
}
```

> **Note:** For more queue examples, see the {{domxref("GPUQueue")}} reference pages.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/pusherrorscope/index.md
---
title: "GPUDevice: pushErrorScope() method"
short-title: pushErrorScope()
slug: Web/API/GPUDevice/pushErrorScope
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.pushErrorScope
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`pushErrorScope()`** method of the
{{domxref("GPUDevice")}} interface pushes a new GPU error scope onto the device's error scope stack, allowing you to capture errors of a particular type.

Once you are done capturing errors, you can end capture by invoking {{domxref("GPUDevice.popErrorScope()")}}. This pops the scope from the stack and returns a {{jsxref("Promise")}} that resolves to an object describing the first error captured in the scope, or `null` if no errors were captured.

## Syntax

```js-nolint
pushErrorScope(filter)
```

### Parameters

- `filter`
  - : An enumerated value that specifies what type of error will be caught in this particular error scope. Possible values are:
    - `"internal"`
      - : The error scope will catch a {{domxref("GPUInternalError")}}.
    - `"out-of-memory"`
      - : The error scope will catch a {{domxref("GPUOutOfMemoryError")}}.
    - `"validation"`
      - : The error scope will catch a {{domxref("GPUValidationError")}}.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

The following example uses an error scope to capture a suspected validation error, logging it to the console.

```js
device.pushErrorScope("validation");

let sampler = device.createSampler({
  maxAnisotropy: 0, // Invalid, maxAnisotropy must be at least 1.
});

device.popErrorScope().then((error) => {
  if (error) {
    sampler = null;
    console.error(`An error occurred while creating sampler: ${error.message}`);
  }
});
```

See [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling) for a lot more examples and information.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/createcomputepipelineasync/index.md
---
title: "GPUDevice: createComputePipelineAsync() method"
short-title: createComputePipelineAsync()
slug: Web/API/GPUDevice/createComputePipelineAsync
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createComputePipelineAsync
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createComputePipelineAsync()`** method of the
{{domxref("GPUDevice")}} interface returns a {{jsxref("Promise")}} that fulfills with a {{domxref("GPUComputePipeline")}}, which can control the compute shader stage and be used in a {{domxref("GPUComputePassEncoder")}}, once the pipeline can be used without any stalling.

> **Note:** It is generally preferable to use this method over {{domxref("GPUDevice.createComputePipeline()")}} whenever possible, as it prevents blocking of GPU operation execution on pipeline compilation.

## Syntax

```js-nolint
createComputePipeline(descriptor)
```

### Parameters

- `descriptor`
  - : See the descriptor definition for the [`GPUDevice.createComputePipeline()`](/en-US/docs/Web/API/GPUDevice/createComputePipeline#syntax) method.

### Return value

A {{jsxref("Promise")}} that fulfills with a {{domxref("GPUComputePipeline")}} object instance when the created pipeline is ready to be used without additional delay.

### Validation

If pipeline creation fails and the resulting pipeline becomes invalid as a result, the returned promise rejects with a {{domxref("GPUPipelineError")}}:

- If this is due to an internal error, the {{domxref("GPUPipelineError")}} will have a `reason` of `"internal"`.
- If this is due to a validation error, the {{domxref("GPUPipelineError")}} will have a `reason` of `"validation"`.

A validation error can occur if any of the following are false:

- The workgroup storage size used by the `module` referenced inside the `compute` property is less than or equal to the {{domxref("GPUDevice")}}'s `maxComputeWorkgroupStorageSize` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- The `module` uses a number of compute invocations per workgroup less than or equal to the {{domxref("GPUDevice")}}'s `maxComputeInvocationsPerWorkgroup` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- The `module`'s workgroup size is less than or equal to the {{domxref("GPUDevice")}}'s corresponding `maxComputeWorkgroupSizeX`, `maxComputeWorkgroupSizeY`, or `maxComputeWorkgroupSizeZ` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.

## Examples

> **Note:** The [WebGPU samples](https://webgpu.github.io/webgpu-samples/) feature many more examples.

### Basic example

The following example shows a process of:

- Creating a bind group layout with {{domxref("GPUDevice.createBindGroupLayout()")}}.
- Feeding the `bindGroupLayout` into {{domxref("GPUDevice.createPipelineLayout()")}} to create a {{domxref("GPUPipelineLayout")}}.
- Using that value immediately in a `createComputePipelineAsync()` call to create a {{domxref("GPUComputePipeline")}}.

```js
async function init() {
  // ...

  const bindGroupLayout = device.createBindGroupLayout({
    entries: [
      {
        binding: 0,
        visibility: GPUShaderStage.COMPUTE,
        buffer: {
          type: "storage",
        },
      },
    ],
  });

  const computePipeline = await device.createComputePipelineAsync({
    layout: device.createPipelineLayout({
      bindGroupLayouts: [bindGroupLayout],
    }),
    compute: {
      module: shaderModule,
      entryPoint: "main",
    },
  });

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/createtexture/index.md
---
title: "GPUDevice: createTexture() method"
short-title: createTexture()
slug: Web/API/GPUDevice/createTexture
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createTexture
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createTexture()`** method of the
{{domxref("GPUDevice")}} interface creates a {{domxref("GPUTexture")}} in which to store 1D, 2D, or 3D arrays of data, such as images, to use in GPU rendering operations.

## Syntax

```js-nolint
createTexture(descriptor)
```

### Parameters

- `descriptor`

  - : An object containing the following properties:

    - `dimension` {{optional_inline}}

      - : An enumerated value indicating the dimension level of the texture. Possible values are:

        - `"1d"`: The texture is one-dimensional.
        - `"2d"`: The texture is two-dimensional or an array of two-dimensional layers.
        - `"3d"`: The texture is three-dimensional.

        `dimension` defaults to `"2d"` if the value is omitted.

    - `format`
      - : An enumerated value specifying the format of the texture. See the [Texture formats](https://gpuweb.github.io/gpuweb/#enumdef-gputextureformat) section of the specification for all the possible values.
    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
    - `mipLevelCount` {{optional_inline}}
      - : A number specifying the number of mip levels the texture will contain. If omitted, this defaults to 1.
    - `sampleCount` {{optional_inline}}
      - : A number specifying the texture's sample count. To be valid, the value must be 1 or 4. If omitted, this defaults to 1. A value higher than 1 indicates a multi-sampled texture.
    - `size`

      - : An object or array specifying the width, height, and depth/array layer count of the texture. The width value must always be specified, while the height and depth/array layer count values are optional and will default to 1 if omitted.

        What follows is a sample `size` array:

        ```js
        size: [16, 16, 2];
        ```

        The object equivalent would look like this:

        ```js
        size: {
          width: 16,
          height: 16,
          depthOrArrayLayers: 2
        }
        ```

    - `usage`

      - : The {{glossary("Bitwise_flags", "bitwise flags")}} representing the allowed usages for the `GPUTexture`. The possible values are in the [`GPUTexture.usage` value table](/en-US/docs/Web/API/GPUTexture/usage#value).

        Note that multiple possible usages can be specified by separating values with pipe symbols, for example:

        ```js
        usage: GPUTextureUsage.COPY_DST | GPUTextureUsage.RENDER_ATTACHMENT;
        ```

    - `viewFormats` {{optional_inline}}
      - : An array of enumerated values specifying other [texture formats](https://gpuweb.github.io/gpuweb/#enumdef-gputextureformat) permitted when calling {{domxref("GPUTexture.createView()")}} on this texture, in addition to the texture format specified in its `format` value.

### Return value

A {{domxref("GPUTexture")}} object instance.

### Validation

The following criteria must be met when calling **`createTexture()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPUTexture")}} object is returned:

- A valid `usage` is specified.
- The values specified in `size` (width, height, or depth/array layer count) are greater than 0.
- `mipLevelCount` is greater than 0.
- `sampleCount` is equal to 1 or 4.
- If `dimension` is set to `"1d"`:
  - The `size` width value is less than or equal to the {{domxref("GPUDevice")}}'s `maxTextureDimension1D` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
  - The `size` height and depth/array layer count values are equal to 1.
  - The `sampleCount` is equal to 1.
  - The `format` is not equal to a [compressed format](https://gpuweb.github.io/gpuweb/#compressed-format) or [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#depth-or-stencil-format).
- If `dimension` is set to `"2d"`:
  - The `size` width and height values are less than or equal to the {{domxref("GPUDevice")}}'s `maxTextureDimension2D` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
  - The `size` depth/array layer count value is less than or equal to the {{domxref("GPUDevice")}}'s `maxTextureArrayLayers` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- If `dimension` is set to `"3d"`:
  - The `size` width, and height, and depth/array layer count values are less than or equal to the {{domxref("GPUDevice")}}'s `maxTextureDimension3D` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
  - The `sampleCount` value is equal to 1.
  - The `format` is not equal to a [compressed format](https://gpuweb.github.io/gpuweb/#compressed-format) or [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#depth-or-stencil-format).
- The `size` width value is a multiple of the [texel block width](https://gpuweb.github.io/gpuweb/#texel-block-width).
- The `size` height value is a multiple of the [texel block height](https://gpuweb.github.io/gpuweb/#texel-block-height).
- If `sampleCount` is greater than 1:
  - `mipLevelCount` is equal to 1.
  - The `size` depth/array layer count value is equal to 1.
  - `usage` includes the `GPUTextureUsage.RENDER_ATTACHMENT` flag.
  - `usage` does not include the `GPUTextureUsage.STORAGE_BINDING` flag.
  - The specified format supports multi-sampling.
- The `mipLevelCount` value is less than or equal to the [maximum miplevel count](https://gpuweb.github.io/gpuweb/#abstract-opdef-maximum-miplevel-count).
- The formats specified in `format` and `viewFormats` are [compatible](https://gpuweb.github.io/gpuweb/#texture-view-format-compatible) with one another.
- If `usage` includes the `GPUTextureUsage.RENDER_ATTACHMENT` flag:
  - `format` is a renderable format (meaning a color renderable format, or a [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#depth-or-stencil-format)).
  - `dimension` is set to `"2d"`.
- If `usage` includes the `GPUTextureUsage.STORAGE_BINDING` flag:
  - The specified `format` includes the `STORAGE_BINDING` capability (see the [Plain color formats](https://gpuweb.github.io/gpuweb/#plain-color-formats) table for reference).

## Examples

In the WebGPU samples [Textured Cube sample](https://webgpu.github.io/webgpu-samples/samples/texturedCube), a texture to use on the faces of a cube is created by:

- Loading the image into an {{domxref("HTMLImageElement")}} and creating an image bitmap using {{domxref("createImageBitmap()")}}.
- Creating a new texture using `createTexture()`.
- Copying the image bitmap into the texture using {{domxref("GPUQueue.copyExternalImageToTexture()")}}.

```js
//...

let cubeTexture: GPUTexture; // Sample is written in TypeScript

{
  const img = document.createElement("img");
  img.src = new URL(
    "../../../assets/img/Di-3d.png",
    import.meta.url
  ).toString();
  await img.decode();
  const imageBitmap = await createImageBitmap(img);

  cubeTexture = device.createTexture({
    size: [imageBitmap.width, imageBitmap.height, 1],
    format: "rgba8unorm",
    usage:
      GPUTextureUsage.TEXTURE_BINDING |
      GPUTextureUsage.COPY_DST |
      GPUTextureUsage.RENDER_ATTACHMENT,
  });
  device.queue.copyExternalImageToTexture(
    { source: imageBitmap },
    { texture: cubeTexture },
    [imageBitmap.width, imageBitmap.height]
  );
}

//...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/createshadermodule/index.md
---
title: "GPUDevice: createShaderModule() method"
short-title: createShaderModule()
slug: Web/API/GPUDevice/createShaderModule
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createShaderModule
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createShaderModule()`** method of the
{{domxref("GPUDevice")}} interface creates a {{domxref("GPUShaderModule")}} from a string of [WGSL](https://gpuweb.github.io/gpuweb/wgsl/) source code.

## Syntax

```js-nolint
createShaderModule(descriptor)
```

### Parameters

- `descriptor`

  - : An object containing the following properties:

    - `code`
      - : A string representing the WGSL source code for the shader module.
    - `hints` {{optional_inline}}

      - : A sequence of record types, with the structure `("string", compilationHint)`. These behave like [ordered maps](/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map). In each case, the `"string"` is a key used to identify or select the record, and the `compilationHint` is either a {{domxref("GPUPipelineLayout")}} object instance or an enumerated value of `"auto"`.

        The point of `hints` is to provide information about the pipeline layout as early as possible to improve performance. The idea is to maximize the amount of compilation that can be done once by `createShaderModule()`, rather than multiple times in multiple calls to {{domxref("GPUDevice.createComputePipeline()")}} and {{domxref("GPUDevice.createRenderPipeline()")}}.

        > **Note:** Different implementations may handle `hints` in different ways, including possibly ignoring them entirely. Providing hints does not guarantee improved shader compilation performance on all browsers/systems.

    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
    - `sourceMap` {{optional_inline}}

      - : A source map definition to provide developer tool integration such as source-language debugging. WGSL names (identifiers) in source maps should follow the rules defined in [WGSL identifier comparison](https://gpuweb.github.io/gpuweb/wgsl/#identifier-comparison). If defined, the source map may be interpreted as a [source-map-v3 format](https://sourcemaps.info/spec.html).

        > **Note:** Different implementations may handle `sourceMap`s in different ways, including possibly ignoring them entirely.

### Return value

A {{domxref("GPUShaderModule")}} object instance.

## Examples

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/), our shader module is created using the following code:

```js
const shaders = `
struct VertexOut {
  @builtin(position) position : vec4f,
  @location(0) color : vec4f
}

@vertex
fn vertex_main(@location(0) position: vec4f,
               @location(1) color: vec4f) -> VertexOut
{
  var output : VertexOut;
  output.position = position;
  output.color = color;
  return output;
}

@fragment
fn fragment_main(fragData: VertexOut) -> @location(0) vec4f
{
  return fragData.color;
}
`;

async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  let device = await adapter.requestDevice();

  // ...
  // later on

  const shaderModule = device.createShaderModule({
    code: shaders,
  });

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- The [WebGPU Shading Language specification](https://gpuweb.github.io/gpuweb/wgsl/)
-e 

File: /files/en-us/web/api/gpudevice/createrenderbundleencoder/index.md
---
title: "GPUDevice: createRenderBundleEncoder() method"
short-title: createRenderBundleEncoder()
slug: Web/API/GPUDevice/createRenderBundleEncoder
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createRenderBundleEncoder
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createRenderBundleEncoder()`** method of the
{{domxref("GPUDevice")}} interface creates a {{domxref("GPURenderBundleEncoder")}} that can be used to pre-record bundles of commands. These can be reused in {{domxref("GPURenderPassEncoder")}}s via the {{domxref("GPURenderPassEncoder.executeBundles", "executeBundles()")}} method, as many times as required.

## Syntax

```js-nolint
createRenderBundleEncoder(descriptor)
```

### Parameters

- `descriptor`
  - : An object containing the following properties:
    - `colorFormats`
      - : An array of enumerated values specifying the expected color formats for render targets. For possible values, see the [`GPUTextureFormat` definition](https://gpuweb.github.io/gpuweb/#depth-or-stencil-format) in the spec.
    - `depthReadOnly` {{optional_inline}}
      - : A boolean. If `true`, specifies that executing any {{domxref("GPURenderBundle")}} created by the {{domxref("GPURenderBundleEncoder")}} will not modify the depth component of the `depthStencilFormat` when executed. If omitted, `depthReadOnly` will default to `false`.
    - `depthStencilFormat` {{optional_inline}}
      - : An enumerated value that specifies the expected depth-or-stencil format for render targets. For possible values, see the [Depth-stencil formats](https://gpuweb.github.io/gpuweb/#depth-or-stencil-format) section of the spec.
    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
    - `sampleCount` {{optional_inline}}
      - : A number representing the expected sample count for render targets.
    - `stencilReadOnly` {{optional_inline}}
      - : A boolean. If `true`, specifies that executing any {{domxref("GPURenderBundle")}} created by the {{domxref("GPURenderBundleEncoder")}} will not modify the stencil component of the `depthStencilFormat` when executed. If omitted, `stencilReadOnly` will default to `false`.

### Return value

A {{domxref("GPURenderBundleEncoder")}} object instance.

## Examples

In the WebGPU Samples [Animometer example](https://webgpu.github.io/webgpu-samples/samples/animometer), numerous similar operations are done on many different objects simultaneously. A bundle of commands is encoded using the following function:

```js
function recordRenderPass(
  passEncoder: GPURenderBundleEncoder | GPURenderPassEncoder
) {
  if (settings.dynamicOffsets) {
    passEncoder.setPipeline(dynamicPipeline);
  } else {
    passEncoder.setPipeline(pipeline);
  }
  passEncoder.setVertexBuffer(0, vertexBuffer);
  passEncoder.setBindGroup(0, timeBindGroup);
  const dynamicOffsets = [0];
  for (let i = 0; i < numTriangles; ++i) {
    if (settings.dynamicOffsets) {
      dynamicOffsets[0] = i * alignedUniformBytes;
      passEncoder.setBindGroup(1, dynamicBindGroup, dynamicOffsets);
    } else {
      passEncoder.setBindGroup(1, bindGroups[i]);
    }
    passEncoder.draw(3, 1, 0, 0);
  }
}
```

Later on, a {{domxref("GPURenderBundleEncoder")}} is created using `createRenderBundleEncoder()`, the function is invoked, and the command bundle is recorded into a {{domxref("GPURenderBundle")}} using {{domxref("GPURenderBundleEncoder.finish()")}}:

```js
const renderBundleEncoder = device.createRenderBundleEncoder({
  colorFormats: [presentationFormat],
});
recordRenderPass(renderBundleEncoder);
const renderBundle = renderBundleEncoder.finish();
```

{{domxref("GPURenderPassEncoder.executeBundles()")}} is then used to reuse the work across multiple render passes to improve performance. Study the example code listing for the full context.

```js
// ...

return function doDraw(timestamp) {
  if (startTime === undefined) {
    startTime = timestamp;
  }
  uniformTime[0] = (timestamp - startTime) / 1000;
  device.queue.writeBuffer(uniformBuffer, timeOffset, uniformTime.buffer);

  renderPassDescriptor.colorAttachments[0].view = context
    .getCurrentTexture()
    .createView();

  const commandEncoder = device.createCommandEncoder();
  const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

  if (settings.renderBundles) {
    passEncoder.executeBundles([renderBundle]);
  } else {
    recordRenderPass(passEncoder);
  }

  passEncoder.end();
  device.queue.submit([commandEncoder.finish()]);
};

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/poperrorscope/index.md
---
title: "GPUDevice: popErrorScope() method"
short-title: popErrorScope()
slug: Web/API/GPUDevice/popErrorScope
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.popErrorScope
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`popErrorScope()`** method of the
{{domxref("GPUDevice")}} interface pops an existing GPU error scope from the error scope stack (originally pushed using {{domxref("GPUDevice.pushErrorScope()")}}) and returns a {{jsxref("Promise")}} that resolves to an object describing the first error captured in the scope, or `null` if no error occurred.

## Syntax

```js-nolint
popErrorScope()
```

### Parameters

None.

### Return value

a {{jsxref("Promise")}} that resolves to an object describing the first error captured in the scope. This can be of type:

- {{domxref("GPUInternalError")}}
- {{domxref("GPUOutOfMemoryError")}}
- {{domxref("GPUValidationError")}}

If no error occurred, it resolves to `null`.

## Examples

The following example uses an error scope to capture a suspected validation error, logging it to the console.

```js
device.pushErrorScope("validation");

let sampler = device.createSampler({
  maxAnisotropy: 0, // Invalid, maxAnisotropy must be at least 1.
});

device.popErrorScope().then((error) => {
  if (error) {
    sampler = null;
    console.error(`An error occurred while creating sampler: ${error.message}`);
  }
});
```

See [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling) for a lot more examples and information.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/createcomputepipeline/index.md
---
title: "GPUDevice: createComputePipeline() method"
short-title: createComputePipeline()
slug: Web/API/GPUDevice/createComputePipeline
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createComputePipeline
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createComputePipeline()`** method of the
{{domxref("GPUDevice")}} interface creates a {{domxref("GPUComputePipeline")}} that can control the compute shader stage and be used in a {{domxref("GPUComputePassEncoder")}}.

## Syntax

```js-nolint
createComputePipeline(descriptor)
```

### Parameters

- `descriptor`

  - : An object containing the following properties:

    - `compute`

      - : An object describing the compute shader entry point of the pipeline. This object can contain the following properties:

        - `constants` {{optional_inline}}

          - : A sequence of record types, with the structure `(id, value)`, representing override values for [WGSL constants that can be overridden in the pipeline](https://gpuweb.github.io/gpuweb/#typedefdef-gpupipelineconstantvalue). These behave like [ordered maps](/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map). In each case, the `id` is a key used to identify or select the record, and the `constant` is an enumerated value representing a WGSL.

            Depending on which constant you want to override, the `id` may take the form of the numeric ID of the constant, if one is specified, or otherwise the constant's identifier name.

            A code snippet providing override values for several overridable constants might look like this:

            ```js
            {
              // ...
              constants: {
                0: false,
                1200: 3.0,
                1300: 2.0,
                width: 20,
                depth: -1,
                height: 15,
              }
            }
            ```

        - `entryPoint`
          - : The name of the function in the `module` that this stage will use to perform its work. The corresponding shader function must have the `@compute` attribute to be identified as this entry point. See [Entry Point Declaration](https://gpuweb.github.io/gpuweb/wgsl/#entry-point-decl) for more information.
        - `module`
          - : A {{domxref("GPUShaderModule")}} object containing the [WGSL](https://gpuweb.github.io/gpuweb/wgsl/) code that this programmable stage will execute.

    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
    - `layout`
      - : Defines the layout (structure, purpose, and type) of all the GPU resources (buffers, textures, etc.) used during the execution of the pipeline. Possible values are:
        - A {{domxref("GPUPipelineLayout")}} object, created using {{domxref("GPUDevice.createPipelineLayout()")}}, which allows the GPU to figure out how to run the pipeline most efficiently ahead of time.
        - A string of `"auto"`, which causes the pipeline to generate an implicit bind group layout based on any bindings defined in the shader code. If `"auto"` is used, the generated bind group layouts may only be used with the current pipeline.

### Return value

A {{domxref("GPUComputePipeline")}} object instance.

### Validation

The following criteria must be met when calling **`createComputePipeline()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPUComputePipeline")}} object is returned:

- The workgroup storage size used by the `module` referenced inside the `compute` property is less than or equal to the {{domxref("GPUDevice")}}'s `maxComputeWorkgroupStorageSize` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- The `module` uses a number of compute invocations per workgroup less than or equal to the {{domxref("GPUDevice")}}'s `maxComputeInvocationsPerWorkgroup` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- The `module`'s workgroup size is less than or equal to the {{domxref("GPUDevice")}}'s corresponding `maxComputeWorkgroupSizeX`, `maxComputeWorkgroupSizeY`, or `maxComputeWorkgroupSizeZ` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.

## Examples

> **Note:** The [WebGPU samples](https://webgpu.github.io/webgpu-samples/) feature many more examples.

### Basic example

Our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/) shows a process of:

- Creating a bind group layout with {{domxref("GPUDevice.createBindGroupLayout()")}}.
- Feeding the `bindGroupLayout` into {{domxref("GPUDevice.createPipelineLayout()")}} to create a {{domxref("GPUPipelineLayout")}}.
- Using that value immediately in a `createComputePipeline()` call to create a {{domxref("GPUComputePipeline")}}.

```js
// ...

const bindGroupLayout = device.createBindGroupLayout({
  entries: [
    {
      binding: 0,
      visibility: GPUShaderStage.COMPUTE,
      buffer: {
        type: "storage",
      },
    },
  ],
});

const computePipeline = device.createComputePipeline({
  layout: device.createPipelineLayout({
    bindGroupLayouts: [bindGroupLayout],
  }),
  compute: {
    module: shaderModule,
    entryPoint: "main",
  },
});

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpudevice/createsampler/index.md
---
title: "GPUDevice: createSampler() method"
short-title: createSampler()
slug: Web/API/GPUDevice/createSampler
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUDevice.createSampler
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createSampler()`** method of the
{{domxref("GPUDevice")}} interface creates a {{domxref("GPUSampler")}}, which controls how shaders transform and filter texture resource data.

## Syntax

```js-nolint
createSampler()
createSampler(descriptor)
```

### Parameters

- `descriptor` {{optional_inline}}

  - : An object containing the following properties:

    - `addressModeU` {{optional_inline}}

      - : An enumerated value specifying the behavior of the sampler when the sample footprint width extends beyond the width of the texture. Possible values are:

        - `"clamp-to-edge"`: The texture coordinates are clamped between 0.0 and 1.0, inclusive.
        - `"repeat"`: The texture coordinates wrap to the other side of the texture.
        - `"mirror-repeat"`: The texture coordinates wrap to the other side of the texture, but the texture is flipped when the integer part of the coordinate is odd.

        If omitted, `addressModeU` defaults to `"clamp-to-edge"`.

    - `addressModeV` {{optional_inline}}
      - : An enumerated value specifying the behavior of the sampler when the sample footprint height extends beyond the height of the texture. Possible and default values are the same as for `addressModeU`.
    - `addressModeW` {{optional_inline}}

      - : An enumerated value specifying the behavior of the sampler when the sample footprint depth extends beyond the depth of the texture. Possible and default values are the same as for `addressModeU`.

    - `compare` {{optional_inline}}

      - : If specified, the sampler will be a comparison sampler of the specified type. Possible (enumerated) values are:

        - `"never"`: Comparison tests never pass.
        - `"less"`: A provided value passes the comparison test if it is less than the sampled value.
        - `"equal"`: A provided value passes the comparison test if it is equal to the sampled value.
        - `"less-equal"`: A provided value passes the comparison test if it is less than or equal to the sampled value.
        - `"greater"`: A provided value passes the comparison test if it is greater than the sampled value.
        - `"not-equal"`: A provided value passes the comparison test if it is not equal to the sampled value.
        - `"greater-equal"`: A provided value passes the comparison test if it is greater than or equal to the sampled value.
        - `"always"`: Comparison tests always pass.

        Comparison samplers may use filtering, but the sampling results will be implementation-dependent and may differ from the normal filtering rules.

    - `label` {{optional_inline}}

      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

    - `lodMinClamp` {{optional_inline}}
      - : A number specifying the minimum level of detail used internally when sampling a texture. If omitted, `lodMinClamp` defaults to 0.
    - `lodMaxClamp` {{optional_inline}}

      - : A number specifying the maximum level of detail used internally when sampling a texture. If omitted, `lodMaxClamp` defaults to 32.

    - `maxAnisotropy` {{optional_inline}}

      - : Specifies the maximum anisotropy value clamp used by the sampler. If omitted, `maxAnisotropy` defaults to 1.

        Most implementations support `maxAnisotropy` values in a range between 1 and 16, inclusive. The value used will be clamped to the maximum value that the underlying platform supports.

    - `magFilter` {{optional_inline}}

      - : An enumerated value specifying the sampling behavior when the sample footprint is smaller than or equal to one texel. Possible values are:

        - `"nearest"`: Return the value of the texel nearest to the texture coordinates.
        - `"linear"`: Select two texels in each dimension and return a linear interpolation between their values.

        If omitted, `magFilter` defaults to `"nearest"`.

    - `minFilter` {{optional_inline}}
      - : An enumerated value specifying the sampling behavior when the sample footprint is larger than one texel. Possible and default values are the same as for `magFilter`.
    - `mipmapFilter` {{optional_inline}}
      - : An enumerated value specifying the behavior when sampling between mipmap levels. Possible and default values are the same as for `magFilter`.

### Return value

A {{domxref("GPUSampler")}} object instance.

### Validation

The following criteria must be met when calling **`createSampler()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPUSampler")}} object is returned:

- `lodMinClamp` is equal to or more than 0.
- `lodMaxClamp` is equal to or more than `lodMinClamp`.
- `maxAnisotropy` is equal to or more than 1.
- If `maxAnisotropy` is more than 1, `magFilter`, `minFilter`, and `mipmapFilter` are `"linear"`.

## Examples

The following snippet creates a `GPUSampler` that does trilinear filtering and repeats texture coordinates:

```js
// ...

const sampler = device.createSampler({
  addressModeU: "repeat",
  addressModeV: "repeat",
  magFilter: "linear",
  minFilter: "linear",
  mipmapFilter: "linear",
});
```

The WebGPU samples [Shadow Mapping sample](https://webgpu.github.io/webgpu-samples/samples/shadowMapping) uses comparison samplers to sample from a depth texture to render shadows.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucomputepassencoder/setpipeline/index.md
---
title: "GPUComputePassEncoder: setPipeline() method"
short-title: setPipeline()
slug: Web/API/GPUComputePassEncoder/setPipeline
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUComputePassEncoder.setPipeline
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setPipeline()`** method of the
{{domxref("GPUComputePassEncoder")}} interface sets the {{domxref("GPUComputePipeline")}} to use for this compute pass.

## Syntax

```js-nolint
setPipeline(pipeline)
```

### Parameters

- `pipeline`
  - : The {{domxref("GPUComputePipeline")}} to use for this compute pass.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

In our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/), several commands are recorded via a {{domxref("GPUCommandEncoder")}}. Most of these commands originate from the {{domxref("GPUComputePassEncoder")}} created via `beginComputePass()`. The `setPipeline()` call is used as appropriate to set the pipeline to use for this pass.

```js
const BUFFER_SIZE = 1000;

// ...

// Create GPUCommandEncoder to encode commands to issue to the GPU
const commandEncoder = device.createCommandEncoder();

// Initiate render pass
const passEncoder = commandEncoder.beginComputePass();

// Issue commands
passEncoder.setPipeline(computePipeline);
passEncoder.setBindGroup(0, bindGroup);
passEncoder.dispatchWorkgroups(Math.ceil(BUFFER_SIZE / 64));

// End the render pass
passEncoder.end();

// Copy output buffer to staging buffer
commandEncoder.copyBufferToBuffer(
  output,
  0, // Source offset
  stagingBuffer,
  0, // Destination offset
  BUFFER_SIZE,
);

// End frame by passing array of command buffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucomputepassencoder/setbindgroup/index.md
---
title: "GPUComputePassEncoder: setBindGroup() method"
short-title: setBindGroup()
slug: Web/API/GPUComputePassEncoder/setBindGroup
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUComputePassEncoder.setBindGroup
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setBindGroup()`** method of the
{{domxref("GPUComputePassEncoder")}} interface sets the {{domxref("GPUBindGroup")}} to use for subsequent compute commands, for a given index.

## Syntax

```js-nolint
setBindGroup(index, bindGroup)
setBindGroup(index, bindGroup, dynamicOffsets)
setBindGroup(index, bindGroup, dynamicOffsets, dynamicOffsetsStart,
             dynamicOffsetsLength)
```

### Parameters

- `index`
  - : The index to set the bind group at. This matches the `n` index value of the corresponding [`@group(n)`](https://gpuweb.github.io/gpuweb/wgsl/#attribute-group) attribute in the shader code ({{domxref("GPUShaderModule")}}) used in the related pipeline.
- `bindGroup`
  - : The {{domxref("GPUBindGroup")}} to use for subsequent compute commands.
- `dynamicOffsets` {{optional_inline}}
  - : A value specifying the offset, in bytes, for each entry in `bindGroup` with `hasDynamicOffset: true` set (i.e. in the descriptor of the {{domxref("GPUDevice.createBindGroupLayout()")}} call that created the {{domxref("GPUBindGroupLayout")}} object that the `bindGroup` is based on). This value can be:
    - An array of numbers specifying the different offsets.
    - A {{jsxref("Uint32Array")}} containing numbers specifying the offsets.

If a {{jsxref("Uint32Array")}} value is specified for `dynamicOffsets`, both of the following parameters are also required:

- `dynamicOffsetsStart`
  - : A number specifying the offset, in array elements, into `dynamicOffsetsData`, where the dynamic offset data begins.
- `dynamicOffsetsLength`
  - : A number specifying the number of dynamic offset values to be read from in `dynamicOffsetsData`.

### Return value

None ({{jsxref("Undefined")}}).

### Exceptions

For `setBindGroup()` calls that use a {{jsxref("Uint32Array")}} value for `dynamicOffsets`, the call will throw with a `RangeError` {{domxref("DOMException")}} if:

- `dynamicOffsetsStart` is less than 0.
- `dynamicOffsetsStart` + `dynamicOffsetsLength` is greater than `dynamicOffsets.length`.

### Validation

The following criteria must be met when calling **`dispatchWorkgroups()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUComputePassEncoder")}} becomes invalid:

- `index` is less than or equal to the {{domxref("GPUDevice")}}'s `maxBindGroups` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- `dynamicOffsets.length` is the same as the number of entries in `bindGroup` with `hasDynamicOffset: true` set.
- For `bindGroup` entries where the bound `buffer`'s `type` is `"uniform"` (see {{domxref("GPUDevice.createBindGroupLayout()")}}), each number in `dynamicOffsets` is a multiple of the {{domxref("GPUDevice")}}'s `minUniformBufferOffsetAlignment` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- For `bindGroup` entries where the bound `buffer`'s `type` is `"storage"` or `"read-only-storage"` (see {{domxref("GPUDevice.createBindGroupLayout()")}}), each number in `dynamicOffsets` is a multiple of the {{domxref("GPUDevice")}}'s `minStorageBufferOffsetAlignment` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- For each `bindGroup` entry, the bound `buffer`'s `offset`, plus the corresponding layout entry's `minBindingSize`, plus the corresponding dynamic offset specified in `dynamicOffsets`, is less than or equal to the bound `buffer`'s `size`.

## Examples

In our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/), several commands are recorded via a {{domxref("GPUCommandEncoder")}}. Most of these commands originate from the {{domxref("GPUComputePassEncoder")}} created via `beginComputePass()`. The `setBindGroup()` call used here is the simplest form, just specifying index and bind group.

```js
const BUFFER_SIZE = 1000;

// ...

// Create GPUCommandEncoder to encode commands to issue to the GPU
const commandEncoder = device.createCommandEncoder();

// Initiate render pass
const passEncoder = commandEncoder.beginComputePass();

// Issue commands
passEncoder.setPipeline(computePipeline);
passEncoder.setBindGroup(0, bindGroup);
passEncoder.dispatchWorkgroups(Math.ceil(BUFFER_SIZE / 64));

// End the render pass
passEncoder.end();

// Copy output buffer to staging buffer
commandEncoder.copyBufferToBuffer(
  output,
  0, // Source offset
  stagingBuffer,
  0, // Destination offset
  BUFFER_SIZE,
);

// End frame by passing array of command buffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucomputepassencoder/label/index.md
---
title: "GPUComputePassEncoder: label property"
short-title: label
slug: Web/API/GPUComputePassEncoder/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUComputePassEncoder.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** read-only property of the
{{domxref("GPUComputePassEncoder")}} interface is a string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUCommandEncoder.beginComputePass()")}} call, or you can get and set it directly on the `GPUComputePassEncoder` object.

## Value

A string. If no label value has previously been set, getting the label returns an empty string.

## Examples

Setting and getting a label via `GPUComputePassEncoder.label`:

```js
const commandEncoder = device.createCommandEncoder();
const passEncoder = commandEncoder.beginComputePass();

passEncoder.label = "mycomputepassencoder";
console.log(passEncoder.label); // "mycomputepassencoder"
```

Setting a label via the originating {{domxref("GPUCommandEncoder.beginComputePass()")}} call, and then getting it via `GPUComputePassEncoder.label`:

```js
const commandEncoder = device.createCommandEncoder();
const passEncoder = commandEncoder.beginComputePass({
  label: "mycomputepassencoder",
});

console.log(passEncoder.label); // "mycomputepassencoder"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucomputepassencoder/end/index.md
---
title: "GPUComputePassEncoder: end() method"
short-title: end()
slug: Web/API/GPUComputePassEncoder/end
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUComputePassEncoder.end
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`end()`** method of the
{{domxref("GPUComputePassEncoder")}} interface completes recording of the current compute pass command sequence.

## Syntax

```js-nolint
end()
```

### Parameters

None.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`end()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUComputePassEncoder")}} becomes invalid:

- The {{domxref("GPUComputePassEncoder")}} is open (i.e. not already ended via an `end()` call).
- any {{domxref("GPUComputePassEncoder.pushDebugGroup", "pushDebugGroup()")}} calls made on this encoder have a corresponding {{domxref("GPUComputePassEncoder.popDebugGroup", "popDebugGroup()")}} call before `end()` is called.

## Examples

In our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/), several commands are recorded via a {{domxref("GPUCommandEncoder")}}. Most of these commands originate from the {{domxref("GPUComputePassEncoder")}} created via {{domxref("GPUCommandEncoder.beginComputePass()")}}.

```js
const BUFFER_SIZE = 1000;

// ...

// Create GPUCommandEncoder to encode commands to issue to the GPU
const commandEncoder = device.createCommandEncoder();

// Initiate render pass
const passEncoder = commandEncoder.beginComputePass();

// Issue commands
passEncoder.setPipeline(computePipeline);
passEncoder.setBindGroup(0, bindGroup);
passEncoder.dispatchWorkgroups(Math.ceil(BUFFER_SIZE / 64));

// End the render pass
passEncoder.end();

// Copy output buffer to staging buffer
commandEncoder.copyBufferToBuffer(
  output,
  0, // Source offset
  stagingBuffer,
  0, // Destination offset
  BUFFER_SIZE,
);

// End frame by passing array of command buffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucomputepassencoder/insertdebugmarker/index.md
---
title: "GPUComputePassEncoder: insertDebugMarker() method"
short-title: insertDebugMarker()
slug: Web/API/GPUComputePassEncoder/insertDebugMarker
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUComputePassEncoder.insertDebugMarker
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`insertDebugMarker()`** method of the
{{domxref("GPUComputePassEncoder")}} interface marks a specific point in a series of encoded compute pass commands with a label.

This could be used for telemetry, or may be utilized in {{domxref("GPUError")}} messages, browser dev tools, or other services in the future to help with debugging.

## Syntax

```js-nolint
insertDebugMarker(markerLabel)
```

### Parameters

- `markerLabel`
  - : A string representing the label to insert.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
// ...

passEncoder.insertDebugMarker("mymarker");

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucomputepassencoder/index.md
---
title: GPUComputePassEncoder
slug: Web/API/GPUComputePassEncoder
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUComputePassEncoder
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUComputePassEncoder`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} encodes commands related to controlling the compute shader stage, as issued by a {{domxref("GPUComputePipeline")}}. It forms part of the overall encoding activity of a {{domxref("GPUCommandEncoder")}}.

A compute pipeline contains a single compute stage in which a compute shader takes general data, processes it in parallel across a specified number of workgroups, then returns the result in one or more buffers.

A `GPUComputePassEncoder` object instance is created via the {{domxref("GPUCommandEncoder.beginComputePass()")}} property.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUComputePassEncoder.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Instance methods

- {{domxref("GPUComputePassEncoder.dispatchWorkgroups", "dispatchWorkgroups()")}} {{Experimental_Inline}}
  - : Dispatches a specific grid of workgroups to perform the work being done by the current {{domxref("GPUComputePipeline")}}.
- {{domxref("GPUComputePassEncoder.dispatchWorkgroupsIndirect", "dispatchWorkgroupsIndirect()")}} {{Experimental_Inline}}
  - : Dispatches a grid of workgroups, defined by the parameters of a {{domxref("GPUBuffer")}}, to perform the work being done by the current {{domxref("GPUComputePipeline")}}.
- {{domxref("GPUComputePassEncoder.end", "end()")}} {{Experimental_Inline}}
  - : Completes recording of the current compute pass command sequence.
- {{domxref("GPUComputePassEncoder.insertDebugMarker", "insertDebugMarker()")}} {{Experimental_Inline}}
  - : Marks a specific point in a series of encoded commands with a label.
- {{domxref("GPUComputePassEncoder.popDebugGroup", "popDebugGroup()")}} {{Experimental_Inline}}
  - : Ends a debug group, which is begun with a {{domxref("GPUComputePassEncoder.pushDebugGroup", "pushDebugGroup()")}} call.
- {{domxref("GPUComputePassEncoder.pushDebugGroup", "pushDebugGroup()")}} {{Experimental_Inline}}
  - : Begins a debug group, which is marked with a specified label, and will contain all subsequent encoded commands up until a {{domxref("GPUComputePassEncoder.popDebugGroup", "popDebugGroup()")}} method is invoked.
- {{domxref("GPUComputePassEncoder.setBindGroup", "setBindGroup()")}} {{Experimental_Inline}}
  - : Sets the {{domxref("GPUBindGroup")}} to use for subsequent compute commands, for a given index.
- {{domxref("GPUComputePassEncoder.setPipeline", "setPipeline()")}} {{Experimental_Inline}}
  - : Sets the {{domxref("GPUComputePipeline")}} to use for this compute pass.

## Examples

In our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/), several commands are recorded via a {{domxref("GPUCommandEncoder")}}. Most of these commands originate from the `GPUComputePassEncoder` created via {{domxref("GPUCommandEncoder.beginComputePass()")}}.

```js
// ...

// Create GPUCommandEncoder to encode commands to issue to the GPU
const commandEncoder = device.createCommandEncoder();

// Create GPUComputePassEncoder to initiate compute pass
const passEncoder = commandEncoder.beginComputePass();

// Issue commands
passEncoder.setPipeline(computePipeline);
passEncoder.setBindGroup(0, bindGroup);
passEncoder.dispatchWorkgroups(Math.ceil(BUFFER_SIZE / 64));

// End the compute pass
passEncoder.end();

// Copy output buffer to staging buffer
commandEncoder.copyBufferToBuffer(
  output,
  0, // Source offset
  stagingBuffer,
  0, // Destination offset
  BUFFER_SIZE,
);

// End frame by passing array of command buffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucomputepassencoder/popdebuggroup/index.md
---
title: "GPUComputePassEncoder: popDebugGroup() method"
short-title: popDebugGroup()
slug: Web/API/GPUComputePassEncoder/popDebugGroup
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUComputePassEncoder.popDebugGroup
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`popDebugGroup()`** method of the
{{domxref("GPUComputePassEncoder")}} interface ends a compute pass debug group, which is begun with a {{domxref("GPUComputePassEncoder.pushDebugGroup", "pushDebugGroup()")}} call.

This could be used for telemetry, or may be utilized in {{domxref("GPUError")}} messages, browser dev tools, or other services in the future to help with debugging.

## Syntax

```js-nolint
popDebugGroup()
```

### Parameters

None.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`popDebugGroup()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUComputePassEncoder")}} becomes invalid:

- The compute pass encoder's debug stack is not empty (i.e. at least one compute pass debug group was previously started with {{domxref("GPUComputePassEncoder.pushDebugGroup", "pushDebugGroup()")}}).

## Examples

```js
// ...

const passEncoder = commandEncoder.beginComputePass();

passEncoder.pushDebugGroup("mygroupmarker"); // Start labeled debug group

passEncoder.setPipeline(computePipeline);
passEncoder.setBindGroup(0, bindGroup);
passEncoder.dispatchWorkgroups(Math.ceil(BUFFER_SIZE / 64));

passEncoder.popDebugGroup();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucomputepassencoder/pushdebuggroup/index.md
---
title: "GPUComputePassEncoder: pushDebugGroup() method"
short-title: pushDebugGroup()
slug: Web/API/GPUComputePassEncoder/pushDebugGroup
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUComputePassEncoder.pushDebugGroup
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`pushDebugGroup()`** method of the
{{domxref("GPUComputePassEncoder")}} interface begins a compute pass debug group, which is marked with a specified label, and will contain all subsequent encoded commands up until a {{domxref("GPUComputePassEncoder.popDebugGroup", "popDebugGroup()")}} method is invoked.

This could be used for telemetry, or may be utilized in {{domxref("GPUError")}} messages, browser dev tools, or other services in the future to help with debugging.

## Syntax

```js-nolint
pushDebugGroup(groupLabel)
```

### Parameters

- `groupLabel`
  - : A string representing the label for the debug group.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
// ...

const passEncoder = commandEncoder.beginComputePass();

passEncoder.pushDebugGroup("mygroupmarker"); // Start labeled debug group

passEncoder.setPipeline(computePipeline);
passEncoder.setBindGroup(0, bindGroup);
passEncoder.dispatchWorkgroups(Math.ceil(BUFFER_SIZE / 64));

passEncoder.popDebugGroup();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucomputepassencoder/dispatchworkgroupsindirect/index.md
---
title: "GPUComputePassEncoder: dispatchWorkgroupsIndirect() method"
short-title: dispatchWorkgroupsIndirect()
slug: Web/API/GPUComputePassEncoder/dispatchWorkgroupsIndirect
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUComputePassEncoder.dispatchWorkgroupsIndirect
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`dispatchWorkgroupsIndirect()`** method of the
{{domxref("GPUComputePassEncoder")}} interface dispatches a grid of workgroups, defined by the parameters of a {{domxref("GPUBuffer")}}, to perform the work being done by the current {{domxref("GPUComputePipeline")}} (i.e. set via {{domxref("GPUComputePassEncoder.setPipeline()")}}).

## Syntax

```js-nolint
dispatchWorkgroupsIndirect(indirectBuffer, indirectOffset)
```

### Parameters

- `indirectBuffer`

  - : A {{domxref("GPUBuffer")}} containing the X, Y, and Z dimensions of the grid of workgroups to dispatch. The buffer must contain a tightly packed block of three 32-bit unsigned integer values representing the dimensions (12 bytes total), given in the same order as the arguments for {{domxref("GPUComputePassEncoder.dispatchWorkgroups()")}}. So for example:

    ```js
    const uint32 = new Uint32Array(3);
    uint32[0] = 25; // The X value
    uint32[1] = 1; // The Y value
    uint32[2] = 1; // The Z value

    // Write values into a GPUBuffer
    device.queue.writeBuffer(buffer, 0, uint32, 0, uint32.length);
    ```

- `indirectOffset`
  - : The offset, in bytes, into `indirectBuffer` where the dimension data begins.

> **Note:** The X, Y, and Z dimension values passed to {{domxref("GPUComputePassEncoder.dispatchWorkgroups()")}} and `dispatchWorkgroupsIndirect()` are the number of workgroups to dispatch for each dimension, not the number of shader invocations to perform across each dimension. This matches the behavior of modern native GPU APIs, but differs from the behavior of OpenCL. This means that if a {{domxref("GPUShaderModule")}} defines an entry point with `@workgroup_size(4, 4)`, and work is dispatched to it with the call `dispatchWorkgroupsIndirect(indirectBuffer);` with `indirectBuffer` specifying X and Y dimensions of 8 and 8, the entry point will be invoked 1024 times total ‚Äî Dispatching a 4 x 4 workgroup 8 times along both the X and Y axes. `4 * 4 * 8 * 8 = 1024`.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`dispatchWorkgroupsIndirect()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUComputePassEncoder")}} becomes invalid:

- `indirectBuffer`'s {{domxref("GPUBuffer.usage")}} contains the `GPUBufferUsage.INDIRECT` flag.
- `indirectOffset` + the total size specified by the `X`, `Y`, and `Z` dimensions is less than or equal to the `indirectBuffer`'s {{domxref("GPUBuffer.size")}}.
- `indirectOffset` is a multiple of 4.

## Examples

```js
// Set global buffer size
const BUFFER_SIZE = 1000;

// Compute shader; note workgroup size of 64
const shader = `
@group(0) @binding(0)
var<storage, read_write> output: array<f32>;

@compute @workgroup_size(64)

...

`;

// ...

// Create GPUCommandEncoder to encode commands to issue to the GPU
const commandEncoder = device.createCommandEncoder();

// Initiate render pass
const passEncoder = commandEncoder.beginComputePass();

// Issue commands
passEncoder.setPipeline(computePipeline);
passEncoder.setBindGroup(0, bindGroup);

const uint32 = new Uint32Array(3);
// Note workgroupCountX is set based on the global buffer size and the shader workgroup count.
uint32[0] = Math.ceil(BUFFER_SIZE / 64);
uint32[1] = 1;
uint32[2] = 1;

const workgroupDimensions = device.createBuffer({
  size: 12,
  usage: GPUBufferUsage.COPY_DST | GPUBufferUsage.INDIRECT,
});
device.queue.writeBuffer(workgroupDimensions, 0, uint32, 0, uint32.length);

passEncoder.dispatchWorkgroupsIndirect(workgroupDimensions, 0);

// End the render pass
passEncoder.end();

// Copy output buffer to staging buffer
commandEncoder.copyBufferToBuffer(
  output,
  0, // Source offset
  stagingBuffer,
  0, // Destination offset
  BUFFER_SIZE,
);

// End frame by passing array of command buffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucomputepassencoder/dispatchworkgroups/index.md
---
title: "GPUComputePassEncoder: dispatchWorkgroups() method"
short-title: dispatchWorkgroups()
slug: Web/API/GPUComputePassEncoder/dispatchWorkgroups
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUComputePassEncoder.dispatchWorkgroups
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`dispatchWorkgroups()`** method of the
{{domxref("GPUComputePassEncoder")}} interface dispatches a specific grid of workgroups to perform the work being done by the current {{domxref("GPUComputePipeline")}} (i.e. set via {{domxref("GPUComputePassEncoder.setPipeline()")}}).

## Syntax

```js-nolint
dispatchWorkgroups(workgroupCountX)
dispatchWorkgroups(workgroupCountX, workgroupCountY)
dispatchWorkgroups(workgroupCountX, workgroupCountY, workgroupCountZ)
```

### Parameters

- `workgroupCountX`
  - : The X dimension of the grid of workgroups to dispatch.
- `workgroupCountY` {{optional_inline}}
  - : The Y dimension of the grid of workgroups to dispatch. If omitted, `workgroupCountY` defaults to 1.
- `workgroupCountZ` {{optional_inline}}
  - : The Z dimension of the grid of workgroups to dispatch. If omitted, `workgroupCountZ` defaults to 1.

> **Note:** The X, Y, and Z dimension values passed to `dispatchWorkgroups()` and {{domxref("GPUComputePassEncoder.dispatchWorkgroupsIndirect()")}} are the number of workgroups to dispatch for each dimension, not the number of shader invocations to perform across each dimension. This matches the behavior of modern native GPU APIs, but differs from the behavior of OpenCL. This means that if a {{domxref("GPUShaderModule")}} defines an entry point with `@workgroup_size(4, 4)`, and work is dispatched to it with the call `passEncoder.dispatchWorkgroups(8, 8);`, the entry point will be invoked 1024 times total ‚Äî Dispatching a 4 x 4 workgroup 8 times along both the X and Y axes. `4 * 4 * 8 * 8 = 1024`.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`dispatchWorkgroups()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPUComputePassEncoder")}} becomes invalid:

- `workgroupCountX`, `workgroupCountY`, and `workgroupCountZ` are all less than or equal to the {{domxref("GPUDevice")}}'s `maxComputeWorkgroupsPerDimension` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.

## Examples

In our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/), several commands are recorded via a {{domxref("GPUCommandEncoder")}}. Most of these commands originate from the {{domxref("GPUComputePassEncoder")}} created via `beginComputePass()`.

At the start of the code, we set a global buffer size of 1000. Also, note that the workgroup size in the shader is set to 64.

```js
const BUFFER_SIZE = 1000;

// Compute shader
const shader = `
@group(0) @binding(0)
var<storage, read_write> output: array<f32>;

@compute @workgroup_size(64)

...

`;
```

Later in the code, the `dispatchWorkgroups()` `workgroupCountX` parameter is set based on the global buffer size and the shader workgroup count.

```js
// ...

// Create GPUCommandEncoder to encode commands to issue to the GPU
const commandEncoder = device.createCommandEncoder();

// Initiate render pass
const passEncoder = commandEncoder.beginComputePass();

// Issue commands
passEncoder.setPipeline(computePipeline);
passEncoder.setBindGroup(0, bindGroup);
passEncoder.dispatchWorkgroups(Math.ceil(BUFFER_SIZE / 64));

// End the render pass
passEncoder.end();

// Copy output buffer to staging buffer
commandEncoder.copyBufferToBuffer(
  output,
  0, // Source offset
  stagingBuffer,
  0, // Destination offset
  BUFFER_SIZE,
);

// End frame by passing array of command buffers to command queue for execution
device.queue.submit([commandEncoder.finish()]);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/navigator/gpu/index.md
---
title: "Navigator: gpu property"
short-title: gpu
slug: Web/API/Navigator/gpu
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.Navigator.gpu
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`Navigator.gpu`** read-only property returns the {{domxref("GPU")}} object for the current browsing context, which is the entry point for the {{domxref("WebGPU_API", "WebGPU API", "", "nocode")}}.

## Value

An {{domxref("GPU")}} object.

## Examples

```js
async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();
  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  const device = await adapter.requestDevice();

  //...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{domxref("WebGPU_API", "WebGPU API", "", "nocode")}}
-e 

File: /files/en-us/web/api/gputexture/destroy/index.md
---
title: "GPUTexture: destroy() method"
short-title: destroy()
slug: Web/API/GPUTexture/destroy
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUTexture.destroy
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`destroy()`** method of the
{{domxref("GPUTexture")}} interface destroys the `GPUTexture`.

## Syntax

```js-nolint
destroy()
```

### Parameters

None.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
// ...

const depthTexture = device.createTexture({
  size: [canvas.width, canvas.height],
  format: "depth24plus",
  usage: GPUTextureUsage.RENDER_ATTACHMENT,
});

// some time later

depthTexture.destroy();
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gputexture/samplecount/index.md
---
title: "GPUTexture: sampleCount property"
short-title: sampleCount
slug: Web/API/GPUTexture/sampleCount
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUTexture.sampleCount
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`sampleCount`** read-only property of the
{{domxref("GPUTexture")}} interface represents the sample count of the `GPUTexture`.

This is set via the `sampleCount` property in the descriptor object passed into the originating {{domxref("GPUDevice.createTexture()")}} call. If omitted, this defaults to 1.

## Value

A number. Possible values are:

- 1
- 4, which indicates a multi-sampled texture.

## Examples

```js
// ...

const depthTexture = device.createTexture({
  size: [canvas.width, canvas.height],
  format: "depth24plus",
  usage: GPUTextureUsage.RENDER_ATTACHMENT,
});

console.log(depthTexture.sampleCount); // 1
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gputexture/depthorarraylayers/index.md
---
title: "GPUTexture: depthOrArrayLayers property"
short-title: depthOrArrayLayers
slug: Web/API/GPUTexture/depthOrArrayLayers
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUTexture.depthOrArrayLayers
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`depthOrArrayLayers`** read-only property of the
{{domxref("GPUTexture")}} interface represents the depth or layer count of the `GPUTexture`.

This is set based on the `size` property in the descriptor object passed into the originating {{domxref("GPUDevice.createTexture()")}} call.

## Value

A number. This represents:

- The depth in pixels, in the case of textures with a `"3d"` {{domxref("GPUTexture.dimension")}}.
- The number of layers, in the case of layered textures with a `"2d"` {{domxref("GPUTexture.dimension")}}.

In cases where the `GPUTexture` does not have a depth or layers, the value is 1.

## Examples

```js
// ...

const test = device.createTexture({
  size: [128],
  format: "r8uint",
  dimension: "1d",
  usage: GPUTextureUsage.COPY_SRC,
});

console.log(test.depthOrArrayLayers); // 1
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gputexture/width/index.md
---
title: "GPUTexture: width property"
short-title: width
slug: Web/API/GPUTexture/width
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUTexture.width
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`width`** read-only property of the
{{domxref("GPUTexture")}} interface represents the width of the `GPUTexture`.

This is set based on the value of the `size` property in the descriptor object passed into the originating {{domxref("GPUDevice.createTexture()")}} call.

## Value

A number.

## Examples

```js
// ...

const depthTexture = device.createTexture({
  size: [640, 480],
  format: "depth24plus",
  usage: GPUTextureUsage.RENDER_ATTACHMENT,
});

console.log(depthTexture.width); // 640
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gputexture/height/index.md
---
title: "GPUTexture: height property"
short-title: height
slug: Web/API/GPUTexture/height
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUTexture.height
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`height`** read-only property of the
{{domxref("GPUTexture")}} interface represents the height of the `GPUTexture`.

This is set based on the value of the `size` property in the descriptor object passed into the originating {{domxref("GPUDevice.createTexture()")}} call.

## Value

A number.

## Examples

```js
// ...

const depthTexture = device.createTexture({
  size: [640, 480],
  format: "depth24plus",
  usage: GPUTextureUsage.RENDER_ATTACHMENT,
});

console.log(depthTexture.height); // 480
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gputexture/label/index.md
---
title: "GPUTexture: label property"
short-title: label
slug: Web/API/GPUTexture/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUTexture.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** property of the
{{domxref("GPUTexture")}} interface provides a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUDevice.createTexture()")}} call, or you can get and set it directly on the `GPUTexture` object.

## Value

A string. If this has not been previously set as described above, it will be an empty string.

## Examples

Setting and getting a label via `GPUTexture.label`:

```js
// ...

const depthTexture = device.createTexture({
  size: [canvas.width, canvas.height],
  format: "depth24plus",
  usage: GPUTextureUsage.RENDER_ATTACHMENT,
});

depthTexture.label = "mytexture";

console.log(depthTexture.label); // "mytexture"
```

Setting a label via the originating {{domxref("GPUDevice.createTexture()")}} call, and then getting it via `GPUTexture.label`:

```js
// ...

const depthTexture = device.createTexture({
  size: [canvas.width, canvas.height],
  format: "depth24plus",
  usage: GPUTextureUsage.RENDER_ATTACHMENT,
  label: "mytexture",
});

console.log(depthTexture.label); // "mytexture"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gputexture/usage/index.md
---
title: "GPUTexture: usage property"
short-title: usage
slug: Web/API/GPUTexture/usage
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUTexture.usage
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`usage`** read-only property of the
{{domxref("GPUTexture")}} interface is the {{glossary("bitwise flags")}} representing the allowed usages of the `GPUTexture`.

This is set via the `usage` property in the descriptor object passed into the originating {{domxref("GPUDevice.createTexture()")}} call.

## Value

The bitwise flags representing the original usages set when the `GPUTexture` was first created. The returned number is the sum of decimal values representing the different flags, as seen in the table below.

| Usage flag                          | Usage description                                                                                                                                                                                                                                                                                                                               | Hex equiv. | Decimal equiv. |
| ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | -------------- |
| `GPUTextureUsage.COPY_SRC`          | The texture can be used as the source of a copy operation, for example the source argument of a {{domxref("GPUCommandEncoder.copyTextureToBuffer", "copyTextureToBuffer()")}} call.                                                                                                                                                             | 0x01       | 1              |
| `GPUTextureUsage.COPY_DST`          | The texture can be used as the destination of a copy/write operation, for example the destination argument of a {{domxref("GPUCommandEncoder.copyBufferToTexture", "copyBufferToTexture()")}} call.                                                                                                                                             | 0x02       | 2              |
| `GPUTextureUsage.RENDER_ATTACHMENT` | The texture can be used as a color or depth/stencil attachment in a render pass, for example as the `view` property of the descriptor object in a {{domxref("GPUCommandEncoder.beginRenderPass", "beginRenderPass()")}} call.                                                                                                                   | 0x10       | 16             |
| `GPUTextureUsage.STORAGE_BINDING`   | The texture can be bound for use as a storage texture in a shader, for example as a resource in a bind group entry when creating a {{domxref("GPUBindGroup")}} (via {{domxref("GPUDevice.createBindGroup", "createBindGroup()")}}), which adheres to a {{domxref("GPUBindGroupLayout")}} entry with a specified storage texture binding layout. | 0x08       | 8              |
| `GPUTextureUsage.TEXTURE_BINDING`   | The texture can be bound for use as a sampled texture in a shader, for example as a resource in a bind group entry when creating a {{domxref("GPUBindGroup")}} (via {{domxref("GPUDevice.createBindGroup", "createBindGroup()")}}), which adheres to a {{domxref("GPUBindGroupLayout")}} entry with a specified texture binding layout.         | 0x04       | 4              |

## Examples

```js
// ...

const depthTexture = device.createTexture({
  size: [canvas.width, canvas.height],
  format: "depth24plus",
  usage: GPUTextureUsage.RENDER_ATTACHMENT,
});

console.log(depthTexture.usage); // 16
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gputexture/index.md
---
title: GPUTexture
slug: Web/API/GPUTexture
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUTexture
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUTexture`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents a container used to store 1D, 2D, or 3D arrays of data, such as images, to use in GPU rendering operations.

A `GPUTexture` object instance is created using the {{domxref("GPUDevice.createTexture()")}} method.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUTexture.depthOrArrayLayers", "depthOrArrayLayers")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A number representing the depth or layer count of the `GPUTexture` (pixels, or number of layers).
- {{domxref("GPUTexture.dimension", "dimension")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : An enumerated value representing the dimension of the set of texels for each `GPUTexture` subresource.
- {{domxref("GPUTexture.format", "format")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : An enumerated value representing the format of the `GPUTexture`.
- {{domxref("GPUTexture.height", "height")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A number representing the height of the `GPUTexture` in pixels.
- {{domxref("GPUTexture.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
- {{domxref("GPUTexture.mipLevelCount", "mipLevelCount")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A number representing the number of mip levels of the `GPUTexture`.
- {{domxref("GPUTexture.sampleCount", "sampleCount")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A number representing the sample count of the `GPUTexture`.
- {{domxref("GPUTexture.usage", "usage")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : The {{glossary("bitwise flags")}} representing the allowed usages of the `GPUTexture`.
- {{domxref("GPUTexture.width", "width")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A number representing the width of the `GPUTexture` in pixels.

## Instance methods

- {{domxref("GPUTexture.createView", "createView()")}} {{Experimental_Inline}}
  - : Creates a {{domxref("GPUTextureView")}} representing a specific view of the `GPUTexture`.
- {{domxref("GPUTexture.destroy", "destroy()")}} {{Experimental_Inline}}
  - : Destroys the `GPUTexture`.

## Examples

In the WebGPU samples [Textured Cube sample](https://webgpu.github.io/webgpu-samples/samples/texturedCube), a texture to use on the faces of a cube is created by:

- Loading the image into an {{domxref("HTMLImageElement")}} and creating an image bitmap using {{domxref("createImageBitmap()")}}.
- Creating a new `GPUTexture` using `createTexture()`.
- Copying the image bitmap into the texture using {{domxref("GPUQueue.copyExternalImageToTexture()")}}.

```js
//...
let cubeTexture: GPUTexture; // Sample is written in TypeScript
{
  const img = document.createElement("img");

  img.src = new URL(
    "../../../assets/img/Di-3d.png",
    import.meta.url
  ).toString();

  await img.decode();

  const imageBitmap = await createImageBitmap(img);

  cubeTexture = device.createTexture({
    size: [imageBitmap.width, imageBitmap.height, 1],
    format: "rgba8unorm",
    usage:
      GPUTextureUsage.TEXTURE_BINDING |
      GPUTextureUsage.COPY_DST |
      GPUTextureUsage.RENDER_ATTACHMENT,
  });

  device.queue.copyExternalImageToTexture(
    { source: imageBitmap },
    { texture: cubeTexture },
    [imageBitmap.width, imageBitmap.height]
  );
}
//...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gputexture/createview/index.md
---
title: "GPUTexture: createView() method"
short-title: createView()
slug: Web/API/GPUTexture/createView
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUTexture.createView
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`createView()`** method of the
{{domxref("GPUTexture")}} interface creates a {{domxref("GPUTextureView")}} representing a specific view of the `GPUTexture`.

## Syntax

```js-nolint
createView()
createView(descriptor)
```

### Parameters

- `descriptor` {{optional_inline}}

  - : An object containing the following properties:

    - `arrayLayerCount` {{optional_inline}}

      - : A number defining how many array layers are accessible to the view, starting with the `baseArrayLayer` value.

        If `arrayLayerCount` is omitted, it is given a value as follows:

        - If `dimension` is `"1d"`, `"2d"`, or `"3d"`, `arrayLayerCount` is 1.
        - If `dimension` is `"cube"`, `arrayLayerCount` is 6.
        - If `dimension` is `"2d-array"`, or `"cube-array"`, `arrayLayerCount` is {{domxref("GPUTexture.depthOrArrayLayers")}} - `baseArrayLayer`.

    - `aspect` {{optional_inline}}

      - : An enumerated value specifying which aspect(s) of the texture are accessible to the texture view. Possible values are:

        - `"all"`
          - : All available aspects of the texture format will be accessible to the view, which can mean all or any of color, depth, and stencil, depending on what kind of format you are dealing with.
        - `"depth-only"`
          - : Only the depth aspect of a [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format) will be accessible to the view.
        - `"stencil-only"`
          - : Only the stencil aspect of a depth-or-stencil format will be accessible to the view.

        If omitted, `aspect` takes a value of `"all"`.

    - `baseArrayLayer` {{optional_inline}}
      - : A number defining the index of the first array layer accessible to the view. If omitted, `baseArrayLayer` takes a value of 0.
    - `baseMipLevel` {{optional_inline}}
      - : A number representing the first (most detailed) mipmap level accessible to the view. If omitted, `baseMipLevel` takes a value of 0.
    - `dimension` {{optional_inline}}

      - : An enumerated value specifying the format to view the texture as. Possible values are:

        - `"1d"`: The texture is viewed as a one-dimensional image.
        - `"2d"`: The texture is viewed as a single two-dimensional image.
        - `"2d-array"`: The texture is viewed as an array of two-dimensional images.
        - `"cube"`: The texture is viewed as a cubemap. The view has 6 array layers, corresponding to the `[+X, -X, +Y, -Y, +Z, -Z]` faces of the cube. Sampling is done seamlessly across the faces of the cubemap.
        - `"cube-array"`: The texture is viewed as a packed array of N cubemaps, each with 6 array layers corresponding to the `[+X, -X, +Y, -Y, +Z, -Z]` faces of the cube. Sampling is done seamlessly across the faces of the cubemaps.
        - `"3d"`: The texture is viewed as a three-dimensional image.

        If `dimension` is omitted, it is given a value as follows:

        - If {{domxref("GPUTexture.dimension")}} is `"1d"`, `dimension` is `"1d"`.
        - If {{domxref("GPUTexture.dimension")}} is `"2d"` and {{domxref("GPUTexture.depthOrArrayLayers")}} is 1, `dimension` is `"2d"`.
        - If {{domxref("GPUTexture.dimension")}} is `"2d"` and {{domxref("GPUTexture.depthOrArrayLayers")}} is more than 1, `dimension` is `"2d-array"`.
        - If {{domxref("GPUTexture.dimension")}} is `"3d"`, `dimension` is `"3d"`.

    - `format` {{optional_inline}}

      - : An enumerated value specifying the format of the texture view. See the [Texture formats](https://gpuweb.github.io/gpuweb/#enumdef-gputextureformat) section of the specification for all the possible values.

        If `format` is omitted, it will be given a value as follows:

        - If `aspect` is `"depth-only"` or `"stencil-only"`, and {{domxref("GPUTexture.format")}} is a [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format), `format` will be set equal to the appropriate [aspect-specific format](https://gpuweb.github.io/gpuweb/#aspect-specific-format).
        - Otherwise it will be set equal to {{domxref("GPUTexture.format")}}.

    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
    - `mipLevelCount` {{optional_inline}}

      - : A number defining how many mipmap levels are accessible to the view, starting with the `baseMipLevel` value.

        If `mipLevelCount` is omitted, it will be given a value of {{domxref("GPUTexture.mipLevelCount")}} - `baseMipLevel`.

### Return value

A {{domxref("GPUTextureView")}} object instance.

### Validation

The following criteria must be met when calling **`createView()`**, otherwise a {{domxref("GPUValidationError")}} is generated and an invalid {{domxref("GPUTextureView")}} object is returned:

- If `aspect` is `"all"`, `format` is equal to {{domxref("GPUTexture.format")}}, or one of the `viewFormats` specified in the originating {{domxref("GPUDevice.createTexture()")}} call's descriptor object.
- If `aspect` is `"depth-only"` or `"stencil-only"`, `format` is equal to the appropriate [aspect-specific format](https://gpuweb.github.io/gpuweb/#aspect-specific-format) of the [depth-or-stencil format](https://gpuweb.github.io/gpuweb/#combined-depth-stencil-format).
- `mipLevelCount` is greater than 0.
- `mipLevelCount` + `baseMipLevel` is less than or equal to {{domxref("GPUTexture.mipLevelCount")}}.
- `arrayLayerCount` is greater than 0.
- `arrayLayerCount` + `baseArrayLayer` is less than or equal to {{domxref("GPUTexture.depthOrArrayLayers")}}.
- If `sampleCount` is greater than 1, `dimension` is `"2d"`.
- If `dimension` is:
  - `"1d"`
    - {{domxref("GPUTexture.dimension")}} is `"1d"`
    - `arrayLayerCount` is 1
  - `"2d"`
    - {{domxref("GPUTexture.dimension")}} is `"2d"`
    - `arrayLayerCount` is 1
  - `"2d-array"`
    - {{domxref("GPUTexture.dimension")}} is `"2d"`
  - `"cube"`
    - {{domxref("GPUTexture.dimension")}} is `"2d"`
    - `arrayLayerCount` is 6
    - {{domxref("GPUTexture.width")}} is equal to {{domxref("GPUTexture.height")}}
  - `"cube-array"`
    - {{domxref("GPUTexture.dimension")}} is `"2d"`
    - `arrayLayerCount` is a multiple of 6
    - {{domxref("GPUTexture.width")}} is equal to {{domxref("GPUTexture.height")}}
  - `"3d"`
    - {{domxref("GPUTexture.dimension")}} is `"3d"`
    - `arrayLayerCount` is 1

## Examples

In the WebGPU Samples [Cubemap demo](https://webgpu.github.io/webgpu-samples/samples/cubemap), you will see multiple examples of how `createView()` is used, both as to create a view `resource` for a {{domxref("GPUDevice.createBindGroup()")}} call, and to provide a `view` in the `depthStencilAttachment` object of a {{domxref("GPUCommandEncoder.beginRenderPass()")}} descriptor.

```js
const uniformBindGroup = device.createBindGroup({
  layout: pipeline.getBindGroupLayout(0),
  entries: [
    {
      binding: 0,
      resource: {
        buffer: uniformBuffer,
        offset: 0,
        size: uniformBufferSize,
      },
    },
    {
      binding: 1,
      resource: sampler,
    },
    {
      binding: 2,
      resource: cubemapTexture.createView({
        dimension: "cube",
      }),
    },
  ],
});

const renderPassDescriptor: GPURenderPassDescriptor = {
  colorAttachments: [
    {
      view: undefined, // Assigned later
      loadOp: "clear",
      storeOp: "store",
    },
  ],
  depthStencilAttachment: {
    view: depthTexture.createView(),

    depthClearValue: 1.0,
    depthLoadOp: "clear",
    depthStoreOp: "store",
  },
};

// ...

const commandEncoder = device.createCommandEncoder();
const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gputexture/format/index.md
---
title: "GPUTexture: format property"
short-title: format
slug: Web/API/GPUTexture/format
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUTexture.format
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`format`** read-only property of the
{{domxref("GPUTexture")}} interface represents the format of the `GPUTexture`.

This is set via the `format` property in the descriptor object passed into the originating {{domxref("GPUDevice.createTexture()")}} call.

## Value

An enumerated value. See the [Texture formats](https://gpuweb.github.io/gpuweb/#enumdef-gputextureformat) section of the specification for all the possible values.

## Examples

```js
// ...

const depthTexture = device.createTexture({
  size: [canvas.width, canvas.height],
  format: "depth24plus",
  usage: GPUTextureUsage.RENDER_ATTACHMENT,
});

console.log(depthTexture.format); // "depth24plus"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gputexture/miplevelcount/index.md
---
title: "GPUTexture: mipLevelCount property"
short-title: mipLevelCount
slug: Web/API/GPUTexture/mipLevelCount
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUTexture.mipLevelCount
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`mipLevelCount`** read-only property of the
{{domxref("GPUTexture")}} interface represents the number of mip levels of the `GPUTexture`.

This is set via the `mipLevelCount` property in the descriptor object passed into the originating {{domxref("GPUDevice.createTexture()")}} call. If omitted, this defaults to 1.

## Value

A number.

## Examples

```js
// ...

const depthTexture = device.createTexture({
  size: [canvas.width, canvas.height],
  format: "depth24plus",
  usage: GPUTextureUsage.RENDER_ATTACHMENT,
});

console.log(depthTexture.mipLevelCount); // 1
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gputexture/dimension/index.md
---
title: "GPUTexture: dimension property"
short-title: dimension
slug: Web/API/GPUTexture/dimension
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUTexture.dimension
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`dimension`** read-only property of the
{{domxref("GPUTexture")}} interface represents the dimension of the set of texels for each `GPUTexture` subresource.

This is set via the `dimension` property in the descriptor object passed into the originating {{domxref("GPUDevice.createTexture()")}} call, which defaults to `"2d"` if omitted.

## Value

An enumerated value. Possible values are:

- `"1d"`: A one-dimensional texture with a single dimension, width.
- `"2d"`: A two-dimensional texture with a width and height, which may also have layers. Only `"2d"` textures can have mipmaps, be multisampled, use a compressed or depth/stencil format, and be used as a render attachment.
- `"3d"`: A three-dimensional texture with a width, height, and depth.

## Examples

```js
// ...

const depthTexture = device.createTexture({
  size: [canvas.width, canvas.height],
  format: "depth24plus",
  usage: GPUTextureUsage.RENDER_ATTACHMENT,
});

console.log(depthTexture.dimension); // "2d"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundle/label/index.md
---
title: "GPURenderBundle: label property"
short-title: label
slug: Web/API/GPURenderBundle/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPURenderBundle.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** read-only property of the
{{domxref("GPURenderBundle")}} interface is a string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPURenderBundleEncoder.finish()")}} call, or you can get and set it directly on the `GPURenderBundle` object.

## Value

A string. If no label value has previously been set, getting the label returns an empty string.

## Examples

Setting and getting a label via `GPURenderBundle.label`:

```js
const renderBundle = renderBundleEncoder.finish();

renderBundle.label = "myrenderbundle";
console.log(renderBundle.label); // "myrenderbundle"
```

Setting a label via the originating {{domxref("GPURenderBundleEncoder.finish()")}} call, and then getting it via `GPURenderBundle.label`:

```js
const renderBundle = renderBundleEncoder.finish({
  label: "myrenderbundle",
});

console.log(renderBundle.label); // "myrenderbundle"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundle/index.md
---
title: GPURenderBundle
slug: Web/API/GPURenderBundle
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPURenderBundle
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPURenderBundle`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents a container for pre-recorded bundles of commands.

The command bundles are encoded using a {{domxref("GPURenderBundleEncoder")}}; once the desired commands have been encoded, they are recorded into a `GPURenderBundle` object instance using the {{domxref("GPURenderBundleEncoder.finish()")}} method.

These command bundles can then be reused across multiple render passes by passing the `GPURenderBundle` objects into {{domxref("GPURenderPassEncoder.executeBundles()")}} calls. Reusing pre-recoded commands can significantly improve app performance in situations where JavaScript draw call overhead is a bottleneck. Render bundles are most effective in situations where a batch of objects will be drawn the same way across multiple views or frames, with the only differences being the buffer content being used (such as updated matrix uniforms).

A good example is VR rendering. Recording the rendering as a render bundle and then tweaking the view matrix and replaying it for each eye is a more efficient way to issue draw calls for both renderings of the scene.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUComputePassEncoder.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Examples

In the WebGPU Samples [Animometer example](https://webgpu.github.io/webgpu-samples/samples/animometer), a lot of like operations are done on many different objects simultaneously. A render bundle is encoded using the following function:

```js
function recordRenderPass(
  passEncoder: GPURenderBundleEncoder | GPURenderPassEncoder
) {
  if (settings.dynamicOffsets) {
    passEncoder.setPipeline(dynamicPipeline);
  } else {
    passEncoder.setPipeline(pipeline);
  }
  passEncoder.setVertexBuffer(0, vertexBuffer);
  passEncoder.setBindGroup(0, timeBindGroup);
  const dynamicOffsets = [0];
  for (let i = 0; i < numTriangles; ++i) {
    if (settings.dynamicOffsets) {
      dynamicOffsets[0] = i * alignedUniformBytes;
      passEncoder.setBindGroup(1, dynamicBindGroup, dynamicOffsets);
    } else {
      passEncoder.setBindGroup(1, bindGroups[i]);
    }
    passEncoder.draw(3, 1, 0, 0);
  }
}
```

Later on, a {{domxref("GPURenderBundleEncoder")}} is created, the function is invoked, and the render bundle is recorded using {{domxref("GPURenderBundleEncoder.finish()")}}:

```js
const renderBundleEncoder = device.createRenderBundleEncoder({
  colorFormats: [presentationFormat],
});
recordRenderPass(renderBundleEncoder);
const renderBundle = renderBundleEncoder.finish();
```

{{domxref("GPURenderPassEncoder.executeBundles()")}} is then used to reuse the work across multiple render passes to improve performance. Study the example code listing for the full context.

```js
// ...

return function doDraw(timestamp) {
  if (startTime === undefined) {
    startTime = timestamp;
  }
  uniformTime[0] = (timestamp - startTime) / 1000;
  device.queue.writeBuffer(uniformBuffer, timeOffset, uniformTime.buffer);

  renderPassDescriptor.colorAttachments[0].view = context
    .getCurrentTexture()
    .createView();

  const commandEncoder = device.createCommandEncoder();
  const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

  if (settings.renderBundles) {
    passEncoder.executeBundles([renderBundle]);
  } else {
    recordRenderPass(passEncoder);
  }

  passEncoder.end();
  device.queue.submit([commandEncoder.finish()]);
};

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/drawindexedindirect/index.md
---
title: "GPURenderBundleEncoder: drawIndexedIndirect() method"
short-title: drawIndexedIndirect()
slug: Web/API/GPURenderBundleEncoder/drawIndexedIndirect
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder.drawIndexedIndirect
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`drawIndexedIndirect()`** method of the
{{domxref("GPURenderBundleEncoder")}} interface draws indexed primitives using parameters read from a {{domxref("GPUBuffer")}}.

> **Note:** This method is functionally identical to its equivalent on {{domxref("GPURenderPassEncoder")}} ‚Äî {{domxref("GPURenderPassEncoder.drawIndexedIndirect", "drawIndexedIndirect()")}}.

## Syntax

```js-nolint
drawIndexedIndirect(indirectBuffer, indirectOffset)
```

### Parameters

- `indirectBuffer`

  - : A {{domxref("GPUBuffer")}} containing the `indexCount`, `instanceCount`, `firstIndex`, `baseVertex`, and `firstInstance` values needed to carry out the drawing operation. The buffer must contain a tightly packed block of five 32-bit unsigned integer values representing the values (20 bytes total), given in the same order as the arguments for {{domxref("GPURenderBundleEncoder.drawIndexed()")}}. So for example:

    ```js
    const uint32 = new Uint32Array(5);
    uint32[0] = 3; // The indexCount value
    uint32[1] = 1; // The instanceCount value
    uint32[2] = 0; // The firstIndex value
    uint32[3] = 0; // The baseVertex value
    uint32[4] = 0; // The firstInstance value

    // Write values into a GPUBuffer
    device.queue.writeBuffer(buffer, 0, uint32, 0, uint32.length);
    ```

- `indirectOffset`
  - : The offset, in bytes, into `indirectBuffer` where the value data begins.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`drawIndirect()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderBundleEncoder")}} becomes invalid:

- `indirectBuffer`'s {{domxref("GPUBuffer.usage")}} contains the `GPUBufferUsage.INDIRECT` flag.
- `indirectOffset` + the total size specified by the value parameters in the `indirectBuffer` is less than or equal to the `indirectBuffer`'s {{domxref("GPUBuffer.size")}}.
- `indirectOffset` is a multiple of 4.

## Examples

```js
// ...

// Create GPURenderBundleEncoder
const bundleEncoder = device.createRenderBundleEncoder(descriptor);

// Set pipeline and vertex buffer
bundleEncoder.setPipeline(renderPipeline);
bundleEncoder.setVertexBuffer(0, vertexBuffer);
bundleEncoder.setIndexBuffer(indexBuffer, "uint16");

// Create drawIndexedIndirect values
const uint32 = new Uint32Array(5);
uint32[0] = 3;
uint32[1] = 1;
uint32[2] = 0;
uint32[3] = 0;
uint32[4] = 0;

// Create a GPUBuffer and write the draw values into it
const drawValues = device.createBuffer({
  size: 20,
  usage: GPUBufferUsage.COPY_DST | GPUBufferUsage.INDIRECT,
});
device.queue.writeBuffer(drawValues, 0, uint32, 0, uint32.length);

// Draw the vertices
bundleEncoder.drawIndexedIndirect(drawValues, 0);

// End the bundle recording
const renderBundle = bundleEncoder.finish();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/drawindirect/index.md
---
title: "GPURenderBundleEncoder: drawIndirect() method"
short-title: drawIndirect()
slug: Web/API/GPURenderBundleEncoder/drawIndirect
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder.drawIndirect
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`drawIndirect()`** method of the
{{domxref("GPURenderBundleEncoder")}} interface draws primitives using parameters read from a {{domxref("GPUBuffer")}}.

> **Note:** This method is functionally identical to its equivalent on {{domxref("GPURenderPassEncoder")}} ‚Äî {{domxref("GPURenderPassEncoder.drawIndirect", "drawIndirect()")}}.

## Syntax

```js-nolint
drawIndirect(indirectBuffer, indirectOffset)
```

### Parameters

- `indirectBuffer`

  - : A {{domxref("GPUBuffer")}} containing the `vertexCount`, `instanceCount`, `firstVertex`, and `firstInstance` values needed to carry out the drawing operation. The buffer must contain a tightly packed block of four 32-bit unsigned integer values representing the values (16 bytes total), given in the same order as the arguments for {{domxref("GPURenderBundleEncoder.draw()")}}. So for example:

    ```js
    const uint32 = new Uint32Array(4);
    uint32[0] = 3; // The vertexCount value
    uint32[1] = 1; // The instanceCount value
    uint32[2] = 0; // The firstVertex value
    uint32[3] = 0; // The firstInstance value

    // Write values into a GPUBuffer
    device.queue.writeBuffer(buffer, 0, uint32, 0, uint32.length);
    ```

- `indirectOffset`
  - : The offset, in bytes, into `indirectBuffer` where the value data begins.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`drawIndirect()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderBundleEncoder")}} becomes invalid:

- `indirectBuffer`'s {{domxref("GPUBuffer.usage")}} contains the `GPUBufferUsage.INDIRECT` flag.
- `indirectOffset` + the total size specified by the value parameters in the `indirectBuffer` is less than or equal to the `indirectBuffer`'s {{domxref("GPUBuffer.size")}}.
- `indirectOffset` is a multiple of 4.

## Examples

```js
// ...

// Create GPURenderBundleEncoder
const bundleEncoder = device.createRenderBundleEncoder(descriptor);

// Set pipeline and vertex buffer
bundleEncoder.setPipeline(renderPipeline);
bundleEncoder.setVertexBuffer(0, vertexBuffer);

// Create drawIndirect values
const uint32 = new Uint32Array(4);
uint32[0] = 3;
uint32[1] = 1;
uint32[2] = 0;
uint32[3] = 0;

// Create a GPUBuffer and write the draw values into it
const drawValues = device.createBuffer({
  size: 16,
  usage: GPUBufferUsage.COPY_DST | GPUBufferUsage.INDIRECT,
});
device.queue.writeBuffer(drawValues, 0, uint32, 0, uint32.length);

// Draw the vertices
bundleEncoder.drawIndirect(drawValues, 0);

// End the bundle recording
const renderBundle = bundleEncoder.finish();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/setpipeline/index.md
---
title: "GPURenderBundleEncoder: setPipeline() method"
short-title: setPipeline()
slug: Web/API/GPURenderBundleEncoder/setPipeline
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder.setPipeline
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setPipeline()`** method of the
{{domxref("GPURenderBundleEncoder")}} interface sets the {{domxref("GPURenderPipeline")}} to use for subsequent render bundle commands.

> **Note:** This method is functionally identical to its equivalent on {{domxref("GPURenderPassEncoder")}} ‚Äî {{domxref("GPURenderPassEncoder.setPipeline", "setPipeline()")}}.

## Syntax

```js-nolint
setPipeline(pipeline)
```

### Parameters

- `pipeline`
  - : The {{domxref("GPURenderPipeline")}} to use for subsequent render bundle commands.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`setPipeline()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderBundleEncoder")}} becomes invalid:

- If the {{domxref("GPURenderPipeline")}} writes to the depth component of the depth/stencil attachment, `depthReadOnly` (as specified in the descriptor of the originating {{domxref("GPUCommandEncoder.beginRenderPass()")}} call) is `true`.
- If the {{domxref("GPURenderPipeline")}} writes to the stencil component of the depth/stencil attachment, `stencilReadOnly` (as specified in the descriptor of the originating {{domxref("GPUCommandEncoder.beginRenderPass()")}} call) is `true`.

## Examples

```js
function recordRenderPass(
  passEncoder: GPURenderBundleEncoder | GPURenderPassEncoder // TypeScript
) {
  if (settings.dynamicOffsets) {
    passEncoder.setPipeline(dynamicPipeline);
  } else {
    passEncoder.setPipeline(pipeline);
  }
  passEncoder.setVertexBuffer(0, vertexBuffer);
  passEncoder.setBindGroup(0, timeBindGroup);
  const dynamicOffsets = [0];
  for (let i = 0; i < numTriangles; ++i) {
    if (settings.dynamicOffsets) {
      dynamicOffsets[0] = i * alignedUniformBytes;
      passEncoder.setBindGroup(1, dynamicBindGroup, dynamicOffsets);
    } else {
      passEncoder.setBindGroup(1, bindGroups[i]);
    }
    passEncoder.draw(3, 1, 0, 0);
  }
}
```

The above snippet is taken from the WebGPU Samples [Animometer example](https://webgpu.github.io/webgpu-samples/samples/animometer).

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/setbindgroup/index.md
---
title: "GPURenderBundleEncoder: setBindGroup() method"
short-title: setBindGroup()
slug: Web/API/GPURenderBundleEncoder/setBindGroup
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder.setBindGroup
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setBindGroup()`** method of the
{{domxref("GPURenderBundleEncoder")}} interface sets the {{domxref("GPUBindGroup")}} to use for subsequent render bundle commands, for a given index.

> **Note:** This method is functionally identical to its equivalent on {{domxref("GPURenderPassEncoder")}} ‚Äî {{domxref("GPURenderPassEncoder.setBindGroup", "setBindGroup()")}}.

## Syntax

```js-nolint
setBindGroup(index, bindGroup)
setBindGroup(index, bindGroup, dynamicOffsets)
setBindGroup(index, bindGroup, dynamicOffsets, dynamicOffsetsStart,
             dynamicOffsetsLength)
```

### Parameters

- `index`
  - : The index to set the bind group at. This matches the `n` index value of the corresponding [`@group(n)`](https://gpuweb.github.io/gpuweb/wgsl/#attribute-group) attribute in the shader code ({{domxref("GPUShaderModule")}}) used in the related pipeline.
- `bindGroup`
  - : The {{domxref("GPUBindGroup")}} to use for subsequent render bundle commands.
- `dynamicOffsets` {{optional_inline}}
  - : A value specifying the offset, in bytes, for each entry in `bindGroup` with `hasDynamicOffset: true` set (i.e. in the descriptor of the {{domxref("GPUDevice.createBindGroupLayout()")}} call that created the {{domxref("GPUBindGroupLayout")}} object that the `bindGroup` is based on). This value can be:
    - An array of numbers specifying the different offsets.
    - A {{jsxref("Uint32Array")}} containing numbers specifying the offsets.

If a {{jsxref("Uint32Array")}} value is specified for `dynamicOffsets`, both of the following parameters are also required:

- `dynamicOffsetsStart`
  - : A number specifying the offset, in array elements, into `dynamicOffsetsData`, where the dynamic offset data begins.
- `dynamicOffsetsLength`
  - : A number specifying the number of dynamic offset values to be read from in `dynamicOffsetsData`.

### Return value

None ({{jsxref("Undefined")}}).

### Exceptions

For `setBindGroup()` calls that use a {{jsxref("Uint32Array")}} value for `dynamicOffsets`, the call will throw with a `RangeError` {{domxref("DOMException")}} if:

- `dynamicOffsetsStart` is less than 0.
- `dynamicOffsetsStart` + `dynamicOffsetsLength` is greater than `dynamicOffsets.length`.

### Validation

The following criteria must be met when calling **`setBindGroup()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderBundleEncoder")}} becomes invalid:

- `index` is less than or equal to the {{domxref("GPUDevice")}}'s `maxBindGroups` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- `dynamicOffsets.length` is the same as the number of entries in `bindGroup` with `hasDynamicOffset: true` set.
- For `bindGroup` entries where the bound `buffer`'s `type` is `"uniform"` (see {{domxref("GPUDevice.createBindGroupLayout()")}}), each number in `dynamicOffsets` is a multiple of the {{domxref("GPUDevice")}}'s `minUniformBufferOffsetAlignment` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- For `bindGroup` entries where the bound `buffer`'s `type` is `"storage"` or `"read-only-storage"` (see {{domxref("GPUDevice.createBindGroupLayout()")}}), each number in `dynamicOffsets` is a multiple of the {{domxref("GPUDevice")}}'s `minStorageBufferOffsetAlignment` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- For each `bindGroup` entry, the bound `buffer`'s `offset`, plus the corresponding layout entry's `minBindingSize`, plus the corresponding dynamic offset specified in `dynamicOffsets`, is less than or equal to the bound `buffer`'s `size`.

## Examples

```js
function recordRenderPass(
  passEncoder: GPURenderBundleEncoder | GPURenderPassEncoder // TypeScript
) {
  if (settings.dynamicOffsets) {
    passEncoder.setPipeline(dynamicPipeline);
  } else {
    passEncoder.setPipeline(pipeline);
  }
  passEncoder.setVertexBuffer(0, vertexBuffer);
  passEncoder.setBindGroup(0, timeBindGroup);
  const dynamicOffsets = [0];
  for (let i = 0; i < numTriangles; ++i) {
    if (settings.dynamicOffsets) {
      dynamicOffsets[0] = i * alignedUniformBytes;
      passEncoder.setBindGroup(1, dynamicBindGroup, dynamicOffsets);
    } else {
      passEncoder.setBindGroup(1, bindGroups[i]);
    }
    passEncoder.draw(3, 1, 0, 0);
  }
}
```

The above snippet is taken from the WebGPU Samples [Animometer example](https://webgpu.github.io/webgpu-samples/samples/animometer).

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/setvertexbuffer/index.md
---
title: "GPURenderBundleEncoder: setVertexBuffer() method"
short-title: setVertexBuffer()
slug: Web/API/GPURenderBundleEncoder/setVertexBuffer
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder.setVertexBuffer
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setVertexBuffer()`** method of the
{{domxref("GPURenderBundleEncoder")}} interface sets or unsets the current {{domxref("GPUBuffer")}} for the given slot that will provide vertex data for subsequent drawing commands.

> **Note:** This method is functionally identical to its equivalent on {{domxref("GPURenderPassEncoder")}} ‚Äî {{domxref("GPURenderPassEncoder.setVertexBuffer", "setVertexBuffer()")}}.

## Syntax

```js-nolint
setVertexBuffer(slot, buffer, offset, size)
```

### Parameters

- `slot`
  - : A number referencing the vertex buffer slot to set the vertex buffer for.
- `buffer`
  - : A {{domxref("GPUBuffer")}} representing the buffer containing the vertex data to use for subsequent drawing commands, or `null`, in which case any previously-set buffer in the given slot is unset.
- `offset` {{optional_inline}}
  - : A number representing the offset, in bytes, into `buffer` where the vertex data begins. If omitted, `offset` defaults to 0.
- `size` {{optional_inline}}
  - : A number representing the size, in bytes, of the vertex data contained in `buffer`. If omitted, `size` defaults to the `buffer`'s {{domxref("GPUBuffer.size")}} - `offset`.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`setVertexBuffer()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderBundleEncoder")}} becomes invalid:

- `buffer`'s {{domxref("GPUBuffer.usage")}} contains the `GPUBufferUsage.VERTEX` flag.
- `slot` is less than the {{domxref("GPUDevice")}}'s `maxVertexBuffers` {{domxref("GPUSupportedLimits", "limit", "", "nocode")}}.
- `offset` + `size` is less than or equal to the `buffer`'s {{domxref("GPUBuffer.size")}}.
- `offset` is a multiple of 4.

## Examples

### Set vertex buffer

```js
function recordRenderPass(
  passEncoder: GPURenderBundleEncoder | GPURenderPassEncoder // TypeScript
) {
  if (settings.dynamicOffsets) {
    passEncoder.setPipeline(dynamicPipeline);
  } else {
    passEncoder.setPipeline(pipeline);
  }
  passEncoder.setVertexBuffer(0, vertexBuffer);
  passEncoder.setBindGroup(0, timeBindGroup);
  const dynamicOffsets = [0];
  for (let i = 0; i < numTriangles; ++i) {
    if (settings.dynamicOffsets) {
      dynamicOffsets[0] = i * alignedUniformBytes;
      passEncoder.setBindGroup(1, dynamicBindGroup, dynamicOffsets);
    } else {
      passEncoder.setBindGroup(1, bindGroups[i]);
    }
    passEncoder.draw(3, 1, 0, 0);
  }
}
```

The above snippet is taken from the WebGPU Samples [Animometer example](https://webgpu.github.io/webgpu-samples/samples/animometer).

### Unset vertex buffer

```js
// Set vertex buffer in slot 0
passEncoder.setVertexBuffer(0, vertexBuffer);

// Later, unset vertex buffer in slot 0
passEncoder.setVertexBuffer(0, null);
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/setindexbuffer/index.md
---
title: "GPURenderBundleEncoder: setIndexBuffer() method"
short-title: setIndexBuffer()
slug: Web/API/GPURenderBundleEncoder/setIndexBuffer
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder.setIndexBuffer
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`setIndexBuffer()`** method of the
{{domxref("GPURenderBundleEncoder")}} interface sets the current {{domxref("GPUBuffer")}} that will provide index data for subsequent drawing commands.

> **Note:** This method is functionally identical to its equivalent on {{domxref("GPURenderPassEncoder")}} ‚Äî {{domxref("GPURenderPassEncoder.setIndexBuffer", "setIndexBuffer()")}}.

## Syntax

```js-nolint
setIndexBuffer(buffer, indexFormat, offset, size)
```

### Parameters

- `buffer`
  - : A {{domxref("GPUBuffer")}} representing the buffer containing the index data to use for subsequent drawing commands.
- `indexFormat`
  - : An enumerated value that defines the format of the index data contained in `buffer`. Possible values are:
    - `"uint16"`
    - `"uint32"`
- `offset` {{optional_inline}}
  - : A number representing the offset, in bytes, into `buffer` where the index data begins. If omitted, `offset` defaults to 0.
- `size` {{optional_inline}}
  - : A number representing the size, in bytes, of the index data contained in `buffer`. If omitted, `size` defaults to the `buffer`'s {{domxref("GPUBuffer.size")}} - `offset`.

#### Note on indexFormat

`indexFormat` determines both the data type of index values in a buffer and, when used with a pipeline that specifies a strip primitive topology (`"line-strip"` or `"triangle-strip"`), also determines the primitive restart value. The primitive restart value is an index value indicating that a new primitive should be started rather than continuing to construct the strip with the prior indexed vertices. The value is `0xFFFF` for `"uint16"`, or `0xFFFFFFFF` for `"uint32"`.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`setIndexBuffer()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderBundleEncoder")}} becomes invalid:

- `buffer`'s {{domxref("GPUBuffer.usage")}} contains the `GPUBufferUsage.INDEX` flag.
- `offset` + `size` is less than or equal to the `buffer`'s {{domxref("GPUBuffer.size")}}.
- `offset` is a multiple of `indexFormat`'s byte size (2 for `"uint16"`, 4 for `"uint32"`).

## Examples

```js
// ...

const bundleEncoder = device.createRenderBundleEncoder(descriptor);

bundleEncoder.setPipeline(pipeline);
bundleEncoder.setBindGroup(0, sceneBindGroupForRender);
bundleEncoder.setBindGroup(1, modelBindGroup);
bundleEncoder.setVertexBuffer(0, vertexBuffer);
bundleEncoder.setIndexBuffer(indexBuffer, "uint16");
bundleEncoder.drawIndexed(indexCount);

const renderBundle = bundleEncoder.finish();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/label/index.md
---
title: "GPURenderBundleEncoder: label property"
short-title: label
slug: Web/API/GPURenderBundleEncoder/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** read-only property of the
{{domxref("GPURenderBundleEncoder")}} interface is a string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUDevice.createRenderBundleEncoder()")}} call, or you can get and set it directly on the `GPURenderBundleEncoder` object.

> **Note:** This property is functionally identical to its equivalent on {{domxref("GPURenderPassEncoder")}} ‚Äî {{domxref("GPURenderPassEncoder.label", "label")}}.

## Value

A string. If no label value has previously been set, getting the label returns an empty string.

## Examples

Setting and getting a label via `GPURenderBundleEncoder.label`:

```js
const renderBundleEncoder = device.createRenderBundleEncoder({
  colorFormats: [presentationFormat],
});

renderBundleEncoder.label = "myrenderbundleencoder";
console.log(renderBundleEncoder.label); // "myrenderbundleencoder"
```

Setting a label via the originating {{domxref("GPUDevice.createRenderBundleEncoder()")}} call, and then getting it via `GPURenderBundleEncoder.label`:

```js
const renderBundleEncoder = device.createRenderBundleEncoder({
  colorFormats: [presentationFormat],
  label: "myrenderbundleencoder",
});

console.log(renderBundleEncoder.label); // "myrenderbundleencoder"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/insertdebugmarker/index.md
---
title: "GPURenderBundleEncoder: insertDebugMarker() method"
short-title: insertDebugMarker()
slug: Web/API/GPURenderBundleEncoder/insertDebugMarker
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder.insertDebugMarker
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`insertDebugMarker()`** method of the
{{domxref("GPURenderBundleEncoder")}} interface marks a specific point in a series of encoded render bundle pass commands with a label.

This could be used for telemetry, or may be utilized in {{domxref("GPUError")}} messages, browser dev tools, or other services in the future to help with debugging.

> **Note:** This method is functionally identical to its equivalent on {{domxref("GPURenderPassEncoder")}} ‚Äî {{domxref("GPURenderPassEncoder.InsertDebugMarker", "InsertDebugMarker()")}}.

## Syntax

```js-nolint
insertDebugMarker(markerLabel)
```

### Parameters

- `markerLabel`
  - : A string representing the label to insert.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
// ...

bundleEncoder.insertDebugMarker("mymarker");

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/index.md
---
title: GPURenderBundleEncoder
slug: Web/API/GPURenderBundleEncoder
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPURenderBundleEncoder`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} is used to pre-record bundles of commands.

The command bundles are encoded by calling the methods of `GPURenderBundleEncoder`; once the desired commands have been encoded, they are recorded into a {{domxref("GPURenderBundle")}} object instance using the {{domxref("GPURenderBundleEncoder.finish()")}} method. These render bundles can then be reused across multiple render passes by passing the `GPURenderBundle` objects into {{domxref("GPURenderPassEncoder.executeBundles()")}} calls.

In effect, this is like a partial render pass ‚Äî `GPURenderBundleEncoder`s have all the same functionality available as {{domxref("GPURenderPassEncoder")}}s, except that they can't begin and end occlusion queries, and can't set the scissor rect, viewport, blend constant, and stencil reference. The `GPURenderBundle` will inherit all these values from the {{domxref("GPURenderPassEncoder")}} that executes it.

> **Note:** Currently set vertex buffers, index buffers, bind groups, and pipeline are all cleared prior to executing a render bundle, and once the render bundle has finished executing.

Reusing pre-recoded commands can significantly improve app performance in situations where JavaScript draw call overhead is a bottleneck. Render bundles are most effective in situations where a batch of objects will be drawn the same way across multiple views or frames, with the only differences being the buffer content being used (such as updated matrix uniforms). A good example is VR rendering. Recording the rendering as a render bundle and then tweaking the view matrix and replaying it for each eye is a more efficient way to issue draw calls for both renderings of the scene.

A `GPURenderBundleEncoder` object instance is created via the {{domxref("GPUDevice.createRenderBundleEncoder()")}} property.

> **Note:** The methods of `GPURenderBundleEncoder` are functionally identical to their equivalents available on {{domxref("GPURenderPassEncoder")}}, except for {{domxref("GPURenderBundleEncoder.finish()")}}, which is similar in purpose to {{domxref("GPUCommandEncoder.finish()")}}.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPURenderBundleEncoder.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Instance methods

- {{domxref("GPURenderBundleEncoder.draw", "draw()")}} {{Experimental_Inline}}
  - : Draw primitives based on the vertex buffers provided by {{domxref("GPURenderBundleEncoder.setVertexBuffer", "setVertexBuffer()")}}.
- {{domxref("GPURenderBundleEncoder.drawIndexed", "drawIndexed()")}} {{Experimental_Inline}}
  - : Draw indexed primitives based on the vertex and index buffers provided by {{domxref("GPURenderBundleEncoder.setVertexBuffer", "setVertexBuffer()")}} and {{domxref("GPURenderBundleEncoder.setIndexBuffer", "setIndexBuffer()")}}
- {{domxref("GPURenderBundleEncoder.drawIndirect", "drawIndirect()")}} {{Experimental_Inline}}
  - : Draw primitives using parameters read from a {{domxref("GPUBuffer")}}.
- {{domxref("GPURenderBundleEncoder.drawIndexedIndirect", "drawIndexedIndirect()")}} {{Experimental_Inline}}

  - : Draw indexed primitives using parameters read from a {{domxref("GPUBuffer")}}.

- {{domxref("GPURenderBundleEncoder.finish", "finish()")}} {{Experimental_Inline}}

  - : Completes recording of the current render pass command sequence.

- {{domxref("GPURenderBundleEncoder.insertDebugMarker", "insertDebugMarker()")}} {{Experimental_Inline}}
  - : Marks a specific point in a series of encoded commands with a label.
- {{domxref("GPURenderBundleEncoder.popDebugGroup", "popDebugGroup()")}} {{Experimental_Inline}}
  - : Ends a debug group, which is begun with a {{domxref("GPURenderBundleEncoder.pushDebugGroup", "pushDebugGroup()")}} call.
- {{domxref("GPURenderBundleEncoder.pushDebugGroup", "pushDebugGroup()")}} {{Experimental_Inline}}
  - : Begins a debug group, which is marked with a specified label, and will contain all subsequent encoded commands up until a {{domxref("GPURenderBundleEncoder.popDebugGroup", "popDebugGroup()")}} method is invoked.
- {{domxref("GPURenderBundleEncoder.setBindGroup", "setBindGroup()")}} {{Experimental_Inline}}

  - : Sets the {{domxref("GPUBindGroup")}} to use for subsequent render bundle commands, for a given index.

- {{domxref("GPURenderBundleEncoder.setIndexBuffer", "setIndexBuffer()")}} {{Experimental_Inline}}

  - : Sets the current {{domxref("GPUBuffer")}} that will provide index data for subsequent drawing commands.

- {{domxref("GPURenderBundleEncoder.setPipeline", "setPipeline()")}} {{Experimental_Inline}}

  - : Sets the {{domxref("GPURenderPipeline")}} to use for this render bundle.

- {{domxref("GPURenderBundleEncoder.setVertexBuffer", "setVertexBuffer()")}} {{Experimental_Inline}}
  - : Sets or unsets the current {{domxref("GPUBuffer")}} that will provide vertex data for subsequent drawing commands.

## Examples

In the WebGPU Samples [Animometer example](https://webgpu.github.io/webgpu-samples/samples/animometer), a lot of like operations are done on many different objects simultaneously. A bundle of commands is encoded using the following function:

```js
function recordRenderPass(
  passEncoder: GPURenderBundleEncoder | GPURenderPassEncoder
) {
  if (settings.dynamicOffsets) {
    passEncoder.setPipeline(dynamicPipeline);
  } else {
    passEncoder.setPipeline(pipeline);
  }
  passEncoder.setVertexBuffer(0, vertexBuffer);
  passEncoder.setBindGroup(0, timeBindGroup);
  const dynamicOffsets = [0];
  for (let i = 0; i < numTriangles; ++i) {
    if (settings.dynamicOffsets) {
      dynamicOffsets[0] = i * alignedUniformBytes;
      passEncoder.setBindGroup(1, dynamicBindGroup, dynamicOffsets);
    } else {
      passEncoder.setBindGroup(1, bindGroups[i]);
    }
    passEncoder.draw(3, 1, 0, 0);
  }
}
```

Later on, a `GPURenderBundleEncoder` is created, the function is invoked, and the command bundle is recorded into a {{domxref("GPURenderBundle")}} using {{domxref("GPURenderBundleEncoder.finish()")}}:

```js
const renderBundleEncoder = device.createRenderBundleEncoder({
  colorFormats: [presentationFormat],
});
recordRenderPass(renderBundleEncoder);
const renderBundle = renderBundleEncoder.finish();
```

{{domxref("GPURenderPassEncoder.executeBundles()")}} is then used to reuse the work across multiple render passes to improve performance. Study the example code listing for the full context.

```js
// ...

return function doDraw(timestamp) {
  if (startTime === undefined) {
    startTime = timestamp;
  }
  uniformTime[0] = (timestamp - startTime) / 1000;
  device.queue.writeBuffer(uniformBuffer, timeOffset, uniformTime.buffer);

  renderPassDescriptor.colorAttachments[0].view = context
    .getCurrentTexture()
    .createView();

  const commandEncoder = device.createCommandEncoder();
  const passEncoder = commandEncoder.beginRenderPass(renderPassDescriptor);

  if (settings.renderBundles) {
    passEncoder.executeBundles([renderBundle]);
  } else {
    recordRenderPass(passEncoder);
  }

  passEncoder.end();
  device.queue.submit([commandEncoder.finish()]);
};

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/popdebuggroup/index.md
---
title: "GPURenderBundleEncoder: popDebugGroup() method"
short-title: popDebugGroup()
slug: Web/API/GPURenderBundleEncoder/popDebugGroup
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder.popDebugGroup
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`popDebugGroup()`** method of the
{{domxref("GPURenderBundleEncoder")}} interface ends a render bundle debug group, which is begun with a {{domxref("GPURenderBundleEncoder.pushDebugGroup", "pushDebugGroup()")}} call.

This could be used for telemetry, or may be utilized in {{domxref("GPUError")}} messages, browser dev tools, or other services in the future to help with debugging.

> **Note:** This method is functionally identical to its equivalent on {{domxref("GPURenderPassEncoder")}} ‚Äî {{domxref("GPURenderPassEncoder.popDebugGroup", "popDebugGroup()")}}.

## Syntax

```js-nolint
popDebugGroup()
```

### Parameters

None.

### Return value

None ({{jsxref("Undefined")}}).

### Validation

The following criteria must be met when calling **`popDebugGroup()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderBundleEncoder")}} becomes invalid:

- The render bundle encoder's debug stack is not empty (i.e. at least one render bundle debug group was previously started with {{domxref("GPURenderBundleEncoder.pushDebugGroup", "pushDebugGroup()")}}).

## Examples

```js
// ...

const bundleEncoder = device.createRenderBundleEncoder(renderBundleDescriptor);

bundleEncoder.pushDebugGroup("mygroupmarker"); // Start labeled debug group

bundleEncoder.setPipeline(renderPipeline);
bundleEncoder.setVertexBuffer(0, vertexBuffer);
bundleEncoder.draw(3);

bundleEncoder.popDebugGroup();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/drawindexed/index.md
---
title: "GPURenderBundleEncoder: drawIndexed() method"
short-title: drawIndexed()
slug: Web/API/GPURenderBundleEncoder/drawIndexed
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder.drawIndexed
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`drawIndexed()`** method of the
{{domxref("GPURenderBundleEncoder")}} interface draws indexed primitives based on the vertex and index buffers provided by {{domxref("GPURenderBundleEncoder.setVertexBuffer", "setVertexBuffer()")}} and {{domxref("GPURenderBundleEncoder.setIndexBuffer", "setIndexBuffer()")}}.

> **Note:** This method is functionally identical to its equivalent on {{domxref("GPURenderPassEncoder")}} ‚Äî {{domxref("GPURenderPassEncoder.drawIndexed", "drawIndexed()")}}.

## Syntax

```js-nolint
drawIndexed(indexCount)
drawIndexed(indexCount, instanceCount)
drawIndexed(indexCount, instanceCount, firstIndex)
drawIndexed(indexCount, instanceCount, firstIndex, baseVertex)
drawIndexed(indexCount, instanceCount, firstIndex, baseVertex, firstInstance)
```

### Parameters

- `indexCount`
  - : A number defining the number of indices to draw.
- `instanceCount` {{optional_inline}}
  - : A number defining the number of instances to draw. If omitted, `instanceCount` defaults to 1.
- `firstIndex` {{optional_inline}}
  - : A number defining the offset into the index buffer, in indices, to begin drawing from. If omitted, `firstIndex` defaults to 0.
- `baseVertex` {{optional_inline}}
  - : A number added to each index value before indexing into the vertex buffers. If omitted, `baseVertex` defaults to 0.
- `firstInstance` {{optional_inline}}
  - : A number defining the first instance to draw. If omitted, `firstInstance` defaults to 0.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
// ...

const bundleEncoder = device.createRenderBundleEncoder(descriptor);

bundleEncoder.setPipeline(pipeline);
bundleEncoder.setBindGroup(0, sceneBindGroupForRender);
bundleEncoder.setBindGroup(1, modelBindGroup);
bundleEncoder.setVertexBuffer(0, vertexBuffer);
bundleEncoder.setIndexBuffer(indexBuffer, "uint16");
bundleEncoder.drawIndexed(indexCount);

const renderBundle = bundleEncoder.finish();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/finish/index.md
---
title: "GPURenderBundleEncoder: finish() method"
short-title: finish()
slug: Web/API/GPURenderBundleEncoder/finish
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder.finish
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`finish()`** method of the
{{domxref("GPURenderBundleEncoder")}} interface completes recording of the current render bundle command sequence, returning a {{domxref("GPURenderBundle")}} object that can be passed into a {{domxref("GPURenderPassEncoder.executeBundles()")}} call to execute those commands in a specific render pass.

## Syntax

```js-nolint
finish(descriptor)
```

### Parameters

- `descriptor` {{optional_inline}}
  - : An object containing the following properties:
    - `label` {{optional_inline}}
      - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

### Return value

A {{domxref("GPURenderBundle")}} object instance.

### Validation

The following criteria must be met when calling **`finish()`**, otherwise a {{domxref("GPUValidationError")}} is generated and the {{domxref("GPURenderBundleEncoder")}} becomes invalid:

- The {{domxref("GPURenderBundleEncoder")}} is open (i.e. not already ended via a `finish()` call).
- The debug stack for the current render pass is empty (i.e. no render pass debug group is currently open, as opened by {{domxref("GPURenderBundleEncoder.pushDebugGroup", "pushDebugGroup()")}}).

## Examples

```js
const renderBundleEncoder = device.createRenderBundleEncoder({
  colorFormats: [presentationFormat],
});
recordRenderPass(renderBundleEncoder);
const renderBundle = renderBundleEncoder.finish();
```

The above snippet is taken from the WebGPU Samples [Animometer example](https://webgpu.github.io/webgpu-samples/samples/animometer).

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/pushdebuggroup/index.md
---
title: "GPURenderBundleEncoder: pushDebugGroup() method"
short-title: pushDebugGroup()
slug: Web/API/GPURenderBundleEncoder/pushDebugGroup
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder.pushDebugGroup
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`pushDebugGroup()`** method of the
{{domxref("GPURenderBundleEncoder")}} interface begins a render bundle debug group, which is marked with a specified label, and will contain all subsequent encoded commands up until a {{domxref("GPURenderBundleEncoder.popDebugGroup", "popDebugGroup()")}} method is invoked.

This could be used for telemetry, or may be utilized in {{domxref("GPUError")}} messages, browser dev tools, or other services in the future to help with debugging.

> **Note:** This method is functionally identical to its equivalent on {{domxref("GPURenderPassEncoder")}} ‚Äî {{domxref("GPURenderPassEncoder.pushDebugGroup", "pushDebugGroup()")}}.

## Syntax

```js-nolint
pushDebugGroup(groupLabel)
```

### Parameters

- `groupLabel`
  - : A string representing the label for the debug group.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
// ...

const bundleEncoder = device.createRenderBundleEncoder(renderBundleDescriptor);

bundleEncoder.pushDebugGroup("mygroupmarker"); // Start labeled debug group

bundleEncoder.setPipeline(renderPipeline);
bundleEncoder.setVertexBuffer(0, vertexBuffer);
bundleEncoder.draw(3);

bundleEncoder.popDebugGroup();

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpurenderbundleencoder/draw/index.md
---
title: "GPURenderBundleEncoder: draw() method"
short-title: draw()
slug: Web/API/GPURenderBundleEncoder/draw
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPURenderBundleEncoder.draw
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`draw()`** method of the
{{domxref("GPURenderBundleEncoder")}} interface draws primitives based on the vertex buffers provided by {{domxref("GPURenderBundleEncoder.setVertexBuffer", "setVertexBuffer()")}}.

> **Note:** This method is functionally identical to its equivalent on {{domxref("GPURenderPassEncoder")}} ‚Äî {{domxref("GPURenderPassEncoder.draw", "draw()")}}.

## Syntax

```js-nolint
draw(vertexCount)
draw(vertexCount, instanceCount)
draw(vertexCount, instanceCount, firstVertex)
draw(vertexCount, instanceCount, firstVertex, firstInstance)
```

### Parameters

- `vertexCount`
  - : A number defining the number of vertices to draw.
- `instanceCount` {{optional_inline}}
  - : A number defining the number of instances to draw. If omitted, `instanceCount` defaults to 1.
- `firstVertex` {{optional_inline}}
  - : A number defining the offset into the vertex buffers, in vertices, to begin drawing from. If omitted, `firstVertex` defaults to 0.
- `firstInstance` {{optional_inline}}
  - : A number defining the first instance to draw. If omitted, `firstInstance` defaults to 0.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
function recordRenderPass(
  passEncoder: GPURenderBundleEncoder | GPURenderPassEncoder // TypeScript
) {
  if (settings.dynamicOffsets) {
    passEncoder.setPipeline(dynamicPipeline);
  } else {
    passEncoder.setPipeline(pipeline);
  }
  passEncoder.setVertexBuffer(0, vertexBuffer);
  passEncoder.setBindGroup(0, timeBindGroup);
  const dynamicOffsets = [0];
  for (let i = 0; i < numTriangles; ++i) {
    if (settings.dynamicOffsets) {
      dynamicOffsets[0] = i * alignedUniformBytes;
      passEncoder.setBindGroup(1, dynamicBindGroup, dynamicOffsets);
    } else {
      passEncoder.setBindGroup(1, bindGroups[i]);
    }
    passEncoder.draw(3, 1, 0, 0);
  }
}
```

The above snippet is taken from the WebGPU Samples [Animometer example](https://webgpu.github.io/webgpu-samples/samples/animometer).

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuuncapturederrorevent/index.md
---
title: GPUUncapturedErrorEvent
slug: Web/API/GPUUncapturedErrorEvent
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUUncapturedErrorEvent
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUUncapturedErrorEvent`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} is the event object type for the {{domxref("GPUDevice")}} {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event, used for telemetry and to report unexpected errors.

Known error cases should be handled using {{domxref("GPUDevice.pushErrorScope", "pushErrorScope()")}} and {{domxref("GPUDevice.popErrorScope", "popErrorScope()")}}.

{{InheritanceDiagram}}

## Constructor

- {{domxref("GPUUncapturedErrorEvent.GPUUncapturedErrorEvent", "GPUUncapturedErrorEvent()")}} {{Experimental_Inline}}
  - : Creates a new `GPUUncapturedErrorEvent` object instance.

## Instance properties

_Inherits properties from its parent, {{domxref("Event")}}._

- {{domxref("GPUUncapturedErrorEvent.error", "error")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A {{domxref("GPUError")}} object instance providing access to the details of the error.

## Examples

You could use something like the following as a global mechanism to pick up any errors that aren't handled by error scopes and capture them.

```js
// ...

device.addEventListener("uncapturederror", (event) => {
  // Re-surface the error
  console.error("A WebGPU error was not captured:", event.error.message);
  reportErrorToServer({
    type: event.error.constructor.name,
    message: event.error.message,
  });
});

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling)
-e 

File: /files/en-us/web/api/gpuuncapturederrorevent/gpuuncapturederrorevent/index.md
---
title: "GPUUncapturedErrorEvent: GPUUncapturedErrorEvent() constructor"
short-title: GPUUncapturedErrorEvent()
slug: Web/API/GPUUncapturedErrorEvent/GPUUncapturedErrorEvent
page-type: web-api-constructor
status:
  - experimental
browser-compat: api.GPUUncapturedErrorEvent.GPUUncapturedErrorEvent
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUUncapturedErrorEvent()`** constructor creates a new
{{domxref("GPUUncapturedErrorEvent")}} object instance.

## Syntax

```js-nolint
new GPUUncapturedErrorEvent(type, options)
```

### Parameters

- `type`
  - : An enumerated value specifying the type of error. Possible values are:
    - `"internal"`
      - : The error is a {{domxref("GPUInternalError")}}.
    - `"out-of-memory"`
      - : The error is a {{domxref("GPUOutOfMemoryError")}}.
    - `"validation"`
      - : The error is a {{domxref("GPUValidationError")}}.
- `options`
  - : An object, which can contain the following properties:
    - `error`
      - : A {{domxref("GPUError")}} object instance providing access to the details of the error.

## Examples

A developer would not manually use the constructor to create a `GPUUncapturedErrorEvent` object. The user agent uses this constructor to create an appropriate object when the {{domxref("GPUDevice")}} {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event fires to allow capturing of an unexpected error.

See the main [`GPUUncapturedErrorEvent`](/en-US/docs/Web/API/GPUUncapturedErrorEvent#examples) page for an example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling)
-e 

File: /files/en-us/web/api/gpuuncapturederrorevent/error/index.md
---
title: "GPUUncapturedErrorEvent: error property"
short-title: error
slug: Web/API/GPUUncapturedErrorEvent/error
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUUncapturedErrorEvent.error
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`error`** read-only property of the
{{domxref("GPUUncapturedErrorEvent")}} interface is a {{domxref("GPUError")}} object instance providing access to the details of the error.

## Value

A {{domxref("GPUError")}} object instance.

## Examples

See the main [`GPUUncapturedErrorEvent`](/en-US/docs/Web/API/GPUUncapturedErrorEvent#examples) page for an example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling)
-e 

File: /files/en-us/web/api/gpucompilationmessage/linenum/index.md
---
title: "GPUCompilationMessage: lineNum property"
short-title: lineNum
slug: Web/API/GPUCompilationMessage/lineNum
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUCompilationMessage.lineNum
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`lineNum`** read-only property of the
{{domxref("GPUCompilationMessage")}} interface is a number representing the line number in the shader code that the message corresponds to.

## Value

A number.

Note that:

- If the message corresponds to a substring, `lineNum` refers to the line number that the substring begins on.
- If the message does not correspond to a specific line of code (perhaps it refers to the whole of the shader code), `lineNum` will be 0.
- Values are one-based ‚Äî a value of 1 refers to the first line of code.
- Lines are delimited by line breaks. In WGSL, a [specific list of characters](https://gpuweb.github.io/gpuweb/wgsl/#line-break) is defined as line breaks.

## Examples

```js
  // ...
  const shaderModule = device.createShaderModule({
    code: shaders,
  });

  const shaderInfo = await shaderModule.getCompilationInfo();
  const firstMessage = shaderInfo.messages[0];
  console.log(firstMessage.lineNum);
  // ...
}
```

See the main [`GPUCompilationInfo` page](/en-US/docs/Web/API/GPUCompilationInfo#examples) for a more detailed example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucompilationmessage/length/index.md
---
title: "GPUCompilationMessage: length property"
short-title: length
slug: Web/API/GPUCompilationMessage/length
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUCompilationMessage.length
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`length`** read-only property of the
{{domxref("GPUCompilationMessage")}} interface is a number representing the length of the substring that the message corresponds to.

## Value

A number.

To be precise, `length` is the number of UTF-16 code units in the shader code substring that the message corresponds to. If the message corresponds to a single point rather than a substring, `length` will be 0.

## Examples

```js
  // ...
  const shaderModule = device.createShaderModule({
    code: shaders,
  });

  const shaderInfo = await shaderModule.getCompilationInfo();
  const firstMessage = shaderInfo.messages[0];
  console.log(firstMessage.length);
  // ...
}
```

See the main [`GPUCompilationInfo` page](/en-US/docs/Web/API/GPUCompilationInfo#examples) for a more detailed example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucompilationmessage/message/index.md
---
title: "GPUCompilationMessage: message property"
short-title: message
slug: Web/API/GPUCompilationMessage/message
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUCompilationMessage.message
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`message`** read-only property of the
{{domxref("GPUCompilationMessage")}} interface is a string representing human-readable message text.

## Value

A string.

## Examples

```js
  // ...
  const shaderModule = device.createShaderModule({
    code: shaders,
  });

  const shaderInfo = await shaderModule.getCompilationInfo();
  const firstMessage = shaderInfo.messages[0];
  console.log(firstMessage.message);
  // ...
}
```

See the main [`GPUCompilationInfo` page](/en-US/docs/Web/API/GPUCompilationInfo#examples) for a more detailed example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucompilationmessage/offset/index.md
---
title: "GPUCompilationMessage: offset property"
short-title: offset
slug: Web/API/GPUCompilationMessage/offset
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUCompilationMessage.offset
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`offset`** read-only property of the
{{domxref("GPUCompilationMessage")}} interface is a number representing the offset from the start of the shader code to the exact point, or the start of the relevant substring, that the message corresponds to.

## Value

A number.

To be precise, `offset` is the number of UTF-16 code units from the beginning of the shader code to the exact point or start of the relevant substring that the message corresponds to.

If the message does not correspond to a specific code position (perhaps it refers to the whole of the shader code), `offset` will be 0.

## Examples

```js
  // ...
  const shaderModule = device.createShaderModule({
    code: shaders,
  });

  const shaderInfo = await shaderModule.getCompilationInfo();
  const firstMessage = shaderInfo.messages[0];
  console.log(firstMessage.offset);
  // ...
}
```

See the main [`GPUCompilationInfo` page](/en-US/docs/Web/API/GPUCompilationInfo#examples) for a more detailed example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucompilationmessage/type/index.md
---
title: "GPUCompilationMessage: type property"
short-title: type
slug: Web/API/GPUCompilationMessage/type
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUCompilationMessage.type
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`type`** read-only property of the
{{domxref("GPUCompilationMessage")}} interface is an enumerated value representing the type of the message. Each type represents a different severity level.

## Value

A enumerated value. Possible values are:

- `"error"`
  - : A shader-creation error, which stops successful compilation.
- `"info"`
  - : A purely informative message, which is low severity.
- `"warning"`
  - : A warning about an issue that will not stop successful compilation, but merits attention by the developer. An example is usage of deprecated functions or syntax.

## Examples

```js
  // ...
  const shaderModule = device.createShaderModule({
    code: shaders,
  });

  const shaderInfo = await shaderModule.getCompilationInfo();
  const firstMessage = shaderInfo.messages[0];
  console.log(firstMessage.type);
  // ...
}
```

See the main [`GPUCompilationInfo` page](/en-US/docs/Web/API/GPUCompilationInfo#examples) for a more detailed example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucompilationmessage/index.md
---
title: GPUCompilationMessage
slug: Web/API/GPUCompilationMessage
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUCompilationMessage
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUCompilationMessage`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents a single informational, warning, or error message generated by the GPU shader module compiler.

An array of `GPUCompilationMessage` objects is available in the `messages` property of the {{domxref("GPUCompilationInfo")}} object accessed via {{domxref("GPUShaderModule.getCompilationInfo()")}}.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUCompilationMessage.length", "length")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A number representing the length of the substring that the message corresponds to.
- {{domxref("GPUCompilationMessage.lineNum", "lineNum")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A number representing the line number in the shader code that the message corresponds to.
- {{domxref("GPUCompilationMessage.linePos", "linePos")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A number representing the position in the code line that the message corresponds to. This could be an exact point, or the start of the relevant substring.
- {{domxref("GPUCompilationMessage.message", "message")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A string representing human-readable message text.
- {{domxref("GPUCompilationMessage.offset", "offset")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A number representing the offset from the start of the shader code to the exact point, or the start of the relevant substring, that the message corresponds to.
- {{domxref("GPUCompilationMessage.type", "type")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : An enumerated value representing the type of the message ‚Äî `"error"`, `"info"`, or `"warning"`.

## Examples

See the main [`GPUCompilationInfo` page](/en-US/docs/Web/API/GPUCompilationInfo#examples) for an example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpucompilationmessage/linepos/index.md
---
title: "GPUCompilationMessage: linePos property"
short-title: linePos
slug: Web/API/GPUCompilationMessage/linePos
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUCompilationMessage.linePos
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`linePos`** read-only property of the
{{domxref("GPUCompilationMessage")}} interface is a number representing the position in the code line that the message corresponds to. This could be an exact point, or the start of the relevant substring.

## Value

A number.

To be precise, `linePos` is the number of UTF-16 code units from the beginning of the line to the exact point or start of the relevant substring that the message corresponds to.

Note that:

- If the message corresponds to a substring, `linePos` refers to the first UTF-16 code unit of the substring.
- If the message does not correspond to a specific code position (perhaps it refers to the whole of the shader code), `linePos` will be 0.
- Values are one-based ‚Äî a value of 1 refers to the first code unit of the line.

## Examples

```js
  // ...
  const shaderModule = device.createShaderModule({
    code: shaders,
  });

  const shaderInfo = await shaderModule.getCompilationInfo();
  const firstMessage = shaderInfo.messages[0];
  console.log(firstMessage.linePos);
  // ...
}
```

See the main [`GPUCompilationInfo` page](/en-US/docs/Web/API/GPUCompilationInfo#examples) for a more detailed example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuerror/message/index.md
---
title: "GPUError: message property"
short-title: message
slug: Web/API/GPUError/message
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUError.message
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`message`** read-only property of the
{{domxref("GPUError")}} interface provides a human-readable message that explains why the error occurred.

## Value

A string.

## Examples

For usage examples of error objects based on `GPUError`, see:

- [`GPUDevice.popErrorScope`](/en-US/docs/Web/API/GPUDevice/popErrorScope#examples)
- [The `GPUDevice uncapturederror` event](/en-US/docs/Web/API/GPUDevice/uncapturederror_event#examples)
- {{domxref("GPUInternalError")}}, {{domxref("GPUOutOfMemoryError")}}, and {{domxref("GPUValidationError")}}

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling)
-e 

File: /files/en-us/web/api/gpuerror/index.md
---
title: GPUError
slug: Web/API/GPUError
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUError
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUError`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} is the base interface for errors surfaced by {{domxref("GPUDevice.popErrorScope")}} and the {{domxref("GPUDevice.uncapturederror_event", "uncapturederror")}} event.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUError.message", "message")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A string providing a human-readable message that explains why the error occurred.

## Examples

For usage examples of error objects based on `GPUError`, see:

- [`GPUDevice.popErrorScope`](/en-US/docs/Web/API/GPUDevice/popErrorScope#examples)
- [The `GPUDevice uncapturederror` event](/en-US/docs/Web/API/GPUDevice/uncapturederror_event#examples)
- {{domxref("GPUInternalError")}}, {{domxref("GPUOutOfMemoryError")}}, and {{domxref("GPUValidationError")}}

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
- [WebGPU Error Handling best practices](https://toji.dev/webgpu-best-practices/error-handling)
-e 

File: /files/en-us/web/api/gpuexternaltexture/label/index.md
---
title: "GPUExternalTexture: label property"
short-title: label
slug: Web/API/GPUExternalTexture/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUExternalTexture.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** property of the
{{domxref("GPUExternalTexture")}} interface provides a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUDevice.importExternalTexture()")}} call, or you can get and set it directly on the `GPUExternalTexture` object.

## Value

A string. If this has not been previously set as described above, it will be an empty string.

## Examples

Setting and getting a label via `GPUExternalTexture.label`:

```js
// ...

const externalTexture = device.importExternalTexture({
  source: video,
});

externalTexture.label = "myExtTexture";

console.log(externalTexture.label); // "myExtTexture"
```

Setting a label via the originating {{domxref("GPUDevice.importExternalTexture()")}} call, and then getting it via `GPUExternalTexture.label`:

```js
// ...

const externalTexture = device.importExternalTexture({
  source: video,
  label: "myExtTexture",
});

console.log(externalTexture.label); //  "myExtTexture"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuexternaltexture/index.md
---
title: GPUExternalTexture
slug: Web/API/GPUExternalTexture
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUExternalTexture
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUExternalTexture`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents a wrapper object containing an {{domxref("HTMLVideoElement")}} snapshot that can be used as a texture in GPU rendering operations.

A `GPUExternalTexture` object instance is created using {{domxref("GPUDevice.importExternalTexture()")}}.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUExternalTexture.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Examples

In the WebGPU samples [Video Uploading sample](https://webgpu.github.io/webgpu-samples/samples/videoUploading), a `GPUExternalTexture` object (created via a {{domxref("GPUDevice.importExternalTexture()")}} call) is used as the value of a bind group entry `resource`, specified when creating a {{domxref("GPUBindGroup")}} via a {{domxref("GPUDevice.createBindGroup()")}} call:

```js
//...
const uniformBindGroup = device.createBindGroup({
  layout: pipeline.getBindGroupLayout(0),
  entries: [
    {
      binding: 1,
      resource: sampler,
    },
    {
      binding: 2,
      resource: device.importExternalTexture({
        source: video,
      }),
    },
  ],
});
//...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpubindgrouplayout/label/index.md
---
title: "GPUBindGroupLayout: label property"
short-title: label
slug: Web/API/GPUBindGroupLayout/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUBindGroupLayout.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** property of the
{{domxref("GPUBindGroupLayout")}} interface provides a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUDevice.createBindGroupLayout()")}} call, or you can get and set it directly on the `GPUBindGroupLayout` object.

## Value

A string. If this has not been previously set as described above, it will be an empty string.

## Examples

Setting and getting a label via `GPUBindGroupLayout.label`:

```js
// ...

const bindGroupLayout = device.createBindGroupLayout({
  entries: [
    {
      binding: 0,
      visibility: GPUShaderStage.COMPUTE,
      buffer: {
        type: "storage",
      },
    },
  ],
});

bindGroupLayout.label = "mybindgrouplayout";

console.log(bindGroupLayout.label); // "mybindgrouplayout";
```

Setting a label via the originating {{domxref("GPUDevice.createBindGroupLayout()")}} call, and then getting it via `GPUBindGroupLayout.label`:

```js
// ...

const bindGroupLayout = device.createBindGroupLayout({
  entries: [
    {
      binding: 0,
      visibility: GPUShaderStage.COMPUTE,
      buffer: {
        type: "storage",
      },
    },
  ],
  label: "mybindgrouplayout",
});

console.log(bindGroupLayout.label); // "mybindgrouplayout";
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpubindgrouplayout/index.md
---
title: GPUBindGroupLayout
slug: Web/API/GPUBindGroupLayout
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUBindGroupLayout
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUBindGroupLayout`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} defines the structure and purpose of related GPU resources such as buffers that will be used in a pipeline, and is used as a template when creating {{domxref("GPUBindGroup")}}s.

A `GPUBindGroupLayout` object instance is created using the {{domxref("GPUDevice.createBindGroupLayout()")}} method.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUBindGroupLayout.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Examples

> **Note:** The [WebGPU samples](https://webgpu.github.io/webgpu-samples/) feature many more examples.

### Basic example

Our [basic compute demo](https://mdn.github.io/dom-examples/webgpu-compute-demo/) shows an example of creating a bind group layout and then using that as a template when creating a bind group.

```js
// ...

const bindGroupLayout = device.createBindGroupLayout({
  entries: [
    {
      binding: 0,
      visibility: GPUShaderStage.COMPUTE,
      buffer: {
        type: "storage",
      },
    },
  ],
});

const bindGroup = device.createBindGroup({
  layout: bindGroupLayout,
  entries: [
    {
      binding: 0,
      resource: {
        buffer: output,
      },
    },
  ],
});

// ...
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpushadermodule/getcompilationinfo/index.md
---
title: "GPUShaderModule: getCompilationInfo() method"
short-title: getCompilationInfo()
slug: Web/API/GPUShaderModule/getCompilationInfo
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUShaderModule.getCompilationInfo
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`getCompilationInfo()`** method of the
{{domxref("GPUShaderModule")}} interface returns a {{jsxref("Promise")}} that fulfills with a {{domxref("GPUCompilationInfo")}} object containing messages generated during the `GPUShaderModule`'s compilation.

## Syntax

```js-nolint
getCompilationInfo()
```

### Parameters

None.

### Return value

A {{jsxref("Promise")}} that fulfills with a {{domxref("GPUCompilationInfo")}} object.

{{domxref("GPUCompilationInfo")}} contains a `messages` property, which is an array of {{domxref("GPUCompilationMessage")}} objects, each one containing the details of an individual compilation message.

## Examples

In the example below, we have deliberately left a parenthesis out of a function declaration in our shader code:

```js
const shaders = `
struct VertexOut {
  @builtin(position) position : vec4f,
  @location(0) color : vec4f
}

@vertex
fn vertex_main(@location(0) position: vec4f,
               @location(1) color: vec4f -> VertexOut
{
  var output : VertexOut;
  output.position = position;
  output.color = color;
  return output;
}

@fragment
fn fragment_main(fragData: VertexOut) -> @location(0) vec4f
{
  return fragData.color;
}
`;
```

When we compile the shader module, we use `getCompilationInfo()` to grab some information about the resulting error:

```js
async function init() {
  // ...

  const shaderModule = device.createShaderModule({
    code: shaders,
  });

  const shaderInfo = await shaderModule.getCompilationInfo();
  const firstMessage = shaderInfo.messages[0];

  console.log(firstMessage.lineNum); // 9
  console.log(firstMessage.message); // "expected ')' for function declaration"
  console.log(firstMessage.type); // "error"

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpushadermodule/label/index.md
---
title: "GPUShaderModule: label property"
short-title: label
slug: Web/API/GPUShaderModule/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUShaderModule.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** property of the
{{domxref("GPUShaderModule")}} interface provides a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUDevice.createShaderModule()")}} call, or you can get and set it directly on the `GPUShaderModule` object.

## Value

A string. If this has not been previously set as described above, it will be an empty string.

## Examples

Setting and getting a label via `GPUShaderModule.label`:

```js
// ...

const shaderModule = device.createShaderModule({
  code: shaders,
});

shaderModule.label = "myshader";

console.log(shaderModule.label); // "myshader"
```

Setting a label via the originating {{domxref("GPUDevice.createShaderModule()")}} call, and then getting it via `GPUShaderModule.label`:

```js
// ...

const shaderModule = device.createShaderModule({
  code: shaders,
  label: "myshader",
});

console.log(shaderModule.label); // "myshader"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpushadermodule/index.md
---
title: GPUShaderModule
slug: Web/API/GPUShaderModule
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUShaderModule
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUShaderModule`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} represents an internal shader module object, a container for [WGSL](https://gpuweb.github.io/gpuweb/wgsl/) shader code that can be submitted to the GPU for execution by a pipeline.

A `GPUShaderModule` object instance is created using {{domxref("GPUDevice.createShaderModule()")}}.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUShaderModule.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

## Instance methods

- {{domxref("GPUShaderModule.getCompilationInfo", "getCompilationInfo()")}} {{Experimental_Inline}}
  - : Returns a {{jsxref("Promise")}} that fulfills with a {{domxref("GPUCompilationInfo")}} object containing messages generated during the `GPUShaderModule`'s compilation.

## Examples

In our [basic render demo](https://mdn.github.io/dom-examples/webgpu-render-demo/), our shader module is created using the following code:

```js
const shaders = `
struct VertexOut {
  @builtin(position) position : vec4f,
  @location(0) color : vec4f
}

@vertex
fn vertex_main(@location(0) position: vec4f,
               @location(1) color: vec4f) -> VertexOut
{
  var output : VertexOut;
  output.position = position;
  output.color = color;
  return output;
}

@fragment
fn fragment_main(fragData: VertexOut) -> @location(0) vec4f
{
  return fragData.color;
}
`;

async function init() {
  if (!navigator.gpu) {
    throw Error("WebGPU not supported.");
  }

  const adapter = await navigator.gpu.requestAdapter();

  if (!adapter) {
    throw Error("Couldn't request WebGPU adapter.");
  }

  let device = await adapter.requestDevice();

  // ...
  // later on

  const shaderModule = device.createShaderModule({
    code: shaders,
  });

  // ...
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuqueryset/destroy/index.md
---
title: "GPUQuerySet: destroy() method"
short-title: destroy()
slug: Web/API/GPUQuerySet/destroy
page-type: web-api-instance-method
status:
  - experimental
browser-compat: api.GPUQuerySet.destroy
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`destroy()`** method of the
{{domxref("GPUQuerySet")}} interface destroys the `GPUQuerySet`.

## Syntax

```js-nolint
destroy()
```

### Parameters

None.

### Return value

None ({{jsxref("Undefined")}}).

## Examples

```js
const querySet = device.createQuerySet({
  type: "occlusion",
  count: 32,
});

// Some time later

querySet.destroy();
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuqueryset/count/index.md
---
title: "GPUQuerySet: count property"
short-title: count
slug: Web/API/GPUQuerySet/count
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUQuerySet.count
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`count`** read-only property of the
{{domxref("GPUQuerySet")}} interface is a number specifying the number of queries managed by the `GPUQuerySet`.

## Value

A number.

## Examples

See the main [`GPUQuerySet`](/en-US/docs/Web/API/GPUQuerySet#examples) page for an example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuqueryset/label/index.md
---
title: "GPUQuerySet: label property"
short-title: label
slug: Web/API/GPUQuerySet/label
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUQuerySet.label
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`label`** property of the
{{domxref("GPUQuerySet")}} interface is a string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.

This can be set by providing a `label` property in the descriptor object passed into the originating {{domxref("GPUDevice.createQuerySet()")}} call, or you can get and set it directly on the `GPUQuerySet` object.

## Value

A string. If this has not been previously set as described above, it will be an empty string.

## Examples

Setting and getting a label via `GPUQuerySet.label`:

```js
const querySet = device.createQuerySet({
  type: "occlusion",
  count: 32,
});

querySet.label = "myqueryset";

console.log(querySet.label); // "myqueryset"
```

Setting a label via the originating {{domxref("GPUDevice.createQuerySet()")}} call, and then getting it via `GPUQuerySet.label`:

```js
const querySet = device.createQuerySet({
  type: "occlusion",
  count: 32,
  label: "myqueryset",
});

console.log(querySet.label); // "myqueryset"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuqueryset/type/index.md
---
title: "GPUQuerySet: type property"
short-title: type
slug: Web/API/GPUQuerySet/type
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.GPUQuerySet.type
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`type`** read-only property of the
{{domxref("GPUQuerySet")}} interface is an enumerated value specifying the type of queries managed by the `GPUQuerySet`.

## Value

An enumerated value. Possible values are:

- `"occlusion"`
  - : The `GPUQuerySet` manages occlusion queries.
- `"timestamp"`
  - : The `GPUQuerySet` manages timestamp queries.

## Examples

See the main [`GPUQuerySet`](/en-US/docs/Web/API/GPUQuerySet#examples) page for an example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

File: /files/en-us/web/api/gpuqueryset/index.md
---
title: GPUQuerySet
slug: Web/API/GPUQuerySet
page-type: web-api-interface
status:
  - experimental
browser-compat: api.GPUQuerySet
---

{{APIRef("WebGPU API")}}{{SeeCompatTable}}

The **`GPUQuerySet`** interface of the {{domxref("WebGPU API", "WebGPU API", "", "nocode")}} is used to record the results of queries on passes, such as occlusion or timestamp queries.

- Occlusion queries are available on render passes to query whether any fragment samples pass all the per-fragment tests for a set of drawing commands (including scissor, sample mask, alpha to coverage, stencil, and depth tests). To run an occlusion query, an appropriate `GPUQuerySet` must be provided as the value of the `occlusionQuerySet` descriptor property when invoking {{domxref("GPUCommandEncoder.beginRenderPass()")}} to run a render pass.

- Timestamp queries allow applications to write timestamps to a `GPUQuerySet`. To run a timestamp query, appropriate `GPUQuerySet`s must be provided inside the value of the `timestampWrites` descriptor property when invoking {{domxref("GPUCommandEncoder.beginRenderPass()")}} to run a render pass, or {{domxref("GPUCommandEncoder.beginComputePass()")}} to run a compute pass. Alternatively, you can run a single timestamp query at any time by invoking {{domxref("GPUCommandEncoder.writeTimeStamp()")}} with an appropriate `GPUQuerySet` as a parameter.

> **Note:** To use timestamp queries, the `timestamp-query` {{domxref("GPUSupportedFeatures", "feature", "", "nocode")}} must be enabled in the {{domxref("GPUDevice")}}.

A `GPUQuerySet` object instance is created using the {{domxref("GPUDevice.createQuerySet()")}} method.

{{InheritanceDiagram}}

## Instance properties

- {{domxref("GPUQuerySet.count", "count")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : A number specifying the number of queries managed by the `GPUQuerySet`.
- {{domxref("GPUQuerySet.label", "label")}} {{Experimental_Inline}}
  - : A string providing a label that can be used to identify the object, for example in {{domxref("GPUError")}} messages or console warnings.
- {{domxref("GPUQuerySet.type", "type")}} {{Experimental_Inline}} {{ReadOnlyInline}}
  - : An enumerated value specifying the type of queries managed by the `GPUQuerySet`.

## Instance methods

- {{domxref("GPUQuerySet.destroy", "destroy()")}} {{Experimental_Inline}}
  - : Destroys the `GPUQuerySet`.

## Examples

The following snippet creates a `GPUQuerySet` that holds 32 occlusion query results, and then returns the `type` and `count`:

```js
const querySet = device.createQuerySet({
  type: "occlusion",
  count: 32,
});

console.log(querySet.count); // 32
console.log(querySet.type); // "occlusion"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The [WebGPU API](/en-US/docs/Web/API/WebGPU_API)
-e 

