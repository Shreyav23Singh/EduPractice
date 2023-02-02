# EduPractice
This is my first repository
Hii

DOM Manipulation in JS - GetElementByTagName 
var li=document.getElementsByTagName('li');
console.log(li);
//we can access individual item also
console.log(li[0]);
console.log(li[1]);
console.log(li[2]);

// we can change the textcontent also
li[0].textContent='Shreya work HARD to achieve SUCCESS and fulfill your dreams';
li[1].textContent='Mobile-APRIL';
li[2].textContent='Home - 2023';
li[3].textContent='Fortuner - 2025';


li[0].style.backgroundColor='yellow';
li[0].style.borderColor='black';
li[0].style.borderWidth="5px";
li[1].style.backgroundColor='red';
li[1].style.borderColor='green';
li[1].style.borderWidth="5px";
li[1].style.color='white';
li[2].style.backgroundColor='blue';
li[2].style.color='white'
li[2].style.borderColor='cyan';
li[2].style.borderWidth="5px";
li[3].style.backgroundColor='orange';
li[0].style.fontWeight='bold';
li[3].style.borderColor='grey';
li[3].style.borderWidth="5px";


//********* ---/Get elemet by class name---*********** */

//Suppose we have to get items by class name as all these items have class name
  /*   var items=document.getElementsByClassName('list-group-item');
    console.log(items);
    //we can access individual item also
    console.log(items[0]);
    console.log(items[1]);
    console.log(items[2]);
    //we can change the textcontent also
    items[1].textContent='Fortuner';
    items[0].textContent='Shreya Word HARD to achieve your Success';
    items[2].textContent='Home';
    items[3].textContent='iPhone';
    //we change the style also
    items[0].style.height=10;
    items[0].style.fontWeight ='bold';
    //add background color
    items[0].style.backgroundColor='pink';
    items[1].style.backgroundColor='yellow';
    items[2].style.backgroundColor='cyan';
    items[3].style.backgroundColor='red';
    items[3].style.color='white';
 */
//If I want to change all the background color in one go 
//items.style.backgroundColor='yellow';  //this will give error


//we have to use for loop
/* for(var i=0 ; i<items.length ;i++){
    items[i].style.backgroundColor='pink';
} */

Q1.What is the advantage of queryselector's against getelementsbyclassname and getelementsbytagname
Q2.What is the difference between queryselector and queryselectorall?

//Traversing the DOM
//I am gonna grab Item list here
/* var itemList = document.querySelector('#items'); */
/* //parent node
console.log(itemList.parentElement);
itemList.parentElement.style.backgroundColor='pink';
console.log(itemList.parentElement.parentElement.parentElement); */

/* //parent Element
console.log(itemList.parentElement);
itemList.parentElement.style.backgroundColor='pink';
console.log(itemList.parentElement.parentElement.parentElement); */

/* Both parentNode and parentElement are same */

//Child Node
/* console.log(itemList.childNodes);

console.log(itemList.children);
console.log(itemList.children[1]);
itemList.children[1].style.backgroundColor='yellow';
itemList.children[2].style.backgroundColor='cyan';
itemList.children[0].style.backgroundColor='red';
itemList.children[0].style.color='white';
itemList.children[3].style.backgroundColor='orange'; */

/* //first child
console.log(itemList.firstChild);

//firstElementChild
console.log(itemList.firstElementChild);
itemList.firstElementChild.textContent='Determination'; */

/* //last child
console.log(itemList.lastChild);

//lastElementChild
console.log(itemList.lastElementChild);
itemList.lastElementChild.textContent='Consistency'; */


/* //nextSibiling
console.log(itemList.nextSibling); // It gives us the text 
//nextElementSibiling
console.log(itemList.nextElementSibling);
 */

/* //previoussibling
console.log(itemList.previousSibling)

//previousElementSibiling
console.log(itemList.previousElementSibling);
itemList.previousElementSibling.style.color="RED";
itemList.previousElementSibling.textContent="Success"; */


//createElement

//create a Div
var newDiv =document.createElement('div');

//Add Class
newDiv.className='Shreya';

//Add id
newDiv.id='Piku';

//Add attribute
newDiv.setAttribute('title' , 'Hello Div');

//create textNode
var newDivText =document.createTextNode('Hello World');

//Add text to div
newDiv.appendChild(newDivText);

var container=document.querySelector('header.container');
var h1=document.querySelector('header h1');

console.log(newDiv)
newDiv.style.fontSize ='30 px';
//container.insertBefore(newDiv,h1);
