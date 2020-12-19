# NiluShinde
assignment part-1
a=`ls /csvserver/solution*`


my_arr=()
for i in $a
do
        my_arr+=("$i")

done

#echo "${my_arr[@]}"

for i in "${!my_arr[@]}"; do
  echo "$i,${my_arr[$i]}"
done>inputFile
