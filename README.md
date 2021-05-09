
<p align="center">

  <img alt="Repository size" src="https://img.shields.io/github/repo-size/aquistapace/react-tooltip-soft">
  
  <a href="https://github.com/aquistapace/react-tooltip-soft/commits/master">
    <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/aquistapace/react-tooltip-soft">
  </a>
    
   <img alt="License" src="https://img.shields.io/badge/license-MIT-brightgreen">
 

  <a href="https://github.com/aquistapace">
    <img alt="Feito por Caroline Aquistapace" src="https://img.shields.io/badge/feito%20por-Caroline-Aquistapace%237519C1">
  </a>
  
  
 
</p>
<h1 align="center">
   React Tooltip Soft 
</h1>

<p align="center"> 
 A simple and basic React tooltip component for yours projects.  
</p>
<p align="left"> 
 Use a Tooltip Easyer when you want to provide an additional explanation about a particular element.  
</p>

## Table Contents
•  <a href="#Install">Install</a> 
•  <a href="#-sobre-o-projeto">Usage</a> 
•  <a href="#-sobre-o-projeto">Documentation</a> 
•  <a href="#-sobre-o-projeto">Examples</a> 


## ⚙️ Install
```bash
# npm
  npm install react-tooltip-soft

# yarn
  yarn add react-tooltip-soft
```


## 🛠 Usage

Import Tooltip Component 
```bash
import {Tooltip} from 'react-tooltip-soft'
```

Utilize o componente com qualquer coisa
```bash
<Tooltip content="Hi">
	<button>Example</button>
</Tooltip>
```
---
## Demo
<p align="left">

  <img alt="Mobile Home" title="Mobile Home" src="https://github.com/aquistapace/react-tooltip-soft/blob/main/tooltip.gif" width="500px">

</p>

## 📄 Documentation
### Component Props
The majority of settings for the Tooltip component are configured using props:
Name | Type| Default | Description| Values
:--------- | :------: | :------:|:--------- |:------:|
position|- | top| Display positioning of the Tooltip in relation to the target element. | left , right, top and bottom
content|any| Example| Content to be displayed in the Tooltip. |
arrow|-| solid|Displays the arrow when solid.Does not display an arrow when none.  |solid or none
arrowColor| string| -| Color of arrow.|*view note
textColor| string| -| Color of text.|*view note
borderColor| string| -| Color of border.|*view note
backgroundColor| string| -| Color of background. |*view note
disabled| boolean| false| Disables the display of the tooltip when true.| true or false
> ***Note** : Accepts color by name  or color code : HEX, RGB, RGBA and HSL .


## 💡 Examples
### Creating Custom Tooltip
```bash
import React from 'react'
import {Tooltip} from 'react-tooltip-soft'

const  App = () => {
	return (
		<>
			<Tooltip 
			 content="Hi" 
			 backgroundColor="purpl"
			 textColor="#000000"
			 borderColor="pink"
			 arrowColor="pink"
			 >
				<button>Example</button>
			</Tooltip>
		</>
	)
}
export default App

```
### Creating a Tooltip without an Arrow
```bash
import React from 'react'
import {Tooltip} from 'react-tooltip-soft'

const  App = () => {
	return (
		<>
			<Tooltip 
			 content="Hi" 
			 backgroundColor="purpl"
			 textColor="#000000"
			 borderColor="pink"
			 arrow="none"
			 >
				<button>Example</button>
			</Tooltip>
		</>
	)
}
export default App

```
### Creating a Tooltip with Image as Content
```bash
import React from 'react'
import {Tooltip} from 'react-tooltip-soft'

const  App = () => {
	return (
		<>
			<Tooltip 
			 content={
			 <>
			 <img src={Image} alt="image">
			 </>}
			 backgroundColor="purpl"
			 textColor="#000000"
			 borderColor="pink"
			 arrowColor="pink"
			 >
				<button>Example</button>
			</Tooltip>
		</>
	)
}
export default App

```


