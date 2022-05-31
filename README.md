prodStartTime="123900"
prodEndTime="124500"

currentTime=`date +"%H%M%S"`
echo $prodStartTime
echo $prodEndTime
echo $currentTime

if [[ ! ( "$currentTime" < "$prodStartTime" || "$currentTime" > "$prodEndTime" ) ]]; then
   echo "--->"
fi

