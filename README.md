## What is React ?
React is a *JavaScript library* created by Facebook and is used for building user interfaces (UIs) and front-end applications.

React is often called framework because of its behavior and capabilities. It's basically V in MVC.

## Why Use React ?
* Makes front-end JavaScript much easier 
* Uses self contained, independent components with their own state
* Much more interactive UIs
* Virtual DOM
* JSX - Easily incorporate JS in markup
* Easy to work with teams

## What Should You Know Before Learning React ?
* JavaScript Fundamentals (Objects, Arrays, Conditionals, etc)

**It may help to learn these first :**
* Classes
* Destructuring
* High Order Array Methods - forEach, map, filter
* Arrow Functions
* Fetch API & Promises 
  
## React State 
* Components can have state which is an object that determines how that components renders and behaves
* We can also have "application level" state by using a state manager like *Redux* or *React Context API*.

for e.g.
```javascript
state = { 
  title: 'xxx',
  body: 'xxx'
  isFeatured: true
}
```

## Create React App
* CLI Tool for creating React Applications.
* Uses *Webpack* but needs no configuration from you.
* Comes bundled with a dev server with hot reload.
* "*npm run build*" will compile all your code to something that the browser can read.

## Anatomy of a Component
**Class based component**
```javascript
Class Post extends React.Component {
  state = {
    title: 'Post One',
    body: 'This is my post'
  }

  render() {
    return (
      <div>
        <h3>{ this.state.title }</h3>
        <p>{this.state.body }</p>
      </div>
    )
  }
}
```


### index.html
React is a single page application(SPA) framework i.e. everything runs through one physical single page i.e index.html. Everything outputs in a following single div.
```javascript
  <div id="root"></div>
```

* render() is a lifecycle method required to render a component in browser