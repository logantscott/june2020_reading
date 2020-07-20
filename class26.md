[Table of Contents](https://github.com/logantscott/june2020_reading)

# Component Based UI  

## Webpack  
Webpack basically combines separate template part files into a single file to be handled by the browser, as well as minifying a bit of the code to reduce overhead.

## React  

### JSX  
JSX extends javascript, and can be used by react to help with easy to read code, especially combining functions/logic and html.
```const element = <h1>Hello, world!</h1>;```

### Rendering  
Using the render method of react, you pass two arguments, the jsx and the root element to render to (usually an html page with a single element w/ id 'root').
```<div id="root"></div>```
```
const element = <h1>Hello, world</h1>;
ReactDOM.render(element, document.getElementById('root'));
```

### Conditional Rendering  
This is basically if/then logic inside of JSX, returning different HTML/elements.  
```if(isLoggedIn){ return <h1>hello!</h1> } else { return <h1>please login</h1> }```

### Components and Props  
This is reminiscent of other templating languages in that you create parts/components and bring them in elsewhere. You can pass properties to the component using props, which, in JSX, looks like html attributes being added to the tag calling the component.  
```
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

```const element = <Welcome name="Logan" />;```

### Event Handling  
You specify the event as a camelCase attribute and call a function in jsx, defining the function somewhere outside of the returned code.
```
handleClick() {
    // do stuff here
  }

  render() {
    return (
      <button onClick={this.handleClick}>
        // state-conditional content
      </button>
    );
  }
```
