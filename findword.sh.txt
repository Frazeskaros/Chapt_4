#!/usr/bin/bash


#import word
s_word="$1";
#import file
log_file="file.txt"

#searching spec word in file.txt 
count=$(grep -o -w $s_word $log_file | wc -l)


#print result
echo "$s_word found $count times"
