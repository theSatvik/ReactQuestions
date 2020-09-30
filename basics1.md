1 When to use a Class Component over a Function Component?

If the component needs state or lifecycle methods then use class component otherwise use function component. However, from React 16.8 with
the addition of Hooks, you could use state , lifecycle methods and other
features that were only available in class component right in your function
component

2 What are Pure Components?

React.PureComponent is exactly the same as React.Component except
that it handles the shouldComponentUpdate() method for you. When
props or state changes, PureComponent will do a shallow comparison on
both props and state. Component on the other hand won’t compare current props and state to next out of the box. Thus, the component will
re-render by default whenever shouldComponentUpdate is called

3What is state in React?

State of a component is an object that holds some information that may
change over the lifetime of the component. We should always try to make
our state as simple as possible and minimize the number of stateful components. Let’s create an user component with message state,
“‘jsx harmony class User extends React.Component { constructor(props)
{ super(props)
this.state = {
message: 'Welcome to React world'
}
}
render() { return (
<h1>{this.state.message}</h1>
</div>
)
} } “‘
State is similar to props, but it is private and fully controlled by the
component. i.e, It is not accessible to any component other than the one
that owns and sets it.

4 What are props in React?

Props are inputs to components. They are single values or objects containing a set of values that are passed to components on creation using a
naming convention similar to HTML-tag attributes. They are data passed
down from a parent component to a child component.
The primary purpose of props in React is to provide following component
functionality:
1. Pass custom data to your component.
2. Trigger state changes.
3. Use via this.props.reactProp inside component’s render()
method.
For example, let us create an element with reactProp property:
jsx harmony <Element reactProp={'1'} />
This reactProp (or whatever you came up with) name then becomes a
property attached to React’s native props object which originally already
exists on all components created using React library.
props.reactProp

5 What is the difference between state and props?

Both props and state are plain JavaScript objects. While both of them
hold information that influences the output of render, they are different
in their functionality with respect to component. Props get passed to
the component similar to function parameters whereas state is managed
within the component similar to variables declared within a function.
