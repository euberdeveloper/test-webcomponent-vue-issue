# test-webcomponent-vue-issue
A repo that reproduces an issue of a webcomponent made with Vue.js 2. The issue is with the rem font sizes, when the tag &lt;html> has a different font style from 16px

## Build

### The dist folder is already included

The `dist` folder is already included, you could just start an http server on dist (`cd dist && npx http-server .`) and open the page in your browser.

### You can build the project on your own

* `npm install`
* `npm run build`
* `cd dist && npx http-server .`

## Reproduction

Open the webpage in your browser. The view should look in a certain way.
After that, **change the `<html>` tag to have a different font-style, let's say `font-size: 9px`**. The view should look very different now.

The point is that there is already this piece of code here:

```scss
// This is because vuetify uses rem, so to make it behave everywhere the same I set the root font-size
:host {
  font-size: 100px !important;
}
```

but it seems completely being ignored.
