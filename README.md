# linux-commands
IFS=$'\n'; for i in $(cat create.list); do /usr/bin/php create-list.php --listname="$i"; done

cat list-to-create.txt  | sort | uniq > create.list

awk 'NF' file

awk 'BEGIN{FS=OFS="."} NR==FNR{a[$1]=$NF;next;} $2 in a {print $1,a[$NF]}' list1.txt list2.txt


grep -Ff list1 list2
