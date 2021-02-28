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
function capitalizeWord(word) {
word = word[0].toUpperCase().concat(word.substring(1, word.length));
return word;
}
==============================
function check(a,x){
return a.includes(x);
};
=============================
function sortMyString(S) {
let evenS = S.split('').filter((x,i) => i % 2).join('')
let oddS = S.split('').filter((x,i) => !(i % 2)).join('')
return oddS + ' ' + evenS
}
===========================
const check = (a, x) => a.find( a => a === x ) === x;
console.log(check([80, 117, 115, 104, 45, 85, 112, 115], 45));

const arraySum = arr => arr.reduce((res, el) => res + (Array.isArray(el) ? arraySum(el) : el), 0);
without pass of letters
============================
function arraySum(arr){
arr = arr.join().split(',').map(el => el * 1)
.filter(el => !isNaN(el))
return arr.reduce((res, el) => res + (Array.isArray(el) ? arraySum(el) : el), 0);
}
========================
function checkTheBucket(bucket){
return bucket.includes('gold');
}
=========================
function invert(array) {
return array.map(e=> e*-1);
}
=========================
function distinct(a) {
return a.filter((item, index) => a.indexOf(item) === index);
}
===========================
Short Average of Array
const avg = (a) => a.reduce((p, c) => p + c) / a.length
=====================================
REACT
var styles = React.StyleSheet.create({
text: {
color: 'black',
backgroundColor: 'white',
fontSize: 30,
margin: 80
}
});
class PropertyFinderApp extends React.Component {
render() {
return React.createElement(React.Text, {style: styles.text}, "Hello World!");
}
}