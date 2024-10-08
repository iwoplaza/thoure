<div align="center">

![phoure (light mode)](/public/phoure-logo-light.svg#gh-light-mode-only)
![phoure (dark mode)](/public/phoure-logo-dark.svg#gh-dark-mode-only)

Ethical AI upscaling for games. _(formerly "mender")_

</div>

<div align="center">
<div style="max-width: 640px">

![hello](/public/phoure-app.png)

</div>
</div>

## What does it do?

It upscales an image by a factor of $4$ (1K → 4K, etc.) with a minimal hit to performance.
For the renderer implemented in the official example, it produces a $2024\times2024$ image ~12 times faster than targeting $2024\times2024$ directly.

## Ethical?

The dataset that was used to train the upscaling neural network was generated with Blender's Geometry Nodes. **No artist's work was used in the process**.

## Roadmap

- [x] Generate procedural data-set with Blender Geometry Nodes.
- [x] Create a slim network architecture.
- [x] Train the network.
- [x] Create ray marching renderer (for SDFs).
- [x] Implement inference on the WebGPU.
- [ ] Extract into a separate package, to be used as an upscaling step in other WebGPU projects.
- [ ] Create rasterizing renderer (polygonal geometry).

## Development

### Local setup

- Install Node.js
- Install pnpm
- Run `pnpm install` to install all dependencies
- Run `pnpm dev` to run the development server, making the web app available via the web browser.
