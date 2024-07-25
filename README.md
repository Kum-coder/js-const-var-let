scope = it is the certain region in a program where define variables can exist and recognise.
like = this is functional scope
functional greet(){
 ur body here
}
this is block scope:-
{
 ur body here
}
var is a functional scope and it can be accesible anywhere in the scope but let and const are a block scope and they are not accessible outside the scope.
for example:-
var a = 5
console.log(a)
or:-
{
var a = 14
}
console.log(a)
but:-
{
let a = 14
console.log(a)
}

{
const a = 15
console.log(a)
}
variable shadowing:-
function greet(){
let a = 'hello'
if (me){
let a = 'hi' - this will shadow that hello or i can say replace that hello, but it can be done inside the block only
console.log(a)
}
console.log(a) - if i use this then it will give me hello bcz it is outside the block
}
There is term called illegal shadowing if in case let variable shadow by var variable.
like:-
function me(){
let a = 14
if (true){
var a = 24 - this will replace value of let bt it will throw error
console.log(a)
}
}

var variables can be redeclared but not let and const variables
like:- 
var a
var a - it not show error
let a
let a - it show error same with happen using const
let and var can be declare without assign values it will not show error but const never declare without assign values.
var and let can be update but const can't be update
var a = 14
a = 5 - it never show error same with let also
const a = 4
a = 8 - it will show error 

hoisting - during the creation phase javascript engine moves the variables and function declaration to top of the code.
like:-
console.log(a)
var a = 14 - it will show undefined bt not error
but:-
console.log(a)
let a = 14 - it throw error bt it is hoisted in temperal dead zone
temperal dead zone - it is the time between declaration  and initialisation of the let and const variables
like - 
function greet(){
console.log(a)
var a = 14 - it will show undefine bcz var is after console.log and it not print value
let a = 7 - it show error as it can not be access before initialisation
const a = 8 - same here also
}


