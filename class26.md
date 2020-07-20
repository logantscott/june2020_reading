[Table of Contents](https://github.com/logantscott/june2020_reading)

# Component Based UI  


## Webpack  



## React  

#### JSX  


#### Rendering  


#### Conditional Rendering  
This is basically if/then logic inside of JSX, returning different HTML/elements.  
```if(isLoggedIn){ <h1>hello!</h1> } else { <h1>please login</h1> }```

#### Components and Props  
This is reminiscent of other templating languages in that you create parts/components and bring them in elsewhere. You can pass properties to the component using props, which, in JSX, looks like html attributes being added to the tag calling the component.  
```class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}```

```const element = <Welcome name="Sara" />;```

#### Event Handling  

