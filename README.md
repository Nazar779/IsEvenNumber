function isEvenNumber(num1){
    /* Чтобы проверить четное число надо его поделить на 2 и проверить с остатком ли
    для этого нужно использовать оператор % деление с остатком и сравнить значение с нулем
    если число делится без остатка выводит первое сообщение иначе выполняется блок else
    */
    if(num1 % 2 === 0){
        return "Even number"
    }else{
        return "Is a not even number"
    }
}

console.log(isEvenNumber(6))// Выведет 2 поскольку 6 делится на 2 без остатка

function PositiveNumberNegative(n){
    /* В этом коде мы проверяем положительное ли число для этого мы используем
    оператор > который проверяет если число больше чем 0 значит оно положительное а иначе отрицательное
    поскольку отрицательные числа всегда меньше 0
    */
    if(n > 0){
        return "Positive number"
    }else{
        return "Negative number"
    }
}

console.log(PositiveNumberNegative(6))


function timeForMilkAndCookies(date){
    if(date.getMonth() === 11 && date.getDate() === 24){
        return true
    }else{
        return false
    }
}
console.log(timeForMilkAndCookies(new Date(2013, 11, 24)))

function matchHouses(step){
    return 6 +(step - 1) * 5
}
console.log(matchHouses(4))


function canNest(arr1, arr2){
    if(Math.min(...arr1) > Math.min(...arr2) && Math.max(...arr1) < Math.max(...arr2)){
        return true
    }else{
        return false
    }
}

console.log(canNest([1, 2, 3, 4], [0, 6]))
console.log(canNest([3, 1], [4, 0]))
console.log(canNest([9, 9, 8], [8, 9]))
