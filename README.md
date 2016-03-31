# Chromatic
Explore, visualize, and prototype your organization's UI components. 
Chromatic is the home for your user interface.

## Usage
Chromatic is available at `/styleguide` in your app in development mode.

``` js
const {Chromatic} = Package['chromatic-api'] || {};

ComponentName = React.createClass({
  // code
});

if (Chromatic) {
  Chromatic.add(ComponentName, {
    specs: [
      new Chromatic.Spec('specName1', {props:
        {
          // props used by your component
        }
      }),
      new Chromatic.Spec('specName2', {props:
        {
          // props used by your component
        }
      })
    ]
  });
}
```

## Package list
The following packages have been added to the root of the project
```
react
kadira:flow-router
react-meteor-app
chromatic  # this is all you need to use chromatic

# below are packages with extra components you can use in your projects
animations
buttons
callout
code-block
color-grid
date-components
form-components
list
loading-spinner
overlays
sortable
tooltips
outlines
```
