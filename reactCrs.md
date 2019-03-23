# reactCrs.utf react.utf <http://www.reactivemanifesto.org/>

*2019-01-04 17:27 udemy react course alternative*

<https://www.udemy.com/react-redux/learn/v4/overview> ← add to
curriculum

<https://codepen.io/sgrider/pen/yRWZEq> ← React Starter (a pen)  
<https://codepen.io/> ← "CodePen is a social development environment for
front-end designers and developers"

*2018-01-27 09:16 back to react
course*

<https://medium.com/@ilyasz/react-js-a-better-introduction-to-the-most-powerful-ui-library-ever-created-ecd96e8f4621>  
<https://medium.com/@ilyasz/mastering-react-functional-components-with-recompose-d4dd6ac98834>  
<https://github.com/hantsy/spring-reactive-sample> ← add to curriculum  
<https://deals.javacodegeeks.com/user/purchases> ← add to curriculum  
<http://www.baeldung.com/spring-boot-actuators> ← add to curriculum  

*2017-11-19 18:55 React Course, day two*

per *React in Motion*
<https://livevideo.manning.com/module/35_2_4/react-in-motion/ramping-up-with-react/building-a-hello-world-component>

Jest is the test fwork of choice, built on Jasmine

next: Unit 3, module 1:
<https://livevideo.manning.com/module/35_3_1/react-in-motion/componentised-uis%3a-intro-%26-overview/what-is-a-component%3f>

jsx can invoke components with an html \< /\> syntax e.g.

    render ()    {
                return <newsletterWidget />
                }

next: Unit 3, module 2:
<https://livevideo.manning.com/module/35_3_2/react-in-motion/componentised-uis%3a-intro-%26-overview/using-props>

props are for passing data between components

have a functioning demo

    /Users/khazelton/opt/hanggryhippo
    npm start
    
    App.js
    ----------
    import React, { Component } from 'react';
    import Display from './Display';
    import './App.css'
    
    class App extends Component {
      render() {
        return (
          <div>
              <Display message='hippo very angry'/>;
          </div>
        );
      }
    }
    
    export default App;
    ----------
    
    Display.jsx
    ----------
    import React, { Component } from 'react';
    
    class Display extends Component {
        render() {
            return (
                <div>
                    {this.props.message}
                </div>
            );
        }
    
    }
    
    export default Display;

Next up:
<https://livevideo.manning.com/module/35_3_3/react-in-motion/componentised-uis%3a-intro-%26-overview/discovering-proptypes>
Unit 3 Module 3

*2017-11-18 08:16 React course*

Curriculum for learning React

<https://github.com/zacbraddy/hangryhippo> React in Motion repo ⇐= ++
Primary course text

    tools:
      - editors
        - atom
        √ webstorm (IntelliJ) <== ++
    
      - build tools
        - webpack (~ grunt, gulp)
        - yeoman:  https://www.jetbrains.com/help/webstorm/creating-a-project-using-yeoman-generator.html  Build Pipeline Generators
        √ create-react-app   <== ++ easiest
    
      - debugging tools
        √ react developer tools for chrome
    
    https://livevideo.manning.com/module/35_2_4/react-in-motion/ramping-up-with-react/building-a-hello-world-component
    
    https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md  <== create-react-home
    
    followed by Azat Mardan, _React Quickly: Painless web apps with React, JSX, Redux, and GraphQL_

KeithsOfficeMBP:opt khazelton$ node -v v6.11.3

KeithsOfficeMBP:opt khazelton$ npm -v 3.10.10

KeithsOfficeMBP:opt khazelton$ npm i create-react-app -g
/Users/khazelton/.npm-packages/bin/create-react-app →
/Users/khazelton/.npm-packages/lib/node\_modules/create-react-app/index.js
- safe-to-string-x@2.0.3
node\_modules/create-react-app/node\_modules/safe-to-string-x
/Users/khazelton/.npm-packages/lib └─┬ create-react-app@1.4.3 ├─┬
hyperquest@2.1.2 │ └─┬ buffer-from@0.1.1 │ └─┬ is-array-buffer-x@1.7.0 │
├─┬ is-object-like-x@1.6.0 │ │ └─┬ is-function-x@3.3.0 │ │ └─┬
normalize-space-x@3.0.0 │ │ ├─┬ trim-x@3.0.0 │ │ │ ├── trim-left-x@3.0.0
│ │ │ └── trim-right-x@3.0.0 │ │ └── white-space-x@3.0.0 │ └─┬
object-get-own-property-descriptor-x@3.2.0 │ ├──
has-own-property-x@3.2.0 │ └─┬ is-index-x@1.1.0 │ ├── math-clamp-x@1.2.0
│ ├─┬ to-integer-x@3.0.0 │ │ └── math-sign-x@3.0.0 │ └─┬
to-number-x@2.0.0 │ └── parse-int-x@2.0.0 └── tar-pack@3.4.1

KeithsOfficeMBP:opt khazelton$ create-react-app hanggryhippo

Creating a new React app in /Users/khazelton/opt/hanggryhippo. ⇐

Installing packages. This might take a couple of minutes. Installing
react, react-dom, and react-scripts…​

> fsevents@1.1.2 install
> /Users/khazelton/opt/hanggryhippo/node\_modules/fsevents node install

\[fsevents\] Success:
"/Users/khazelton/opt/hanggryhippo/node\_modules/fsevents/lib/binding/Release/node-v48-darwin-x64/fse.node"
already installed Pass --update-binary to reinstall or
--build-from-source to recompile

> uglifyjs-webpack-plugin@0.4.6 postinstall
> /Users/khazelton/opt/hanggryhippo/node\_modules/uglifyjs-webpack-plugin
> node lib/post\_install.js

hanggryhippo@0.1.0 /Users/khazelton/opt/hanggryhippo ├─┬ react@16.1.1 │
├─┬ fbjs@0.8.16 │ │ ├── core-js@1.2.7 │ │ ├─┬ isomorphic-fetch@2.2.1 │
│ │ └─┬ node-fetch@1.7.3 │ │ │ ├── encoding@0.1.12 │ │ │ └──
is-stream@1.1.0 │ │ ├── promise@7.3.1 │ │ ├── setimmediate@1.0.5 │ │ └──
ua-parser-js@0.7.17 │ ├─┬ loose-envify@1.3.1 │ │ └── js-tokens@3.0.2 │
├── object-assign@4.1.1 │ └── prop-types@15.6.0 ├── react-dom@16.1.1
└─┬ react-scripts@1.0.17 ├─┬ autoprefixer@7.1.6 │ ├─┬ browserslist@2.9.0
│ │ └── electron-to-chromium@1.3.27 │ ├── caniuse-lite@1.0.30000766 │
├── normalize-range@0.1.2 …​ …​ │ │ └── path-type@1.1.0 │ ├─┬
string-width@1.0.2 │ │ ├── code-point-at@1.1.0 │ │ └─┬
is-fullwidth-code-point@1.0.0 │ │ └── number-is-nan@1.0.1 │ ├──
which-module@1.0.0 │ └── yargs-parser@4.2.1 ├─┬
webpack-manifest-plugin@1.3.2 │ └─┬ fs-extra@0.30.0 │ ├── jsonfile@2.4.0
│ └── klaw@1.3.1 └── whatwg-fetch@2.0.3 A

Success\! Created hanggryhippo at /Users/khazelton/opt/hanggryhippo
Inside that directory, you can run several commands:

    npm start
      Starts the development server.

    npm run build
      Bundles the app into static files for production.

    npm test
      Starts the test runner.

    npm run eject
      Removes this tool and copies build dependencies, configuration files
      and scripts into the app directory. If you do this, you can’t go back!

We suggest that you begin by typing:

    cd hanggryhippo
    npm start

Happy hacking\!

    - - -
    _2018-04-30  13:29 references and links_
    
    https://reactjs.org/tutorial/tutorial.html
    https://medium.com/the-node-js-collection/modern-javascript-explained-for-dinosaurs-f695e9747b70

