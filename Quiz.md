# 判斷完全數
```
function isComplete (n) {
    let arr = [] 
	  for (var i=1; i<=n; i++) {
  	  if (n % i === 0) {
    	arr.push(i)  // 找出所有因數並放到 array      
      } 
    }
    let len = arr.length // 所有因數的數量
    let sum = 0
    for (var i=0; i<len-1; i++) {
  	  sum += arr[i] // 將所有因數相加
    }
    if (arr[len-1] === sum) {
      return true
    } else {
      return false
    }    
}
isComplete(6) // true
isComplete(39) // false
```
