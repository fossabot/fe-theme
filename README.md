<p align="center">
  <a href="https://github.com/hg-arch/fe-theme">
    <img src="https://png.pngtree.com/png-clipart/20220103/original/pngtree-show-biceps-png-image_7019290.png" alt="FE-Theme Logo" width="100" />
  </a>
</p>
<h2 align="center">A React library using styled-component to build consistent, responsive, theme able UI 💪 </h2>
<br />
<p align="center">
   <a href="https://www.npmjs.com/package/fe-theme">
     <img alt="Minified Size" src="https://img.shields.io/badge/minzipped_size-100kb-%23e95143"/>
   </a>
  <a href="https://styled-components.com/releases#v6.1.1">
    <img alt="Styled Component Version" src="https://img.shields.io/badge/styled_component-6.1.1-%2350c62a"/>
  </a>
  <a href="https://react.dev/reference/react">
    <img alt="React Version" src="https://img.shields.io/badge/react_version-18.2.0-blue"/>
  </a>
  <a href="https://www.npmjs.com/package/fe-theme">
    <img alt="Downloads Per Month" src="https://img.shields.io/badge/downloads-1k%2Fmonth-%23027f02"/>
  </a>
  <a href="https://github.com/hg-arch/fe-theme/stargazers">
    <img alt="Stars" src="https://img.shields.io/badge/stars-30.0-%23eac54f"/>
  </a>
  <a href="https://github.com/hg-arch/fe-theme/blob/master/LICENSE.md">
    <img alt="MIT License" src="https://img.shields.io/badge/license-MIT-%23d7614b"/>
  </a>
</p>
<br />

FE-Theme is a styled-component based comprehensive library of accessible, reusable, and composable React components that streamlines the development of modern web applications and websites. The library offers a theme based UI to quickly start a new small/medium/large size web based applications.

## Table of contents

- 📦 [Installation](#installation)
- 💻 [Setup](#setup)
- ✨ [Contributors](#contributors)
- ⚖️ [License](#license)
  
## Installation

    npm install fe-theme --save

## Setup

#### 1. Importing UI component in your application
```js
import Button from 'fe-theme/Button';
```

```js
<Button />
```
Hurrah...!!! Button is created, but color does not match with the application. No worries.
  

#### 2. Do you want to change theme according to your application?
##### Generate a sample file(sample-theme.js) by running below commond in terminal in your project location.

```cp sample-theme.js ./``` Or <a href="https://github.com/hg-arch/fe-theme/blob/master/sample-theme.js">```Download Sample File```</a>

#### 3. Bootstrap theme by calling a ```themeInit```  function and pass it to ```ThemeProvider``` in ```theme``` property

```js
import React from 'react';
import ReactDOM from 'react-dom';
import { ThemeProvider } from 'styled-components';
import themeInit from 'fe-theme/Init';
import theme from './sample-theme.js';
import App from './App';

ReactDOM.hydrate(
    <ThemeProvider theme={themeInit(theme)}>
        <App />
    </ThemeProvider>,
    document.getElementById('root'),
);
```

#### 4. Go to the sample-theme.js and change the theme like primary: '#000', secondary: '#333'
```js
<Button design="primary" />
<Button design="secondary" />
```

## Contributors

Thanks goes to these wonderful people

<table>
    <tbody>
      <tr>
        <td align="center" valign="top" width="14.28%">
          <a href="https://github.com/hg-arch">
            <img src="https://avatars.githubusercontent.com/u/6891544?s=400&v=4" width="64px;" alt="Himanshu Gupta" />
            <br />
            <sub><b>Himanshu Gupta</b></sub>
          </a>
          <br />
        </td>
        <td align="center" valign="top" width="14.28%">
          <a href="https://github.com/ashwinihegde123">
            <img src="https://avatars.githubusercontent.com/u/40521396?v=4" width="64px;" alt="Ashwini Hegde" />
            <br />
            <sub><b>Ashwini Hegde</b></sub>
          </a>
          <br />
        </td>
        <td align="center" valign="top" width="14.28%">
          <a href="https://github.com/vineet091">
            <img src="https://avatars.githubusercontent.com/u/5345138?v=4" width="64px;" alt="Vineet Gupta" />
            <br />
            <sub><b>Vineet Gupta</b></sub>
          </a>
          <br />
        </td>
        <td align="center" valign="top" width="14.28%">
          <a href="https://github.com/Alok30">
            <img src="https://avatars.githubusercontent.com/u/36290248?s=64&v=4" width="64px;" alt="Alok Dubey" />
            <br />
            <sub><b>Alok Dubey</b></sub>
          </a>
          <br />
        </td>
        <td align="center" valign="top" width="14.28%">
          <a href="https://github.com/Ravi-Chef">
            <img src="https://avatars.githubusercontent.com/u/31059087?v=4" width="64px;" alt="Ravi Verma" />
            <br />
            <sub><b>Ravi Verma</b></sub>
          </a>
          <br />
        </td>
      </tr>
    </tbody>
</table>

### License

MIT © [Himanshu Gupta](https://github.com/hg-arch)
