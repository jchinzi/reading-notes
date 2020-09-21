### Questions:

**Why do we not need more .html pages in a multi-page React app?**

Rather than rendering completely different .html pages, routing in a React app instead renders the appropriate JS components (which may or may not be reused from one page to the next)

**If we wanted a component to show up on every page, where would we put it and why?
Outside the <BrowserRouter/>
*Inside the <BrowserRouter />, outside a <Route />*
Inside a <Route />**

In this case, we would want to put it inside the <BrowserRouter />, outside a <Route />.
We would do it this way because when using <BrowserRouter />, those tags need to encompass everthing that is being rendered.  However, by not tying it to a particular route it will therefore render for all views/routes.  (For example, we might do this with headers and footers that we want to be persistent throughout the app)

*Source: RESTy App, Week 5 Project*

**What does props.children contain?**

props.children contains whatever code is written between the opening and closing tags of that component.  In order to use this feature, the component must be invoked using full opening and closing tags rather than a self-closing tag.

*Source: https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891*

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|composition|A natural pattern of the component model, or how we build components from other components|https://dev.to/bouhm/thinking-in-react-component-composition-fp5#:~:text=What%20is%20Composition%3F,in%20building%20many%20other%20components.|
|Children / Child Components|A child component takes props from its parent component and is within that parents scope|https://stackoverflow.com/questions/44092105/what-is-the-difference-between-child-and-parent-component-in-angular-2#:~:text=A%20child%20component%20is%20a%20more%20specific%20part%20inside%20a,are%20child%20components%20of%20it.|
|Hash Routing|A <Router> that uses the hash portion of the URL to keep your UI in sync with the URL|https://reactrouter.com/web/api/HashRouter|
|Link Routing|One way to navigate around an app - a <Link> can know when a route it links to is active and then automatically apply an activeClassName and/or activeStyle when given either prop.|https://knowbody.github.io/react-router-docs/api/Link.html|

---

[Home](https://jchinzi.github.io/reading-notes/)