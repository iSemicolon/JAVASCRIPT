# JAVASCRIPT
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>

    
</head>
<body>
   
    <p>HELLO WORLD</p>
    <p id="demo"></p> 
    <p id="demo1"></p>
    <p id="demo2"></p>
    <p id="demo3"></p>
    <p id="demo4"></p>
    <p id="demo5"></p>
    <p id="demo6"></p>
    <p id="demo7"></p>
    <p id="demo8"></p>
    <p id="demo9"></p>
    <p id="demo10"></p>
    <p id="demo11"></p>
    <p id="demo12"></p>
    <p id="demo13"></p>
    <p id="demo14"></p>
    <p id="demo15"></p>
    <p id="demo16"></p>
    <p id="demo17"></p>
    <p id="demo18"></p>
    <p id="demo19"></p>
    <p id="demo20"></p>
    <p id="demo21"></p>
    <p id="demo22"></p>
    <p id="demo23"></p>
    <p id="demo24"></p>
    <p id="demo25"></p>
    <p id="demo26"></p>
    <p id="demo27"></p>
    <p id="demo28"></p>
    <p id="demo29"></p>
    <p id="demo30"></p>
    <p id="demo31"></p>
    <!--Print On Browser Window-->

    <!--
    <p>Hello World</p>
    <script>document.write("WELCOME TO JAVASCRIPT")
    document.getElementById("demo").innerHTML=5+6</script> 

    <p>Hello JavaScript</p>

    <button type="button" onclick="document.write(5+6)">Try it</button>
    
    <script>window.alert(10+20)
    console.log(30+40)</script>

    <button onclick="window.print(100)"></button>
    -->
    <!--
        JAVASCRIPT VARIABLES 
        1.var (global scope)
        2.let (resticted scope)
        3.const(can't change its value)
    -->
<!--
    <script>
        var a=10;
        let b=20;
        const c=30;
        document.writeln(a);
        document.writeln(b);
        document.write(c);
    </script> -->

    <!--var vs let-->
    <script>
/*
{

var a=10;
}

document.getElementById("demo").innerHTML=a; //output will be 10 allow local scope or block level scope


const c=90;
c=45;
document.getElementById("demo").innerHTML=c;  //no output error will generate here


{
let b=50;
}

document.getElementById("demo").innerHTML=b; //no output , */


//DATA TYPES----
//number, datatypes, string , object type
/*
var a=10;
document.getElementById("demo").innerHTML=a;

var ch1='palash7497';
document.getElementById("demo1").innerHTML=ch1;

var str="samanta";
document.getElementById("demo2").innerHTML=str;

//JavaScript objects are written with curly braces {}.

//Object properties are written as name:value pairs, separated by commas.
var obj={firstname: "palash", lastname: "samanta"};
document.getElementById("demo3").innerHTML=obj.firstname;

var bool=false;
document.getElementById("demo4").innerHTML=bool;


var arr=["palash", "nanda", "kalyan"];
document.getElementById("demo5").innerHTML=arr;
        
//TYPE OF OPERATOR FIND

document.getElementById("demo6").innerHTML=typeof arr; //object

var car;
document.getElementById("demo7").innerHTML=typeof car; //undefined

var person=null;
document.getElementById("demo8").innerHTML=typeof person + "<br>" +typeof 1+ "<br>"+ typeof "p"; //object number string
*/

// Spread operators 
//syntex: var variablename1 = [...arr1, ...arr2, ...arr3 ]; 
/*
let arr1=[1,2,3,4,5];
let arr2=[6,7,8,9];

let arr=arr1.concat(arr2);
document.getElementById("demo9").innerHTML=arr;

//simple solutions

let arr1 = [1,2,3];
let arr2 = [4,5];
let arr3=[10,20,30,40];
  
arr = [...arr1, ...arr2, ...arr3];
document.getElementById("demo10").innerHTML=arr;


//Array.from();

let arr=Array.from("abcde123dfr");
document.getElementById("demo11").innerHTML=arr;
*/
//OBJECTS.............

/*
In JavaScript, almost "everything" is an object.

Booleans can be objects (if defined with the new keyword)
Numbers can be objects (if defined with the new keyword)
Strings can be objects (if defined with the new keyword)
Dates are always objects
Maths are always objects
Regular expressions are always objects
Arrays are always objects
Functions are always objects
Objects are always objects
All JavaScript values, except primitives, are objects


//JAVASCRIPT PRIMITIVE DATA TYPES

A primitive value is a value that has no properties or methods.

A primitive data type is data that has a primitive value.

JavaScript defines 5 types of primitive data types:

1. string
2. number
3. boolean
4. null
5. undefined
Primitive values are immutable (they are hardcoded and therefore cannot be changed).

//OBJECT CREATION

There are different ways to create new objects:

1. Define and create a single object, using an object literal.
2. Define and create a single object, with the keyword new.
3. Define an object constructor, and then create objects of the constructed type.

1.USING OBJECT LITERALS

var arr ={a:10, b:20, c:30, d:40};

var arr={
    a:10,
    b:20,
    c:30,
    d:40
};

2.USING NEW KEYWORDS
 var arr=new Object()
 arr.a=10;
 arr.b=20;
 arr.c=30;
 arr.d=40;

 ////javascript objects are immutable

 var arr={a:10, b:20, c:30, d:40}

 var arr1=arr;

 arr1.a=25;

 3.

 //javascript accessing properties

 var arr={a:10, b:20, c:30, d:40}

 1. document.getElementId("demo10").InnerHTML=arr.a
 2. documnet.getElementId("demo10").InnerHTML=arr["a"];
 3. var x="a";
 document.getElementById("demo10").InnerHTML=arr[x];

//Adding New Properties
*/
//var arr={a:10, b:20, c:30, d:40};

 /*arr.e=50;

document.getElementById("demo12").innerHTML=arr.e;

//delete elements

delete arr.a;
document.getElementById("demo13").innerHTML=arr.a;

//displaying object properties
var arrb={a:10, b:20, c:30, d:40};
var db=Object.values(arrb);

document.getElementById("demo14").innerHTML=db;



//JAVASCRIPT GET-SET METHOD

var arrb={a:10,
     b:20,
      c:30,
       d:40,
  get func()
{
    return this.b;
}
};

document.getElementById("demo15").innerHTML=arrb.func;


var arr={a:10,
     b:20,
      c:30,
       d:40,
       e:"",
  set func(lang)
{
    this.e=lang;
}
};

arr.func="english";

document.getElementById("demo16").innerHTML=arr.e;

var person = {
  firstName: "John",
  lastName : "Doe",
  language : "",
  set lang(lang) {
    this.language = lang.toUpperCase();
  }
};

// Set an object property using a setter:
person.lang = "en";

// Display data from the object:
document.getElementById("demo").innerHTML = person.language;



//function add in constructor

function consta(a,b,c,d)
{
    this.a1=a;
    this.b1=b;
    this.c1=c;
    this.d1=d;
}
consta.e=50;

var num=new consta(90,80,60,50);
document.getElementById("demo16").innerHTML=num.e;

//dirctly we can't add in constructor for this we have to write inside constuctor

// no1.solutions

function constac(a,b,c,d)
{
    this.a1=a;
    this.b1=b;
    this.c1=c;
    this.d1=d;
    this.e1=45;
}

var num1=new constac(1,2,3,4);
document.getElementById("demo17").innerHTML=num1.e1;

//BEST SOLUTIONS TO ADDING DATA IN CONSTRUCTORS USING PROTOTYPE

function constacto(a,b,c,d){
    this.a1=a;
    this.b1=b;
    this.c1=c;
    this.d1=d;
}

constacto.prototype.e1=100;

var v=new constacto(10,20,30,40);

document.getElementById("demo18").innerHTML=v.e1;

*/

//Function Call

//JavaScript Function Definitions

/*
var res=myFunc(10,20);

document.getElementById("demo19").innerHTML=res;

function myFunc(a,b)
{
    return a*b;
}

//Function Expressions
A JavaScript function can also be defined using an expression




var res= function(a,b){
    return a*b;
}

document.getElementById("demo20").innerHTML=res;


var res=function(a,b){
    return a*b;
}

document.getElementById("demo21").innerHTML=res(4,3);


//The Function() Constructor

JavaScript functions are defined with the function keyword.

Functions can also be defined with a built-in JavaScript function constructor called Function().

var res=new Function("a","b","return a*b")
document.getElementById("demo22").innerHTML=res(4,2);*/

//JAVASCRIPT FUNCTION

//Function Declaration

/*
var x=func(4,3);

document.getElementById("demo23").innerHTML=x;

function func (a,b) {
    var c=a*b;

    return c;
    
}


//Function Expressions

var x= function (a,b) {
    return a*b;
    
}

document.getElementById("demo24").innerHTML=x;


//Functions are Objects or length og arguments

var x=func(3,4);

function func(a,b){
    return arguments.length;
}
document.getElementById("demo25").innerHTML=x;*/



//Arrow functions allows a short syntax for writing function expressions.

/*You don't need the function keyword, the return keyword, and the curly brackets.
Arrow functions do not have their own this. They are not well suited for defining object methods.

Arrow functions are not hoisted. They must be defined before they are used.

Using const is safer than using var, because a function expression is always constant value.

You can only omit the return keyword and the curly brackets if the function is a single statement. Because of this, it might be a good habit to always keep them:
*/

/*
var x=(a,b)=>{return a*b};

document.getElementById("demo26").innerHTML=x(8,5);



//Function declaration types

var x=(a,b=2)=>{
    return a*b;
}

document.getElementById("demo27").innerHTML=x(5); 

//Array and Functions

var x=func(10,40,30,20,50);
function func()
{
    

    for(var i=0; i<arguments.length;i++)
    {
        var z=arguments[i];

        if(z<=arguments[i]){
            z=arguments[i];

        }
    }

    return z;
}

document.getElementById("demo28").innerHTML=x; 

//Sum of Array ELEMENTS


var x=func(25,45,85,98,47);

function func(){
    var sum=0;

    for(var z=0; z<arguments.length;z++){

        sum=sum+arguments[z];
    }

    return sum;

}

document.getElementById("demo29").innerHTML=x; 

//The JavaScript call() Method


var person={
    fullName: function(){
        return this.firstName+" "+this.lastName;
    }
}

var person1={
    firstName:"PALASH" ,
    lastName: "SAMANTA"
}

var person2={
    firstName:"KALYAN",
    lastName: "JANA"
}

var x=person.fullName.call(person1);
document.getElementById("demo30").innerHTML=x; */


//With the apply() method, you can write a method that can be used on different objects.


var person={
    fullName: function(){
        return this.firstName +" " +this.lastName;
    }
}

//JavaScript Callbacks()

/*A callback is a function passed as an argument to another function

This technique allows a function to call another function

A callback function can run after another function has finished
*/


function display(data){
    document.getElementById("demo32").innerHTML=data;
}

function myFirst(){
    display("GOOD MORNING");
}

function mySecond(){
    display("GOOD NIGHT");
}
mySecond();
myFirst();



var person1={
    firstName:"PALASH",
    lastName:"SAMANTA"

}
var x=person.fullName.apply(person1);
document.getElementById("demo31").innerHTML=x;
    </script>


    
</body>
</html>
