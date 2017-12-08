# Vue.js tabs component styled with Bulma
##### A Vue.js Tabs component using the bulma css framework.

## How it works?

Well, like any vue component you will nedd to register it in your app js file.
```js
Vue.component('tabs', require('./components/Tabs.vue'));
Vue.component('tab', require('./components/Tab.vue'));
```

And in your views you just wrap as many tab components as you wish inside the tabs component, like so:

```html
<tabs>
  <tab></tab>
  <tab></tab>
  <tab></tab>
</tabs>
```

## There are 2 things required on the tab component, as its main API.
1. **name**:this is the regular html name attribute, as i implemented this as a prop for the tab component.
2. **selected**: You can put this on one or more tab component and bind it, this will visualise and tell the the user what tab isselected:
```html
<tab name"MyTab" :selected="true"></tab>
```

And this is it really, nice and simple.
