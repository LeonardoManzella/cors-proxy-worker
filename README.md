# CORS proxy worker

An online CORS proxy using Cloudflare Workers to expose as a consumible service wich adds necessary CORS headers to a third party API response
Created using Cloudflare Worker

## How to use

A specific working example (with url of worker changed) could be :

```
    let fetchedResponse =  fetch("https://my-worker-path.workers.dev/corsproxy/?apiurl=https://api.to.call).then(function(d) {return d.json()});
```

## Technology

The project uses the following libraries:

- Node.js
- Wrangler
- Prettier
- JsHint
- HTTP Headers API

## Serverless

To deploy using serverless add a [`serverless.yml`](https://serverless.com/framework/docs/providers/cloudflare/) file.
