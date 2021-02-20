Hello

==============================
1 Solution
function solution(str) {
let splitString = str.split('');
let reverseArray = splitString.reverse();
let joinArray = reverseArray.join('');
return joinArray;
}
2 Solution
function solution(str){
return str = str.split('').reverse().join('');
}
=============================
Square(n) Sum
function squareSum(numbers){
return numbers.reduce(function(sum, n){
return (n*n) + sum;
}, 0)
}
==============================
Capitalization and Mutability
function capitalizeWord(word) {
var str = word[0].toUpperCase();
for (let i = 1; i<word.length; i++) {
str += word[i];
}
return str;
}
==============================
function SmallestIntegerFinder(numbers) {
let min = numbers[0];
for (let i = 1; i < numbers.length; i++){
if (numbers[i] < min ){
min = numbers[i];
}
}
return min;
}
console.log(SmallestIntegerFinder([78,56,232,12,0]))

==============================
function reverseList(list) {
let arr = [];
for (let i = list.length - 1; i >= 0; i --){
arr.push(list[i]);
}
return arr;
}
==============================
var countSheep = function (num){
let sheep = '';
for (let i = 1; i <= num; i++){
sheep = sheep + i + ' ' + 'sheep...';
}
return sheep;
}
console.log(countSheep(3));
==============================
function createPhoneNumber(numbers){
numbers.unshift("(");
numbers.splice(4, 0, ")", " ");
numbers.splice(9, 0, "-");
return numbers.join("");
}
==============================
function whoIsPaying(name){
let arr= [name];
if (name.length >= 2) {
arr.push(name.slice(0, 2));
}
return arr;
}
console.log(whoIsPaying("I"))
==============================
function bonusTime(salary, bonus) {
return `£${salary * (bonus ? 10 : 1)}`;
}
console.log(bonusTime(10000, false));
==================================
function averageString(str) {
if (str === '') return 'n/a';
let arr1 = str.split(' ');
let arr = [];
for (let i of arr1) {
switch (i) {
case 'zero':
arr.push(0);
break;
case 'one':
arr.push(1);
break;
case 'two':
arr.push(2);
break;
case 'three':
arr.push(3);
break;
case 'four':
arr.push(4);
break;
case 'five':
arr.push(5);
break;
case 'six':
arr.push(6);
break;
case 'seven':
arr.push(7);
break;
case 'eight':
arr.push(8);
break;
case 'nine':
arr.push(9);
break;
default: return 'n/a';
}
}
let num = 0;
for (let num1 of arr) {
num += num1;
}
num = Math.floor(num / arr.length);
switch (num) {
case 0:
str = 'zero';
break;
case 1:
str = 'one';
break;
case 2:
str = 'two';
break;
case 3:
str = 'three';
break;
case 4:
str = 'four';
break;
case 5:
str = 'five';
break;
case 6:
str = 'six';
break;
case 7:
str = 'seven';
break;
case 8:
str = 'eight';
break;
case 9:
str = 'nine';
break;
}
return str;
}
=====================
plus one KATA
function solve(s) {
let a = 0;

for (let letter of s.split('')) {
if (letter === letter.toUpperCase()) a += 1;
}
if (a > s.length/2) {
return s.toUpperCase();
} else {
return s.toLowerCase();
}
}
==========================

function rgb(r, g, b){
return [r,g,b].map(function(x) {
return ('0'+Math.max(0, Math.min(255, x)).toString(16)).slice(-2);
}).join('').toUpperCase();
}
============================
function getCount(str) {
str = str.replace(/a|e|i|o|u/g, "!").split("!").length - 1;
return str;
}
console.log(getCount("abracadabra"));
