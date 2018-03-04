# Course 1

#some useful scripts

#1 hours and rates for 40 hour work week and 1.5 overtime pay above 40 total hours
try: 
  sh = input('Enter Hours: ')
  sr = input('Enter Rate: ')
  fh = float(sh)
  fr = float(sr)
except ValueError:
  print('Please enter valid input')

if fh > 40:
  regular = fr * fh
  overtime = (fh - 40) * (fr * 0.5)
  total = regular + overtime
else:
  total = fh * fr
print('Pay:', total)
