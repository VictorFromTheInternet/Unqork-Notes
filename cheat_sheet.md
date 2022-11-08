# Table of Contents
* [Formulas: calc and init](#formulas-for-calc-and-init)
  * [Moment JS](#moment-js)
  * [Excel](#excel)
* [Formulas: DWFs](#formulas-for-calc-and-init)



<br>
<br>
<br>

# Formulas: for Calc and Init

### Moment JS
Use Case     | Formula/URL | Description
:----------:|:-------------:|:---------------:
 Diff, years (age)  |   =moment(moment(),'diff',moment(*varDateInput*),'years')        | calculates the diff from todays date to the input/var date
 Diff, days         | =moment(moment(*var1*),'diff',moment(*var2*),'days')             | formula is set to diff in 'days' (can also be 'years','months', 'seconds')
 Format, timestamp            | =moment(moment(),'format','DD MM YYYY hh:mm:ss a')     | current date/time timestamp format, ex: 04 11 2022 11:52:00 am
 Format, calander day         | =moment(moment(A),'format','dddd')                     | returns the calender day, ex: Sunday, Monday, etc.
 Format, calender timestamp   | =moment(moment(A),'format','LLLL')                     | returns the following format:  Sunday, September 18, 2022 7:00 PM  
 Today, timestamp             | =today()                                               | returns timestamp, ex: Thu Sep 23 2020 16:01:36 GMT-0400 (Eastern Daylight Time) 
 
 
 
 * https://momentjs.com/
 * https://docs.unqork.io/Content/A05-ModEditor-Data_Event/A05007I-Calculator_UseCase_MomentJS.htm

<br>
<br>
<br>

### Excel 
#### String Formulas
Use Case     | Formula/URL | Description
:----------:|:-------------:|:---------------:
Uppercase to lowercaser   |  =tolowercase(A)       | converts string to lowercase
Lowercase to Uppercase    |  =toUppercase(A)       | converts string to uppercase
Convert type to string    |  =text(A)              | input to text
Concat                    |  =concatenate(A , B)   | adds/concats two strings
Create/return a Substring          |  =mid(A,*start*,*size*)   |  A is the original string, start will be the first index of the substr, size will be the length of the substr ( ex: A='abcdefg' -> mid(A, 1, 4) -> 'bcde')



#### int Formulas
Use Case     | Formula/URL | Description
:----------:|:-------------:|:---------------:
Convert to char | char(A) | int input to char
Convert to int | value(A) | string to int/num
Generate rand num |  randbetween(A , B) | generates a random number between a-b

<br>
<br>
<br>

# Common Component Configurations
