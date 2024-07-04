# تعریف متغیرها برای ذخیره اعداد ورودی و عملگر
num1 = 0
num2 = 0
operator = ""

# دریافت عدد اول از کاربر
print("عدد اول را وارد کنید (تا سه رقم): ")
num1 = float(input())

# دریافت عملگر از کاربر
print("عملگر (+, -, *, /) را وارد کنید: ")
operator = input()

# دریافت عدد دوم از کاربر
print("عدد دوم را وارد کنید (تا سه رقم): ")
num2 = float(input())

# محاسبه نتیجه براساس عملگر انتخابی
if operator == "+":
  result = num1 + num2
elif operator == "-":
  result = num1 - num2
elif operator == "*":
  result = num1 * num2
elif operator == "/":
  if num2 != 0:
    result = num1 / num2
  else:
    print("تقسیم بر صفر غیرمجاز است!")
    result = 0
else:
  print("عملگر نامعتبر!")
  result = 0

# نمایش نتیجه
print("نتیجه:", result)
