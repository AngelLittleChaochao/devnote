
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

## compare string and if else

if [ "$val" == "hello" ]; then
	echo "hello"
elif [ "$val" == "world" ]
    echo "world"
fi

