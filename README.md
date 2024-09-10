# Задание 1
cut -d: -f1 /etc/passwd |sort

![image](https://github.com/user-attachments/assets/648ae0aa-0d9e-42dc-bb99-922db5931d4f)

# Задание 2
cat /etc/protocols | awk '{print $2, $1}' | sort -rn | head -n 5 | awk '{printf "%d %s\n", $1, $2}'

![image](https://github.com/user-attachments/assets/1cd8b258-c87e-4be9-9da9-39842b5528e7)

# Задание 3
