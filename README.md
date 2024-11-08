# egui-web-minimal

Here is a minimal example of deploying egui to the web with WASM

Take a good read here: <https://rustwasm.github.io/docs/book/introduction.html>

You will need `wasm-pack` to then

```shell
wasm-pack build
```

to nicely have target artifacts inside `pkg` folder.

Then, use the templates from <https://github.com/rustwasm/create-wasm-app> or just your own.

The only thing you have to do to make egui render is adding a `<canvas>` tag inside your HTML with an ID.

Then, with the example code from eframe (as of 0.29.1) <https://docs.rs/eframe/latest/eframe/#usage-web>, you will start an instance of `WebHandle` with the `<canvas>` ID.
