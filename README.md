# ES6: Getters and Setters & Template Literals

## Getters & Setters
**Definition**: Getters and setters are used for defining computed properties. A computed property is one that uses a function to get or set an object value.

### Example from ES5
```javascript
var person = {
  name: "Beyonce",
  get name() {
    return this.name;
  },
  set personName(val) {
    this.name = val;
  }
}
```

Then in the console:

```javascript
person.name = "Mrs. Carter"
var bestArtistEver = person.name
console.log(bestArtistEver);
```

### Examples using ES6
```javascript
class Person {
  constructor(name) {
    this._hello = name;
  }
  get personName() {
    return this._hello;
  }
  set personName (newName) {
    this._name = newName;
  }
}
```

Then in the console:

```javascript
let adele = new Person("Adele")
adele.personName
adele.personName = "A-Dawg"
adele.personName
```

### Video
[![video](images/video-getters-setters.png)](https://www.youtube.com/watch?v=nx6DFeNIXlA)

## Template Literals
**Definition**: Template literals are string literals that can stretch across multiple lines and include interpolated expressions.

Template Strings use back-ticks rather than single or double quotes.

They help make the following easier:

* String interpolation
* String concatenation
* Multiline strings
* String substitution

### Example from ES5
Multiline strings in ES5:

```javascript
var teacher = "Andy \n" + "is on a higher level"
```

### Example from ES6
Multiline strings in ES6:

```javascript
var teacher = `Andy
is on a higher level`
```

### Example from ES5
String concatenation:
```javascript
var person = "Andy Kim";
console.log('my name is ' + person + '!');
```
### Example from ES6
Better string concatenation:

```javascript
var person = "Andy Kim";
console.log(`My name is ${person}!`);
```
### Video
[![video](images/video-literals.png)](https://www.youtube.com/watch?v=LTbnmiXWs2k)
