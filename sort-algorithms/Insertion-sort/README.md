# Insertion Sort 
## YouTube Videos 
- [moash Hamadani](https://youtu.be/nKzEJWbkPbQ)

## solve with 
JavaScript
```javascript
let sortFun = function (array) {
        let greenArray = [array.shift()]
        array.forEach((value) => {
          let insertAt = 0
          for (
            let greenIndex = greenArray.length - 1;
            greenIndex >= 0;
            greenIndex--
          ) {
            const greenItem = greenArray[greenIndex]
            if (value > greenItem) {
              insertAt = Number(greenIndex + 1)
              greenIndex = -1
            }
          }
          greenArray.splice(insertAt, 0, value)
        })
        return greenArray
      }

```
---

back to 

[Sort Algorithms](https://github.com/resources-indexing/Introduction-To-Algorithms#sort-algorithms)

