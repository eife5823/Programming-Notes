### 判斷完全數
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
### 大數加法
```
function add(a, b) {
  a = a.split('').reverse(); // a= ["4", "3", "2", "1"]
  b = b.split('').reverse(); // b = ["9", "8", "7", "6", "5"]

  var result = [];
  var length = Math.max(a.length, b.length); // 取兩個數字中最大的 length 決定要跑幾圈迴圈
  var carry = 0;
  for (var  i = 0; i < length; i++) {
  
    /* 跑到第二圈時才會開始把進位加進去數字 */
    var sum = parseInt(a[i] || 0 ) + parseInt(b[i] || 0 ) + carry; // sum = 每個元素總和+進位 (數字位數可能不同所以要補 0)
    result[i] = sum % 10; // 新陣列的每個元素為(元素總和+進位)除以10的餘數
    carry = (sum - result[i]) / 10; // 進位=(元素總和-餘數) /10
  }

  if (carry) {
    result.push(carry); // 迴圈結束後若還有進位要再push進位到新陣列
  }

  return result.reverse().join('');
}  
```
### 打不倒的空氣人
```
function pc (arr1, arr2) {
  let newArr = arr1.join('').split(''); // ["a", "b", "c", "d", "e", "f"]
  let len = arr2.length
  let result = ""; //結果是一個字串，要注意在迴圈外面宣告
  for (var i=0; i<len; i++) {
    var index = arr2[i]-1; // 0 3    
    result += newArr[index]; // 每跑完一圈就將字母放進 result 裡   
  }
  return result;     
}

console.log(pc(['ab', 'cd', 'ef'], [1, 4, 5])); //ad
```
