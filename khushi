#!/bin/bash

# Run git remote -v command and store the output in a variable
remote=$(git remote -v)

# Extract the first line from the output
first_line=$(echo "$remote" | sed -n '1p')

# Check if the first line is empty or contains "github.com:yandex-praktikum"
if [ -z "$first_line" ] || [[ "$first_line" == *"github.com:yandex-praktikum"* ]]; then
    echo "Упс. Кажется, вы не сделали Fork репозитория!"
else
    echo "Секретный ключ: practicum"
fi
