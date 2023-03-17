# JSObject-Class_ArraysOfData
JavaScript Object, Class data. Create a multiple object that push data array into object setter and getter JS.

```JS
 // Developer Object !
 class Developer {

  constructor(name, yearsExperience) {

    this.name = name;
    this.yearsExperience = yearsExperience;

  }

  // Method getName of Developer
  getName = () => { return this.name; }

  // Method Years of Experience of Developer
  getYearsExperience = () => { return this.yearsExperience; }

 } 
```

```JS 
 // Create NEW DEVELOPER !
 const dev1 = new Developer('Niel', 6 );
 const dev2 = new Developer('NielOffice', 7 );
 
 // Check Developers!
 console.log( dev1, dev2 );

 // Result 
 Developer {name: 'Niel', yearsExperience: 6, getName: ƒ, getYearsExperience: ƒ} 
 Developer {name: 'NielOffice', yearsExperience: 7, getName: ƒ, getYearsExperience: ƒ}
```
 
```JS
 // Experts 
 class Experts {
 
  // Expertise is the ability
  // The Experts is the objects
  constructor(expertise, experts ) {
     
    this.expertise  = expertise;
    this.experts = experts;
  }
  
  // Setter or add new Experts
  // push to array this.experts
  addExperts = (experts) => { return this.experts.push(experts); } 

  // Getter 
  // Get all expert
  getExperts = () => { return this.experts; }

 }
```
 
```JS
 // Create two object Developers 
 // Expertise is Web Developer
 const experts = new Experts('Web Developer', [dev1, dev2] ); // NEW DEVs
 // Checking objects
 console.log(experts);

```

```JS
 // Console.log() | Result 
 Experts {expertise: 'Web Developer', experts: Array(2), addExperts: ƒ, getExperts: ƒ}
 addExperts : (experts) => { return this.experts.push(experts); }
 expertise : "Web Developer"
 experts : Array(2)
  0 : Developer {name: 'Niel', yearsExperience: 6, getName: ƒ, getYearsExperience: ƒ}
  1 : Developer {name: 'NielOffice', yearsExperience: 7, getName: ƒ, getYearsExperience: ƒ}
 length : 2
 [[Prototype]] : Array(0)
 getExperts : () => { return this.experts; }
 [[Prototype]] : Object
```
 
```JS 
 // add new expert
 const dev3 = new Developer('John', 8 ); 
 // set expert
 experts.addExperts(dev3);

 // check new added expert
 console.log(experts.getExperts());
```
 
```JS
 // Console.log() | Result 
 (3) [Developer, Developer, Developer]
  0 : Developer {name: 'Niel', yearsExperience: 6, getName: ƒ, getYearsExperience: ƒ}
  1 : Developer {name: 'NielOffice', yearsExperience: 7, getName: ƒ, getYearsExperience: ƒ}
  2 : Developer {name: 'John', yearsExperience: 8, getName: ƒ, getYearsExperience: ƒ}
 length : 3
 [[Prototype]] : Array(0)
```

 This is how to create an static object and new object that push on existing without instantiate class. 
 This will helps when you are collecting a static data that you needs in order to manipulate for whatever reason to achive your web application goal interface or interactive. 
 This how you can easily maintain your code clean and easy. 
