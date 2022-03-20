# <p align="center"> Leap Year 🌛
A program that works out whether a given year is a leap year. A normal year has 365 days, leap years have 366, with an extra day in February.  
  
## 🚨 This is how it work out whether if a particular year is a leap year.
`On every year that is evenly divisible by 4 
EXCEPT every year that is evenly divisible by 100 
UNLESS the year is also evenly divisible by 400`
  
- e.g. The year 2000:
  * 2000 ÷ 4 = 500 (Leap)
  * 2000 ÷ 100 = 20 (Not Leap)
  * 2000 ÷ 400 = 5 (Leap!)
  * **So the year 2000 is a leap year**.
- But the year 2100 is not a leap year because:
  * 2100 ÷ 4 = 525 (Leap)
  * 2100 ÷ 100 = 21 (Not Leap)
  * 2100 ÷ 400 = 5.25 (Not Leap)
  
  
  ![Leap_Year_Chart](https://user-images.githubusercontent.com/36781269/159159725-1ccd8f0f-4cb9-4199-a26f-8cc33add6b1d.PNG)

```python 
year = int(input("Which year do you want to check? "))
if year % 4 == 0:
  if year % 100 == 0:
    if year % 400 == 0:
      print("Leap year.")
    else:
      print("Not leap year.")
  else:
    print("Leap year.")
else:
  print("Not leap year.")
```
