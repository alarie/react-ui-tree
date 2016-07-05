# jab-react-tree [![Build Status](https://travis-ci.org/gabchang/jab-react-tree.svg)](https://travis-ci.org/gabchang/jab-react-tree)
React tree component

This is a fork of [react-ui-tree](https://pqx.github.io/react-ui-tree) by [Wang Zuo](https://github.com/pqx).
This project was initially developed for a webpage builder. It maintains an internal tree structure within the component through [js-tree](https://github.com/wangzuo/js-tree).

### Demo
[https://pqx.github.io/react-ui-tree](https://pqx.github.io/react-ui-tree)

### Installation
``` sh
npm install react-ui-tree --save
```

### Usage
``` javascript
<Tree
  paddingLeft={20}              // left padding for children nodes in pixels
  tree={this.state.tree}        // tree object
  onChange={this.handleChange}  // onChange(tree) tree object changed
  renderNode={this.renderNode}  // renderNode(node) return react element
  onDragStart={ (node) => () }  // onDragStart(node) the dragging tree node
  onDragEnd={ (node) => () }    // onDragEnd(node) the dropped tree node
/>

// a sample tree object
// node.children, node.collapsed, node.leaf properties are hardcoded
{
  "module": "react-ui-tree",
  "children": [{
    "collapsed": true,
    "module": "dist",
    "children": [{
      "module": "node.js"
    }]
  }]
}
```
check [app.js](https://github.com/gabchang/jab-react-tree/blob/master/example/app.js) for a working example

### Development
- npm install
- npm start
- http://localhost:8888/example

### License
MIT
