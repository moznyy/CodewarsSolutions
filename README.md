
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

 
