
## reference variable
t="abc"

reference variable by quote

echo "$t"
echo "${t}"

## hash map as dictionary
declare -A hashmap
hashmap["key1"]="value1"
hashmap["key2"]="value2"

val1="${hashmap["key1"]}"
val2="${hashmap["key2"]}"

echo "$val1" "$val2"

iterate hashmap
for i in "${!hashmap[@]}"
do
  echo "key  : $i"
  echo "value: ${hashmap[$i]}"
done

## compare string and if else

if [ "$val" == "hello" ]; then
	echo "hello"
elif [ "$val" == "world" ]
    echo "world"
fi


## jq command
raw lines to array
if test.txt is like:
    aaaaa
	bbbbb
	
> jq --raw-input --slurp 'split("\n")' test.txt
   ["aaaaa",
   "bbbbb"
   ""
   ]
   
> jq --raw-input --slurp 'split("\n")|.[0:-1]' test.txt   
   '| [0:-1]' is to remove last line 
   ["aaaaa",
   "bbbbb"
   ]
    
