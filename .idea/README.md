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
