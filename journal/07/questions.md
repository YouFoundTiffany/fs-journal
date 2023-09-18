# Managing the Fullstack Application

1. Describe the two ways to bind Data in Vue?

  > One Way Binding, Two Way Binding

2. The `SPA` acronym stands for what?

  > Single Page Application

3. What are some of the advantages/uses of a `SPA` over a traditional one?

  > Fast, instant, hardly any wait time
Easily debuggable
Good user experience

4. What does the `onMounted` method in Vue do?

  > It is a lifecycle hook. Lifecycle hooks are a window into how the library you’re using works behind-the-scenes. Lifecycle hooks allow you to know when your component is created, added to the DOM, updated, or destroyed.


5. What is the `v-model` attribute in Vue for, and when might you use it?

  > By default, v-model on a component uses modelValue as the prop and update:modelValue as the event. We can modify these names passing an argument to v-model:

6. What is the package.json file used for?

  > The package. json file contains descriptive and functional metadata about a project, such as a name, version, and dependencies. The file provides the npm package manager with various information to help identify the project and handle dependencies.

7. Which Vue attributes(directives) could you use to conditionally render elements on a page?

  > v-if

8. What is the purpose of the `key` attribute when using `v-for` on an element?

  > The key attribute is used with the v-for directive so that Vue can tell the elements apart properly. Vue optimizes performance by reusing elements. So when elements are created from an array with v-for , if the key attribute is NOT used, element properties can be mixed when the array gets modified.

9. What is the `<slot>` element and what is it used for?

  > The <slot> element is a slot outlet that indicates where the parent-provided slot content should be rendered. With slots, the <FancyButton> is responsible for rendering the outer <button> (and its fancy styling), while the inner content is provided by the parent component.
