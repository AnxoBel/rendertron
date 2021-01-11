# Rendertron cookies-support branch
For the original README, check [README.original.md](./README.original.md).

This branch adds support for cookies injection.

Only new code was added in a way that no break in the original code should happen. Building steps remain the same.

## How to use it

Create in the main directory a file called `cookies.json`. It expects a list of objects that follow the [Puppeteer specification](https://github.com/puppeteer/puppeteer/blob/v1.17.0/docs/api.md#pagesetcookiecookies). For example:

```
[
  {
    "name": "cookie1",
    "value": "some-value",
    "domain": ".example.com"
  },
  {
    "name": "cookie2",
    "value": "test"
  }
]

```
