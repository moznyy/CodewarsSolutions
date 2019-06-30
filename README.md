
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