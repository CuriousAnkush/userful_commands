####Mysql Query output to CSV format
mysql db_name -h host_name -u user -p password -e command_name| sed "s/'/\'/;s/\t/\",\"/g;s/^/\"/;s/$/\"/;s/\n//g" > outputfile.txt
