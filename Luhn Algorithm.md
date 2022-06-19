# Luhn Algorithm
![For more information, click here](https://en.wikipedia.org/wiki/Luhn_algorithm)
给出一个信用卡号 `c_number`：
1. 首先，记下最后一位：`var check`
2. 然后，从第一位开始：
```
sum = 0
while second last position not reached:
  if position is odd: sum += position
  else:
    double = c_number[position]*2
    sum += double%10
    double -= double %10
    double = double/10
    sum += double
waiting_to_check = 10-sum%10
if(waiting_to_check == check): return true
else return false
```
