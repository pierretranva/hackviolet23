


## Table of contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Technologies](#technologies)
4. [Pre-Requisites](#pre-requisites)
5. [Setup Instructions](#setup-instructions)
6. [Register Windows with Slots (Quick Registration)](#register-windows-slots)
7. [Register Custom Windows (Advanced Registration)](#register-windows-custom)
8. [Window API](#window-api)
9. [FAQ](#faq)

<a name="project-overview"></a>
## Project Overview
This project aims to create an interactive Web OS template for Vue. Included in the template are all necessary logic for individual window components, navbars and app grids. Users are able to register new components (custom or otherwise) easily. 

<a name="features"></a>
## Features
- Interactable and Draggable Windows
- Built-in Navigation Bar (+ logic)
- Window Logic (States, Fullscreen, Minimization etc.)
- Themes (Blueprint, Windows, MacOS)

<a name="technologies"></a>
## Technologies
- Vue 2
- Vuex 
- InteractJS
- MomentJS

<a name="setup-instruction"></a>
## Setup Instructions

1. Clone the repository to your local machine

2. Make sure you have Vue.js installed 

[Official Documentation from Vue](https://vuejs.org/v2/guide/installation.html)

3. Rename the folder to ```hackviolet23```

4. Cd into project folder and install packages + dependencies


```bash
$ cd hackviolet23 && npm install
```

4. Serve project

```bash
$ npm run serve
```
5. If there is an error with node while loading the dev server (Windows OS ran into this problem) then type this command first:

```bash
$ $env:NODE_OPTIONS="--openssl-legacy-provider"
```

<a name="register-windows-slots"></a>
## Register Windows (slots method)

Registering a window with the slots method will allow you quick access to the pre-made window template. This method is most suited for users who do not require any change in the styling or layout of the window itself.

1. Head to ```/src/store/index.js```

2. Register a new window by pasting the following snippet within the windows state array

```js
{
     windowId: "UniqueWindowID", 
     windowState: "close",
     displayName: "Unique Window",
     windowComponent: 'window',
     windowContent: 'Placeholder',
     windowContentPadding: {
         top: null,
         right: null,
         bottom: null,
         left: null
     },
     position: "absolute",
     positionX: "10vw",
     positionY: "10vh",
     iconImage: "placeholder.png",
     altText: "Placeholder Icon",
     fullscreen: false
 },
 ```
 
3. Change 'windowId' to a unique window ID and 'displayName' to a preferred name for the window.

```js
windowId: "MyNewWindow"
```

```js
displayName: "New Window"
```

4. The content displayed within the window is registered to the 'Placeholder' component. Simply create a new content component under ```/src/components/views``` folder and replace 'windowContent' with the name of the new content component created. 

```js
windowContent: "MyNewWindowContent"
```

/src/components/views/MyNewWindowContent.vue
```js
<template>
  <p>this is my new window's content!</p>
</template>
```

5. Head over to ```/src/App.vue``` to import and register the new components under the <script> section.
  
```js
  import MyNewWindowContent from './components/views/MyNewWindowContent'
```
  
```js
  components: {
    ...,
    MyNewWindowContent
  }
```

6. Save all changed or created files and head to localhost to view changes.
     
<a name="register-windows-custom"></a>
## Register Windows (Custom Window)

Registering a custom window is also made relatively simple due to each window having a dedicated object state tracking the window to present. You might want to register a custom window if the layout or styling of the window itself needs to be modified (i.e. removal or addition of buttons in window's top bar).
     
1. Head to ```/src/store/index.js```

2. Register a new window by pasting the following snippet within the windows state array

```js
{
     windowId: "UniqueWindowID", 
     windowState: "close",
     displayName: "Unique Window",
     windowComponent: 'window',
     windowContent: 'Placeholder',
     windowContentPadding: {
         top: null,
         right: null,
         bottom: null,
         left: null
     },
     position: "absolute",
     positionX: "10vw",
     positionY: "10vh",
     iconImage: "placeholder.png",
     altText: "Placeholder Icon",
     fullscreen: false
 },
 ```
 
3. Change 'windowId' to a unique window ID and 'displayName' to a preferred name for the window.

```js
windowId: "MyCustomWindow"
```

```js
displayName: "Custom Window"
```
     
4. The window UI itself is stored under 'windowComponent' and we can now register our own custom window by changing the registered components.
    
```
windowComponent: 'SpecialWindow'
```
     
5. Create a new window component named ```SpecialWindow.vue
``` under ```/src/components/template``` and ***copy the contents of Window.vue into this new file***. 
     
6. For demonstration purposes, we will simply change the background of the 'top-bar' of the window and add some content replacing the slot section. 
     
Paste this CSS snippet under the style section.
```css
.top-bar {
     background-color: green !important;
}
```
     
Replace the slot tags with this snippet of HTML.   
     
```html
<p>This is my new custom window</p>
```

6. Head over to ```/src/App.vue``` to import and register the new components under the <script> section.
```js
  import SpecialWindow from './components/template/SpecialWindow'
```
  
```js
  components: {
    ...,
    SpecialWindow
  }
```
     
7. Save all changed or created files and head to localhost to view changes.
     
<a name="switch-themes"></a>
## Switching Themes
Included in the template are three different themes, the default Blueprint theme, a MacOS theme and a Windows theme. Switching between themes is made relatively easy but certain themes may require some minor tweaking.

### Blueprint Theme
1. Head over to ```/src/App.vue```, under the script section, import the Blueprint Navbar variant. 
```js 
import Navbar from './components/blueprint/Navbar'
```

2. Under the style section of App.vue, import the Blueprint CSS variant. 
```css
@import './assets/css/blueprint/app.css';
@import './assets/css/blueprint/window.css';
@import './assets/css/blueprint/appgrid.css';
```

3. Save all changes and head to localhost to view changes. 

### Windows Theme
1. Head over to ```/src/App.vue```, under the script section, import the Windows Navbar variant. 
```js 
import Navbar from './components/windows/Navbar'
```

2. Under the style section of App.vue, import the Windows CSS variant. 
```css
@import './assets/css/windows/app.css';
@import './assets/css/windows/window.css';
@import './assets/css/windows/appgrid.css';
```    
     

### MacOS Theme
1. Head over to ```/src/App.vue```, under the script section, import the MacOS Navbar variant ***and MacOS Top Navbar***. 
```js 
import Navbar from './components/macos/Navbar'
import TopNavbar from './components/macos/TopNavbar.vue'
```

2. Register the Top Navbar
```js
components: {
     ...,
     TopNavbar
}```
     
3. Under the style section of App.vue, import the MacOS CSS variant. 
```css
@import './assets/css/macos/app.css';
@import './assets/css/macos/window.css';
@import './assets/css/macos/appgrid.css';
```
     
<a name="window-api"></a>
## Window API
| Name | Description | Type |
| ---- | ----------- | ---- |
| windowId | Unique ID to identify a window | String |
| windowState | Tracks window's open, close or minimized state | String |
| displayName | Label for window in app grid and window header title | String |
| windowComponent | Window's own UI, can be changed to use a custom window, see custom window registration section | String |
| windowContent | Tracks window's content component, will be inserted in under slots if making use of standard window, see registration of windows with slots section | String |
| windowContentPadding | Sets padding of content within the window | String or null |
| position | Sets CSS position of window | String |
| positionX | Sets initial X displacement of window | String |
| positionY | Sets intial Y displacement of window | String |
| iconImage | Name of icon image of window, icons should be placed in ```/assets/icons/``` | String |
| altText | Icon's alternative text | String |
| fullscreen | Tracks whether a window is in fullscreen or not | Boolean |
