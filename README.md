# Задание 1
cut -d: -f1 /etc/passwd |sort

![image](https://github.com/user-attachments/assets/648ae0aa-0d9e-42dc-bb99-922db5931d4f)

# Задание 2
cat /etc/protocols | awk '{print $2, $1}' | sort -rn | head -n 5 | awk '{printf "%d %s\n", $1, $2}'

![image](https://github.com/user-attachments/assets/1cd8b258-c87e-4be9-9da9-39842b5528e7)

# Задание 3
#!/bin/bash
# Проверяем, был ли передан аргумент

if [ $# -eq 0 ]; then

    echo "Использование: $0 \"Ваш текст\""

    exit 1

fi

# Получаем текст из аргумента

text="$1"

# Вычисляем длину текста

length=${#text}

# Создаем верхнюю и нижнюю границы

border=$(printf "%0.s-" $(seq 1 $((length + 2))))

border="+$border+"

# Выводим баннер

echo "$border"

echo "| $text |"

echo "$border"
![image](https://github.com/user-attachments/assets/3d750aee-83f7-41d7-9b11-8082cd58d1d3)

![image](https://github.com/user-attachments/assets/d6f55d3e-1e0a-42df-8b00-0bf753cc54af)

# Задание 4
grep -oE '\b[a-zA-Z_][a-zA-Z0-9_]*\b' hello.go | grep -vE '\b(int|void|return|if|else|for|while|include|stdio)\b' | sort | uniq

![image](https://github.com/user-attachments/assets/c267db17-ec12-405b-aee0-28a6f761e2dc)

# Задание 5

chmod +x reg
./reg banner




# Задание 6
chmod +x check_comment.sh
./check_comment.sh

