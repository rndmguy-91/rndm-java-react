# JavaScript
	
## let, const
Anstatt den Begriff "var" zu nutzen wird let und const genutzt. const kann dabei nicht mehr verändert werden. let ist quasi das neue var und sollte immer anstatt var genutzt werden. 

## Arrow Functions
Normale Funktion sieht so aus:
```
function myFunction(){ }
```

Arrow Function sehen so aus:

```
const myFunction = (props,props) => { }
const myFunction = props => { } (Nur eine Varbale)
const myFunction = () => { } (Keine)

const myFunction = number => return number * 2; (Nur eine Zeile als Verarbeitung)
```

## Exports and Imports Modules
```
export default Variablename 
```
in einer Datei. Andere Datei: 

```
"import Variablename from './..../.js'"";
```
Es wird also einfach das default geladen. Der Name kann beim Import dann bestimmt werden. 

```javascript
export const clean = () => {...} 

import{clean} from './..../.js'
```

Hier wird auf den exakten Namen gezielt um es zu laden. Hier bestimmt das Export den Namen.

## Classes

```javascript
class Human {
	constructor(){
		this.gender = 'male';
	}
}

class Person{
	constructor(){
		super(); (Von Masterclass Human)
		this.name = 'Max'; (ES6)
	}
	printMyName(){
		console.log(this.name);
	}
}
const person = new Person();
person.printMyName();
````


## Classes ES7

```javascript
class Human {
	gender = 'male';
}

class Person{
	name = 'Max'; (ES7)
	printMyName = () =>{
		console.log(this.name);
	}
	(Funktion ist also quasi eine const Variable in diesem Fall)
}

const person = new Person();
person.printMyName();
```

## Spread and Rest

### Spread 
Split up an array or object propterie.

```javaspript

const array = [ ...oldArray,1,2] (Alles Array vorher + 1 und 2)
const newObject = { ...oldObject, newProp: 5 } (ist newProp vorhanden wird es überschrieben)
```
### Rest

Merge args into an array, like in a function

```javascript
function sort( ...args){
    return args.sort();
}
```









	
	
	
	
	
	
	
	
	
	
	


