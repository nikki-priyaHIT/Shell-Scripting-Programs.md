# Write a shell script to show the maximum of three numbers provided as command line arguments
```shell
#!/bin/bash

echo $1 $2 $3 

if [ $# -ne 3 ]
then
echo "Invalid arguments!"

else


if [ $1 -gt $2 -a $1 -gt $3 -a $1 -ne $2 -a $1 -ne $3 ]
then
echo "The greatest number is $1"


elif [ $2 -gt $1 -a $2 -gt $3 -a $2 -ne $1 -a $2 -ne $3 ]
then
echo "The greatest number is $2"

elif [ $3 -gt $1 -a $3 -gt $2 -a $3 -ne $1 -a $3 -ne $2 ]
then 
echo "The greatest number is $3"
else
echo "All the three numbers are equal"
fi

fi
```
# Output
![shell1](https://user-images.githubusercontent.com/66662965/138910989-920e800e-0255-4eae-92cb-741b88727975.png)
