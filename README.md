# Week - 1
```
let arr1 = ['2', 'a', '3', 3, 4, 3, 5, 5]
let arr2 = ['c', 'c', 'h', 1, 1, 1, 4]
let arr3 = [
    { name: 'ali', id: 221 },
    { name: 'veli', id: 343 },
    { name: 'konya', id: 333 },
    { name: 'ali', id: 664 },
    { name: 'selim', id: 112 }
]
let arr4 = [1, 1, 1, 4, 5, 5, 3, 2]
/* 
1- arr1 başına 'a' elemanını ekleyiniz
2- arr1 sonuna 6 elemanını ekleyiniz
3- arr1 sonundaki elemanı siliniz
4- arr1 başındaki elemanı siliniz
5- arr1 ile arr2 arraylerini iki farklı yöntemle birleştiriniz
6- kendisine gönderilen arrayde verilen elemanın olup olmadığını bulan array ve 
    aranan eleman olmak üzere iki parametre alan ve geriye boolean değer döndüren bir fonksiyon yazınız
    ve bu fonkisiyona arr2 ve 'h' parametresini verip çağırınız
7- arr2 içindeki 'h' elemanın indexsini bulunuz
8- arr2 nin eleman sayısını 3 adete 2 faklı yöntemle düşrünüz
9- kendisine verilecek array elemanlarını döngü ile dönüp, array içindeki number
    değerlerinin toplamını geriye dönen bir fonkiyon yazınız ve arr1 değeri ile çağırınız   
10- arr1 elemanlarını string değere çeviren bir map fonksiyonu yazınız    
11- arr3 içindeki id değeri 221 olan elemanı bulunuz
12- arr3 içindeki user değerleri ali olan elemanları bulunuz
13- arr3 içindeki elemanlarının id değerlerinin toplamlarını bulan bir reduce fonsiyonu yazınız
her sorunun cevabını console.log ile yazıdırın
*/

//1

let first = arr1
first.unshift('a')
console.log(first)
2
let second = arr1
second.push('a')
console.log(second)
//3
let third = arr1
third.pop()
console.log(third)
//4
let forth = arr1
forth.shift()
console.log(forth)
//5
let arr5 = arr1.concat(arr2)
let arr6 = [...arr1,...arr2]
console.log(arr5,arr6)
//6
function sixth(arr2,h){
    return (arr2.includes(h))
}
//7
console.log(arr2.indexOf('h'))
//8
console.log(arr2.slice(0,3))

arr2.length=3
console.log(arr2)
//9
function nineth(arr1){
    var sum=0;
    for(let i=0;i<arr1.length;i++)
    {
        if(typeof arr[i]=='number')
        {
            sum+=arr[i]
        }
    }
    return sum
}
console.log(nineth(arr1))
//10
function tenth(arr1){
    let arr2 = arr1.map(i=>i.toString())
    return arr2
}
console.log(tenth(arr1))
//11
console.log(arr3.find(i=>i.id==221))
//12
console.log(arr3.filter(i=>i.name=='ali'))
//13
const sumId = arr1.reduce(
    (previousValue, currentValue) => previousValue + currentValue.id,
    0
  );
console.log(sumId)
}
```
# Homework 
Basic Array methods


## Homework Description

Completed questions with desired solutions


## Author

Cenk Buker
