#!/bin/sh
# lock the DilkDaddies branch for pushing
refname="$1"

if [[ $refname == "refs/heads/DilkDaddies" ]]
then
    echo "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
    echo "You cannot push to DilkDaddies! It's locked"
    echo "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
    exit 1
fi
exit 0
