# noop-swagger-ui-dist
> A noop swagger-ui-dist used to remove it from lambda bundle

## Motivation

hapi-swagger [requires](https://github.com/glennjones/hapi-swagger/blob/v14.2.4/lib/index.js#L7) swagger-ui-dist to exist in the lambda bundle.

We want to save space and remove it from the bundle.

## Usage

Add thie resolution to your package.json and install with yarn:

```json
{
  "resolutions": {
    "swagger-ui-dist": "https://github.com/tepez/noop-swagger-ui-dist"
  }
}
```