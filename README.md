
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