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
funFind(arr)
