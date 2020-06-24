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

## Destructing
Extract arrray elements and store them in variables.

```javascript
const numbers = [1,2,3];
[num1,num2] = numbers;
console.log(num1,num2); -> only 1 and 2
```
same with objects
```jvascript
{name} = {name:'Max', age:'28'}
console.log(name) -> Max (age would not work)
```
## References
primitive types like bool int etc. are copied like:
```jvascript
const number = 1;
const number2 = number;  // number2 is a real copy.
```
working with objects you just copy the pointer to memory and not the hole object or arrays.

```jvascript
const person = {
    name:'Max';
};
const personTwo = person;
```
So personTwo is a copy of the pointer to person

```jvascript
const person = {
    name:'Max';
};
const personTwo {
    ...person
}
```
this a real copy of the person by using the spread operator.

## ArrayFunctions

```jvascript
const numbers = [1,2,3];
const doubleNumArray = numbers.map( (num) => {
    return num * 2;
});
```
Modify arrays with array functions like .map(). In map for example you can create a arrow function witch works for each number 'num'. 





	
	
	
	
	
	
	
	
	
	
	


