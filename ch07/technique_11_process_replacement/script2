#!/bin/bash
# Redirect stdout for this script
exec > /tmp/outfile2
# All subsequent commands print to /tmp/outfile2
echo "My name is $USER"
echo "My current directory is $PWD"
echo "Guess how many lines are in the file /etc/hosts?"
wc -l /etc/hosts
echo "Goodbye for now"
