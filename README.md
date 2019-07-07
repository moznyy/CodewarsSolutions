
*https://www.codewars.com/kata/if-you-cant-sleep-just-count-sheep/train/javascript
```javascript
         var countSheep = function (num) {
          let newString = '';
           for (let i = 1; i <= num; i++); {
            newString = newString + i + 'sheep...';
           }
           return newString;
         }
```
*https://www.codewars.com/kata/capitalization-and-mutability/train/javascript
```javascript
function capitalizeWord(word) {
  return word[0].toUpperCase() + word.slice(1);
}
```
*https://www.codewars.com/kata/56bc28ad5bdaeb48760009b0/solutions/javascript
 ```javascript
function removeChar(str) {
  return str.slice(1, -1);
}
```
*https://www.codewars.com/kata/convert-a-string-to-an-array/train/javascript
```javascript
function stringToArray(string){
  return string.split(' ');
}
```
*https://www.codewars.com/kata/determine-offspring-sex-based-on-genes-xx-and-xy-chromosomes/train/javascript
```javascript
function chromosomeCheck(sperm) {
  return `Congratulations! You're going to have a ${sperm === 'XY' ? 'son' : 'daughter'}.`
}
```
*https://www.codewars.com/kata/thinkful-logic-drills-traffic-light/train/javascript
```javascript
function updateLight(current) {
  
  return current === 'yellow' ? 'red' : current === 'green' ? 'yellow' : 'green';

}
```
*https://www.codewars.com/kata/the-feast-of-many-beasts/train/javascript
```javascript
function feast(beast, dish) {
  return beast[0] === dish[0] && beast[beast.length - 1] === dish[dish.length - 1]
}
```
*https://www.codewars.com/kata/students-final-grade/solutions/javascript
```javascript
function finalGrade (exam, projects) {
  if(exam > 90 || projects > 10) return 100;
  if(exam > 75 & projects >= 5) return 90;
  if(exam > 50 & projects >= 2) return 75;
  return 0;
}
```
*https://www.codewars.com/kata/type-of-sum/train/javascript
```javascript
const typeOfSum = (a, b) => typeof(a + b);
```
*https://www.codewars.com/kata/sleigh-authentication/train/javascript
```javascript
function Sleigh() {}

Sleigh.prototype.authenticate = function(name, password) {
  return name === 'Santa Claus' && password === 'Ho Ho Ho!';
};
```
*https://www.codewars.com/kata/switch-it-up/train/javascript
```javascript
switchItUp=n=>["Zero","One","Two","Three","Four","Five","Six","Seven","Eight","Nine"][n]
```
```javascript
*https://www.codewars.com/kata/random-case/train/javascript
function randomCase(x) {
  return x.split('')
    .map(function(e) { return Math.random() < 0.5 ? e.toUpperCase() : e.toLowerCase(); })
    .join('');
}
```
 ```javascript
*https://www.codewars.com/kata/alphabet-symmetry/train/javascript
function solve(arr){  
  var alphabeth = "abcdefghijklmnopqrstuvwxyz";
  return arr.map(x => x.toLowerCase().split('').filter((y,i) => i==alphabeth.indexOf(y)).length);
};
```
```javascript
*https://www.codewars.com/kata/credit-card-issuer-checking/train/javascript
function getIssuer(number) {
  if (/^3[4|7]\d{13}$/.test(number)) return 'AMEX'
  if (/^6011\d{12}$/.test(number)) return 'Discover'
  if (/^5[1-5]\d{14}$/.test(number)) return 'Mastercard'
  if (/^4(\d{12}|\d{15})$/.test(number)) return 'VISA'
  return 'Unknown'
}
```
```javascript
*https://www.codewars.com/kata/create-phone-number/train/javascript
function createPhoneNumber(numbers){
  let formatPhone = [];
  for(let i=0; i<numbers.length; i++){
    if(i === 0){
      formatPhone.push('(' + numbers[i]);
    } else if(i === 2){
      formatPhone.push(numbers[i] + ')');
    } else if(i === 3){
      formatPhone.push(' ' + numbers[i]);
    } else if(i === 5){
      formatPhone.push(numbers[i] + '-');
    } else {
      formatPhone.push(numbers[i]);
    }
  }
  
  return formatPhone.join('');
}

console.log(createPhoneNumber([1, 2, 3, 4, 5, 6, 7, 8, 9, 0])); 
```
*https://www.codewars.com/kata/remove-string-spaces/train/javascript
```javascript
function noSpace(x){
  return x.replace(/\s/g, '');
}
```
*https://www.codewars.com/kata/who-is-going-to-pay-for-the-wall/train/javascript
```javascript
function whoIsPaying(name){
 return  name.length <= 2 ? [name] : [name, name.substr(0, 2)];
}
```

*https://www.codewars.com/kata/do-i-get-a-bonus/train/javascript
```javascript
function bonusTime(salary, bonus) {
  return bonus ? `£${10 * salary}` : `£${salary}`;
}
```
*https://www.codewars.com/kata/returning-strings/train/javascript
```javascript
function greet(name){
  return `Hello, ${name} how are you doing today?`;
}
```
*https://www.codewars.com/kata/string-ends-with/train/javascript
```javascript

function solution(str, ending){
  return new RegExp(ending+"$", "i").test(str);
}
```
*https://www.codewars.com/kata/print-a-rectangle-using-asterisks/train/javascript
```javascript
function getRectangleString(width, height) {
 if (width===1&&height===1) return '*\r\n'
 if (width===1&&height===2) return '*\r\n*\r\n'
  let start = '*'.repeat(width)+'\r\n'
  let mid = '*'+' '.repeat(width-2)+'*'+'\r\n'
  let end = mid.repeat(height-2)
  return start+end+start
}
```
*https://www.codewars.com/kata/string-average/train/javascript
```javascript
function averageString(str) {
  const num = {zero:0,one:1,two:2,three:3,four:4,five:5,six:6,seven:7,eight:8,nine:9}
  const word = {0:'zero',1:'one',2:'two',3:'three',4:'four',5:'five',
  6:'six',7:'seven',8:'eight',9:'nine'}
  if (!str.length) return 'n/a'
  let n=0
  const l=str.split(' ').length
  const arr=str.split(' ').map(v=>num.hasOwnProperty(v)?v=num[v]:n=1).reduce((a,b)=>a+b,0)
  return n===0?word[Math.floor(arr/l)]:'n/a'
}
```
*https://www.codewars.com/kata/are-we-alternate/train/javascript
```javascript
function isAlt(word) {
 
  return word.split('').every((v,i)=>{
  if (/[aeiou]/.test(word[0])){
    if (i%2===0&&/[aeiou]/.test(v)){
      return true
      } else if (i%2!==0&&!/[aeiou]/.test(v)){ return true
      } else {return false}
    }
  if (!/[aeiou]/.test(word[0])){
    if (i%2==0&&!/[aeiou]/.test(v)){
      return true
      } else if (i%2!==0&&/[aeiou]/.test(v)){ return true
      } else {return false}
    }
  })
}
```
*https://www.codewars.com/kata/ordering-the-words/train/javascript
```javascript

function orderWord(s){
 return !s||s.length==0?"Invalid String!":s.split('').sort().join('')
}
```
*https://www.codewars.com/kata/shortest-word/train/javascript
```javascript
function findShort(s){
    return Math.min(...s.split(" ").map (s => s.length));
}
```
*https://www.codewars.com/kata/double-char/train/javascript
```javascript
function doubleChar(str) {
  return str.split("").map((letter) => `${letter}${letter}`).join("");
}
```
*https://www.codewars.com/kata/convert-boolean-values-to-strings-yes-or-no/train/javascript
```javascript
function boolToWord( bool ){
 return bool ? 'Yes':'No';
}
```
*https://www.codewars.com/kata/fix-string-case/train/javascript
```javascript
function solve(s){
    let up=s.split('').filter(v=>v.match(/[A-Z]/)).length
    let down=s.split('').filter(v=>v.match(/[a-z]/)).length
    return down>=up?s.toLowerCase():s.toUpperCase();
}
```
*https://www.codewars.com/kata/bit-counting/train/javascript
```javascript
var countBits = function(n) {
  return n.toString(2).replace(/0/g,'').length;
};
```
*https://www.codewars.com/kata/fake-binary/train/javascript
```javascript
function fakeBin(x) {
    return x.split('').map(n => n < 5 ? 0 : 1).join('');
}
```

 
