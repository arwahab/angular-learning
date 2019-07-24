# Learning Angular

### Following this: https://angular.io/start

How `Templates` work:


- Angular's template syntax extends HTML and JavaScript
  * Ex: template file: `product-list.component.html`

- Directives -  We can use the `*ngFor directive` to have each product in the list to be displayed the same way, one after the other on the page. 
    * `*ngFor` causes the `<div>` to be repeated for each product in the list.
    * `*ngFor` is a "structural directive".  
    
    * Structural directives shape or reshape the DOM's structure, typically by adding, removing, and manipulating the elements to which they are attached. 
    
    * Any directive with an `*` is a structural directive.

- To display the names of the products, use the interpolation syntax `{{ }}`. 
- Interpolation renders a property's value as text.
- Interpolation `{{ }}` lets you render the property value as text; property binding `[ ]`lets you use the property value in a template expression.
-  Event binding is done by using `( )` around the event.
- Angular's template syntax:
    *   `*ngFor`
    *   `*ngIf`
    *   `Interpolation {{ }}`
    *   `Property binding [ ]`
    *   `Event binding ( )`
---------------------------------------------------------------------------------------------- 

How `Components` work:

- Components define areas of responsibility in your UI that let you reuse these sets of UI functionality.
- A component is comprised of three things:
    * 1- A `component class`, which handles data and functionality. Ex: the product data and the share() method were defined in the component class.
    * 2- An `HTML template`, which determines what is presented to the user. In the previous section, we modified the product list's HTML template to display the name, description, and a "Share" button for each product.

- Component-specific styles define the look and feel. The product list does not define any styles.

- An Angular application is composed of a `tree of components`, in which each Angular component has a specific purpose and responsibility.

- The `@Component` indicates that the following class is a component. It provides metadata about the component, such as: 
    *  `templates`, 
    *   `styles`, 
    *    and  `selector`

- The `@Input` decorator indicates that the property value will be passed in from the component's parent (in this case, the product list component).
---------------------------------------------------------------------------------------------- 

How `Routing` works:

- To do `routing` we need to use the Angular `router`. 
- The Angular `router` enables us to show different components and data to the user based on where the user is in the application. 
- The `router` enables navigation from one view to the next as users perform application tasks like:

    *   Enter a URL in the address bar, and the browser navigates to a corresponding page.
    *   Click links on the page, and the browser navigates to a new page.
    *   Click the browser's back and forward buttons, and the browser navigates backward and forward        through the history of pages you've seen.

- `app.module.ts` is where we can register a route.
- 

