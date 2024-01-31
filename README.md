# Код калькулятора
def додавання(x, y):
    return x + y

def віднімання(x, y):
    return x - y

def множення(x, y):
    return x * y

def ділення(x, y):
    if y != 0:
        return x / y
    else:
        return "Ділення на нуль!"

# Введення користувача
операція = input("Виберіть операцію (+, -, *, /): ")
число1 = float(input("Введіть перше число: "))
число2 = float(input("Введіть друге число: "))

# Виконання операції
if операція == '+':
    результат = додавання(число1, число2)
elif операція == '-':
    результат = віднімання(число1, число2)
elif операція == '*':
    результат = множення(число1, число2)
elif операція == '/':
    результат = ділення(число1, число2)
else:
    результат = "Невірна операція"

# Виведення результату
print("Результат: ", результат)
