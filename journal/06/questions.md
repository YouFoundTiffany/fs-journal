# Single Page Applications with Vue
01. What is the entrypoint of an application?

  > main.js

02. What is the difference between a vue `component` and `page`?

  > Technically they have the same capabilities. The difference is in usage and how they are organized in folder hierarchy. For now, our directive is to use pages for navigation and components to be displayed on a page. Mostly... :D

03. What is ***Component-Based Architecture***?

  > a framework for organizing a software with reusable components, vs large unmanageable files wherein elements are inaccessible.

04. What are the three tags that make up a Vue component?

  > template script and style

05. What are ***lifecycle hooks***? What are lifecycle hooks used for?

  > Lifecycle hooks in Vue are certain stages in the lifecycle of a component where we can add code to do things. Every time a component reaches a new stage in its lifecycle, a specific function runs, and we can add code to that function. Such functions are called lifecycle hooks, because we can "hook" our code into that stage.
  These are all the lifecycle hooks a component has:

beforeCreate
created
beforeMount
mounted
beforeUpdate
updated
beforeUnmount
unmounted
errorCaptured
renderTracked
renderTriggered
activated
deactivated
serverPrefetch

06. Which component in Vue does the vue-router use to mount pages onto?

  > pages are mounted in the router.js file, in the routes array.
  const routes = [
  {
    path: '/',
    name: 'Home',
    component: loadPage('HomePage')
  },

07. What is the difference between the `AppState` and the state object within a component?

  > Each component has its own. The AppState utilizes the observer pattern and a single source of truth for all components in the app using vue's reactive wrapper.

08. What is the responsibility of `Services` in our Vue projects?

  > Same as it is in the MVCs framework.

09. What are ***props*** and how are they used? Provide an example

  > Props are how we pass variables and other information around between different components. To use props, you pass props to another component, and that component can then use that value.

  export default {
  props: {car: {type: Car, required: true}},

10. What is the Vue method used to create watchable objects such as `state` or `AppState`?

  > watchEffect()