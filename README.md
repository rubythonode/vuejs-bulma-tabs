# Vue.js tabs component styled with Bulma
##### A Vue.js Tabs component using the bulma css framework.

## How it works?

Well, like any vue component you will nedd to register it in your app js file.
```js
Vue.component('tabs', require('./path/to/your/component/Tabs.vue'));
Vue.component('tab', require('./path/to/your/component/Tab.vue'));
```

And in your views you just wrap as many tab components as you wish inside the tabs component, like so:

```html
<tabs>
  <tab></tab>
  <tab></tab>
  <tab></tab>
</tabs>
```

#### There are 2 things required on the tab component, as its main API.
1. **name**: This is the regular html name attribute, as i implemented this as a prop for the tab component.
2. **selected**: You can put this on one or more tab component and bind it, this will visualise and tell the the user what tab is selected:
```html
<tab name"MyTab" :selected="true"></tab>
```

The finished thing should be like this:

```html
<tabs>
  <tab name"MyTab1" :selected="true">
    Content of tab goes here.
  </tab>
  <tab name"MyTab2">
    Content of tab goes here.
  </tab>
  <tab name"MyTab3">
   Content of tab goes here.
  </tab>
</tabs>
```
And this is it really, nice and simple.
