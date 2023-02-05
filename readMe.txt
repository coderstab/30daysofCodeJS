1 => How to find duplicate elements in an array?
Ans => 
let arr = [2,2,3,4,4,5,7,7];
let resArr= [];
let index = 0;
let length = arr.length;
function funFind(arr){
for(i=0;i<length-1;i++){
     for(j=i+1;j<length;j++){
          if(arr[i]===arr[j]){
              resArr[index] = arr[i];
              index++;
          }
     }
}
console.log(resArr)
}
funFind(arr);
2 => How to remove duplicate elements in an array?
Ans => 
var arr = ["apple", "mango", 
        "apple", "orange", "mango", "mango"];
        var resArr = [];
  
    function funRem(arr){
        for(let i=0;i<arr.length;i++){
            if(resArr.indexOf(arr[i]) === -1){
                resArr.push(arr[i]);
            }
        }
        console.log(resArr)
        
    }
    funRem(arr)
    
3 => Counting the occurrences / frequency of array elements
Ans => 
var arr= [5, 5, 5, 2, 2, 2, 2, 2, 9, 4];
result = { };
function funFrq(arr){
      for(var i=0;i<arr.length;i++){
          if(!result[arr[i]]){
              result[arr[i]] = 0;
              ++result[arr[i]]
          }
      }
      console.log(result);
}
funFrq(arr)
