# Simple opa-wasm node typescript application

The application is in [app.ts](./app.ts) and shows loading a `*.wasm` file,
initializing the policy, and evaluating it with input.

## Install dependencies

```bash
npm install
```

## Build the WebAssembly binary for the example policy

There is an example policy included with the example, see
[example.rego](./example.rego)

> Requires OPA v1.1.0+

```bash
npm run build
```

## Run the example Node JS code that invokes the Wasm binary:

```bash
npm start -- '{"message": "world"}'
```

```bash
npm start -- '{"message": "not-world"}'
```
