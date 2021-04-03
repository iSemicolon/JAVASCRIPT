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








    </script>
    
    //////////////////////////////////////////////////////////////////////////////
    
    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>

    <script>
        function takevalue()
        {
            var fname=document.getElementById("fullname").value;
            var dateOfBirth=document.getElementById("dob").value;
            var UserId=document.getElementById("uId").value;

        var gender1=document.getElementById("r1").value;
        var gender2=document.getElementById("r2").value;
        var gender3=document.getElementById("r3").value;

         var rd1=document.getElementById('r1').checked;
         var rd2=document.getElementById('r2').checked;
         var rd3=document.getElementById('r3').checked;
       

        var loc1=document.getElementById("l1").value;
        var loc2=document.getElementById("l2").value;
        var loc3=document.getElementById("l3").value;
        var loc4=document.getElementById("l4").value;

         var chk1=document.getElementById('l1').checked;
         var chk2=document.getElementById('l2').checked;
         var chk3=document.getElementById('l3').checked;
         var chk4=document.getElementById('l4').checked;
       



            document.write("YOUR INFO : <BR>"+"FIRST NAME : "+fname+"<br>");
            document.write("date-Of-Birth : "+dateOfBirth+"<br>");
            document.write("user : "+UserId+"<br>");              


              //GENDER FIND
            if(rd1==true)
          {
            
          document.write("Gender : "+gender1+"<br>");
         }

          else if(rd2==true)
          {
            
          
          document.write("Gender : "+gender2+"<br>");
          }

        else{
         
        
          document.write("Gender : "+gender3+"<br>");
          }
       

       //LOCATION FIND
          if(chk1==true)
          {
            
          document.write("Location : "+loc1+"<br>");
         }

          else if(chk2==true)
          {
            
          
          document.write("Location : "+loc2+"<br>");
          }

        else if(chk3==true)
         {
        
          document.write("Location : "+loc3+"<br>");
          }

          else 
         {
        
          document.write("Location : "+loc4+"<br>");
          }


        }


        


        </script>


</head>
<body>
    
        <form >
            
                    <input type="text" style="text-transform: uppercase" id="fullname" placeholder="full name">
                
                    <input type="date" id="dob" placeholder="Date of Birth">
                
                    <input type="text" id="uId" placeholder="username">
                
                        <input type="password" placeholder="password">
                   
                        <input type="text" placeholder="confirm password">
                   
                  
                      
                        <input type="radio" id="r1" name="gender4"  value="male" >Male
                        <input type="radio" id="r2" name="gender4"  value="female">Female
                        <input type="radio" id="r3" name="gender4" value="other">Other
                        

                                <input type="checkbox" id="l1" name="kol" value="KOLKATA">KOLKATA
                                <input type="checkbox" id="l2" name="jp" value="JAIPUR">JAIPUR
                                <input type="checkbox" id="l3" name="del" value="DELHI">DELHI
                                <input type="checkbox" id="l4" name="blr" value="BANGALORE">BANGALORE

<!--

                                <select name="dropDown" id="dp">
                                  <option value="Deposit">Deposit</option>
                                  <option value="Withdraw">Withdraw</option>
                                </select> -->


               
                <!-- NOW WE NEED TO ADD SUBMIT BUTTON -->
            
                    <input type="submit" onclick="takevalue()">
                 
        </form>
    

</body>
</html>
    
</body>
</html>
