Var:
•	can be declared outside any function to be used inside any function
•	can be declared inside any function or any other {} which are of only if or if -else or switch etc. and can be used anywhere inside the function
•	can be changed again and again anywhere


// var is a function scope
if(true){
    var varVariable = 'This is var';
    var varVariable = 'This is var again';
}

console.log(varVariable);




Q1 Explain difference between var/ let const by giving examples. ?

Let:
•	can be declared outside any function to be used inside any function
•	if declared inside any function or any other {} which are of only if or if-else or switch etc. and can't be used anywhere inside the function and can be only used inside statement
•	can be changed again and again only inside the statement in which they are made in


	       // let is a block scope
                       if(true){
	      let letVariable = 'This is let';

 	      // let variable can't re-define but we can re-assign value




Const:
•	can be declared outside any function to be used inside any function
•	can be declared inside any function or any other {} which are of only if or if-else or switch etc. and can be used anywhere inside the function
•	cannot be changed again and agan anywhere, if tried to, will result in an error
 


//const variable can't re-define and re-assign value
if(true){
    const constVarible = {
        name: 'JavaScript',
        age: '25 years',
    };
    constVarible.name = 'JS';

    console.log(constVarible) // {name: 'JS',age: '25 years'} <= we can update const variable declared object 
}
