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