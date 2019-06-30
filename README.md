
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