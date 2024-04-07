```javascript
// Duration: 1/2 hour 2024-03-09 12:30-2:00

const twoSum = (nums, target) => {
  let pointer = 0;
  let maxNumsLengthArray = [...nums.keys()];
  let sum;

  console.log(`Input: num = [${nums}], target = ${target}`);

  for (let i = 0; i < maxNumsLengthArray.length; i++) {
    let addIndices = [];
    let totalSums = [];
    let targetSumIndices = [];

    pointer = i;

    // iterate indexes to add with the pointer
    for (let num of maxNumsLengthArray) {
      if (num === pointer) {
        continue;
      } else {
        addIndices.push(num);
      }
    }

    for (const j of addIndices) {
      sum = nums[pointer] + nums[j];
      totalSums.push(sum);

      if (sum === target) {
        targetSumIndices.push(pointer, j);
      } else {
        continue;
      }
    }

    console.log(
      `\npointer: ${nums[pointer]} + ${nums[addIndices[0]]}, ${
        nums[addIndices[1]]
      }`
    );
    console.log(`Output: ${totalSums}`);
    console.log(`Indices: ${targetSumIndices}`);
  }
};

let testNums = [2, 3, 4];
const testTarget = 6;

twoSum(testNums, testTarget);

var inneffectivetwoSum = function (nums, target) {
  for (var i = 0; i < nums.length; i++) {
    for (var j = i + 1; j < nums.length; j++) {
      if (nums[i] + nums[j] == target) {
        console.log(i, j);
        // return [i, j];
      }
    }
  }
};

inneffectivetwoSum(testNums, testTarget);
```
