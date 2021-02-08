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