Write a blog on difference between HTTP1.1 vs HTTP2?

HTTP1.1:

(i) HTTP1.1 is less efficient when compared to HTTP2.
(ii) It is slower than HTTP2 in terms of site loading.
(iii) It doesn't allow PUSH.
(iv) HTTP1.1 loads resource one after other so if one resource can't loaded,it bolocks all other resources behind it.
(v) It keeps all requests and responses in plain text.
(vi) Here Server only serves content What client ask for it.
(vii) HTTP1.1 maintains less performance boost compared to other.
(viii) It doesn't use HPACK method.
(ix) It uses ordered and blocking methods.
(x) In HTTP1.1 developers doesn't have any control over prioritization.
(xi) It doesn't reduce any additional round-trip times While Http2 reduces,meaning websites load faster with less optimization.


HTTP2:

(i) HTTP2 is more efficient.
(ii) It is faster than Http1.1 in terms of site loading.
(iii) It allows PUSH to response  proactively into client cache.
(iv) Http2 is able to use single TCP connection to send multiple Streams of data at once so that no resource blocks any other resource.
(v) It uses binary framing layer to encapsulate all messages in binary format.
(vi) By using PUSH, it allows server to serve content before client asks for it.
(vii) It maintains great performance boost.
(viii) It uses most advanced compression method HPACK.
(ix) HTTP2 is fully multiplexed.
(X) In Http2 developers have detailed control over prioritization.
(xi) While Http2 reduces additional round-trip times, meaning websites load faster with less optimatization.


Write a blog about objects and its internal representation in Javascript?

Objects and its internal representation:

A Javascript objects is a collection of named values having state and behaviour(properties and method).

For eg: Person, Car, Bike, Personal computer, Washing machine,etc..
Take the case of cars.
            All cars have the same properties, but the property values differ from car to car. All cars have the same methods, but the methods are performed at different times.
            Let's have an example of MERC car and list out its properties(Features):
       1. Make: Mercedes
       2. Model: C-Class
       3.Color: White
       4.Fuel: Diesel
       5.Weight: 850kg
       6.Mileage: 8Kmpl
       7.Rating: 4.5
            Taking the above as reference, I'll stress up on objects, object properties and methods.
     
     1) OBJECTS:
            The following code assigns a simple value(Mercedes) to a variable named car:
            Var car ="Mercedes";
              Objects are variables too. But objects can contain many values. 
              The foolwing code assign many values(Mercedes, C-Class, White & so on) to a variable named car:
                  
                  Var car={
                    Make : "Mercedes",
                    Model : "C-Class",
                    Color : "White",
                    Fuel : Diesel,
                    Weight : "850kg",
                    Mileage : "8kmpl",
                    Rating : 4.5
                    }
       The values are written as name:value pairs (name & value separated by a colon).
      
  Syntax:
          Var<object-name>={Key1:value1, Key2:value2,.......keyN:valueN};
  
  So, conclusion and definition for Javascript objects is "Javascript objects are containers for named values".
  
 2) OBJECTS PROPERTIES:
            The name:value pairs (in Javascript objects ) are called properties.
            Var car={
                   Make : "Mercedes",
                   Model : "C-Class",
                   Color : "White",
                   Fuel : Diesel,
                   Weight : "850kg",
                   Mileage : "8kmpl",
                   Rating : 4.5
               }
     From the above snippet, let's have a look what falls under property and property value.
  
                Property          Property Value
                  Make             Mercedes
                  Model            C-Class
                  Color            White
                  Fuel            Diesel
                  Weight          850kg
                  Mileage         8kmpl
                  Rating          4.5

 The object properties can be different primitive values, other objects and functions. Properties can usually be changed, added and deleted, but some are read only.
    The syntax for adding a property to an object is :
      ObjectName.ObjectProperty=propertyValue;
    The syntax for deleting a property from an object is:
      deleteObjectName.ObjectProperty;
  The syntax to access a property  from an object is:
      ObjectName.property                         //car.Make
          //or
      ObjectName["property"]                      //car["make"]
          //or
      ObjectName[expression]                      //x="Make"; car[x]
  
So,conclusion and simple definition for Javascript properties is "properties are the values associated with a Javascript object".
  
  
3) Object Methods:
          An object method is an object property containing a function definition.
  For eg: Let's assume to start the car there will be mechanical functionality.
   
        function(){return ignition.on}
  and so similar is to stop /brake/headlights on & off, etc.
  So, conclusion and simple definition for Javascript object methods is "Methods are actions that can be performed on objects".


