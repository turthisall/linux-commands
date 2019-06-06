# linux-commands
IFS=$'\n'; for i in $(cat create.list); do /usr/bin/php create-list.php --listname="$i"; done

cat list-to-create.txt  | sort | uniq > create.list

awk 'NF' file
