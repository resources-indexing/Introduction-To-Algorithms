# Insertion Sort 
## YouTube Videos 
- [moash Hamadani](https://youtu.be/nKzEJWbkPbQ)



## JavaScript Employment
#### My First Employmentation
```javascript
let sortFun = function (array) {
  let first = array.shift()
  let greenArray = []
  if (first != undefined) {
    greenArray.push(first )
  }
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
#### Better Emplement 
```javascript 
let sortFun = function(array) {
  for(let i = 1; i<array.length ; i++) {
    const current = array[i]
    let j = i - 1 
    while(j>=0 && array[j] > current ) {
      array[j+1] = array[j]
      j--
    }
    array[j+1] = current
  }
}
```
---

back to 

[Sort Algorithms](https://github.com/resources-indexing/Introduction-To-Algorithms#sort-algorithms)

