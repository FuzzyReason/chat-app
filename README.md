# Chat app

This is a pretty old test task which is worth sharing

## About the project

1. I used own React starter kit because it makes the solution more flexible and scalable. For example, the create-react-app kit is limited in some points that are related to the Webpack. So, to my opinion, every developer should have his own starter kit, also it removes all the magic that is in the ready solutions;
2. I used material UI components ([http://www.material-ui.com/#/](http://www.material-ui.com/#/)) to create UI. There are many solutions on the Internet but this is what I like best. It is just my preference;
3. I created the socket-middleware to isolate work with sockets. This solution is not sharpened for a specific implementation of the socket endpoints so it can be used everywhere;
4. I used the SCSS preprocessor to write styles. It allows me to use Nested Rules, Variable Interpolation and etc. It really helps us to write in the BEM approach;
5. I used the Immutable.JS library to have immutability in data;
6. I used the redux-thunk library ([https://github.com/gaearon/redux-thunk](https://github.com/gaearon/redux-thunk)) to create async logic and have access to the store in actions;
7. I created the custom-prop-types-tool to have ability to validate immutable data in proptypes. Something like this: 
```
CustomPropTypesTool.immutableMapOf(PropTypes.instanceOf(MessageRecord));
```
8. I used the Jest library ([https://facebook.github.io/jest/](https://facebook.github.io/jest/)) to write tests.

It was an interesting task for me because I had a possibility to create the react app which uses sockets. I analyzed the existing solutions and realized that at the moment there are no specific architectural solutions for working with sockets. Most people use them directly in the components, but as for me, I think it's wrong.

## Usage

```
npm i
npm run dev
```
