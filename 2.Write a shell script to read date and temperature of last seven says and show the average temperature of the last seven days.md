# Write a shell script to read date and temperature of last seven says and show the average
temperature of the last seven days

```shell
#!/bin/bash

echo "Please start entering the values of the temperature of the last 7 days"

for((i=7;i>0;i--))
do
dat=$(date '+%d/%m/%Y' -d "-$i days")

echo "Enter the temperature for date $dat"
read temp
sum=$((sum+temp))
done


echo "Average Temperature is"
echo "scale=2;$sum/7"|bc
```
