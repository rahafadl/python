# 🟢 الدرس 1: المتغيرات، المدخلات، والمخرجات في بايثون

## 📌 ما هي المتغيرات؟
المتغيرات هي "صناديق" نخزن فيها معلومات. كل صندوق له اسم، ونقدر نغير محتواه متى ما نريد.

### ✅ مثال:
```python
الاسم = "سارة"
العمر = 12
```
هنا خزنا الاسم داخل متغير اسمه `الاسم`، وخزنا رقم داخل متغير اسمه `العمر`.

## 📥 المدخلات (Input)
لو نريد المستخدم يكتب لنا شيء، نستخدم دالة `input()`.

### ✅ مثال:
```python
الاسم = input("ما اسمك؟ ")
print("أهلاً يا " + الاسم)
```

## 📤 المخرجات (Output)
نستخدم `print()` عشان نطبع أي شيء على الشاشة.

### ✅ مثال:
```python
print("مرحبًا بالعالم!")
```

## 🧠 تدريب صغير:
1. أنشئ متغيرًا اسمه `البلد` وضع فيه اسم بلدك.
2. اطبع جملة تقول: "أنا من [اسم البلد]".
3. اطلب من المستخدم عمره، ثم اطبع: "عمرك هو: [العمر] سنة".

### 📝 مثال متكامل:
```python
البلد = "السعودية"
print("أنا من " + البلد)

العمر = input("كم عمرك؟ ")
print("عمرك هو: " + العمر + " سنة")
```

---

# 🟡 الدرس 2: أنواع البيانات والمعاملات في بايثون

## 🧱 أنواع البيانات الأساسية:
1. **النصوص (Strings)**: كلمات أو جُمل بين علامتي اقتباس.
   - مثال: "مرحبا", 'Python'

2. **الأعداد الصحيحة (Integers)**: أعداد بدون فاصلة.
   - مثال: 5, 100, -3

3. **الأعداد العشرية (Floats)**: أعداد تحتوي على فاصلة عشرية.
   - مثال: 3.14, 0.5

4. **القيم المنطقية (Booleans)**: تعبر عن صح أو خطأ.
   - مثال: True, False

## ➕ المعاملات (Operators):

### 🔢 المعاملات الرياضية:
- + للجمع
- - للطرح
- * للضرب
- / للقسمة
- // قسمة عدد صحيح (بدون فاصلة)
- % باقي القسمة (modulus)
- ** الأس (الرفع للقوة)

### ✅ أمثلة:
```python
x = 10
y = 3

print(x + y)  # 13
print(x - y)  # 7
print(x * y)  # 30
print(x / y)  # 3.333...
print(x // y) # 3
print(x % y)  # 1
print(x ** y) # 1000
```

## 🧠 تدريب صغير:
1. عرف متغيرين لأعداد.
2. اطبع نتيجة جمعهم وضربهم.
3. جرب باقي العمليات الرياضية.

---

# 🔵 الدرس 3: القوائم (Lists) في بايثون

## 📚 ما هي القوائم؟
القائمة هي مجموعة من العناصر، نقدر نخزن فيها أشياء كثيرة داخل متغير واحد.

### ✅ مثال:
```python
الطلاب = ["علي", "سارة", "محمد"]
الأعمار = [10, 12, 11]
```

## 🎯 الوصول إلى عناصر القائمة:
نبدأ العد من الصفر!
```python
print(الطلاب[0])  # علي
print(الطلاب[1])  # سارة
```

## ✏️ تعديل عنصر في القائمة:
```python
الطلاب[1] = "هدى"
```

## ➕ إضافة عناصر:
```python
الطلاب.append("نورة")
```

## ❌ حذف عناصر:
```python
الطلاب.remove("محمد")
```

## 🧠 تدريب صغير:
1. أنشئ قائمة فيها 3 أشياء تحبها.
2. اطبع العنصر الثاني.
3. غير العنصر الأول.
4. أضف عنصر جديد.
5. احذف عنصرًا من القائمة.

---

# 🟣 الدرس 4: Tuple والـ Dictionary

## 📦 الـ Tuple:
هي مثل القائمة، لكن ما نقدر نغير عناصرها.
```python
الأيام = ("الأحد", "الاثنين", "الثلاثاء")
print(الأيام[0])
```

## 🔑 القواميس (Dictionary):
فيها أزواج: **مفتاح (Key)** و **قيمة (Value)**.
```python
الطالب = {
    "الاسم": "سارة",
    "العمر": 12,
    "الصف": "سادس"
}
```

### 📌 الوصول للمفاتيح والقيم:
```python
print(الطالب["الاسم"])
print(الطالب.get("العمر"))
```

## 🧠 تدريب صغير:
1. أنشئ Tuple يحتوي 3 فصول دراسية.
2. أنشئ Dictionary لطالب: الاسم والعمر والصف.
3. اطبع اسم الطالب من القاموس.

---

# 🔶 الدرس 5: الشروط (If)

## ❓ نستخدم if لاتخاذ قرار بناءً على شرط:
```python
العمر = 15
if العمر >= 18:
    print("أنت بالغ")
else:
    print("أنت صغير")
```

## 🧠 تدريب صغير:
1. اطلب من المستخدم عمره.
2. إذا كان 18 أو أكثر، قل له "مسموح لك الدخول".
3. غير ذلك، قل له "ممنوع الدخول".

---

# 🔁 الدرس 6: التكرار (Loops)

## 🔄 for loop:
```python
الأسماء = ["سارة", "علي", "نورة"]
for اسم in الأسماء:
    print("مرحبًا " + اسم)
```

## 🔁 while loop:
```python
عدد = 1
while عدد <= 3:
    print("العدد هو: ", عدد)
    عدد += 1
```

## 🧠 تدريب صغير:
1. أنشئ قائمة بـ 3 أشياء.
2. اطبع كل عنصر باستخدام for.
3. اطبع الأرقام من 1 إلى 5 باستخدام while.

---

# 🟩 الدرس 7: الدوال (Functions)

## 🧠 ما هي الدالة؟
هي مجموعة أوامر نعطيها اسم، ونقدر نستدعيها أكثر من مرة.

### ✅ مثال:
```python
def حيّا(الاسم):
    print("أهلاً وسهلاً يا " + الاسم)

حيّا("سارة")
حيّا("علي")
```

## 🧠 تدريب صغير:
1. أنشئ دالة ترحب بالمستخدم.
2. أنشئ دالة تأخذ رقمين وتطبع مجموعهم.

---

# 🏁 مشروع تطبيقي: إنشاء دليل هاتف

## 🎯 الهدف:
بناء برنامج يُمثل دليل الهاتف، بحيث:
- المستخدم يُدخل رقم هاتف ويبحث عن اسم صاحبه.
- أو يُدخل اسم شخص ويبحث عن رقمه.
- أو يُضيف شخص جديد مع رقمه.
- ويتحقق من صحة الرقم (10 أرقام، كلها أرقام).

## ✅ الكود:
```python
phone_book = {
    "1111111111": "Amal",
    "2222222222": "Mohammed",
    "3333333333": "Khadijah",
    "4444444444": "Abdullah",
    "5555555555": "Rawan",
    "6666666666": "Faisal",
    "7777777777": "Layla"
}

def is_valid_number(number):
    return len(number) == 10 and number.isdigit()

def find_name_by_number():
    number = input("📞 أدخل الرقم: ")
    if is_valid_number(number):
        if number in phone_book:
            print("👤 الاسم: ", phone_book[number])
        else:
            print("❌ الرقم غير موجود")
    else:
        print("⚠️ الرقم غير صحيح")

def find_number_by_name():
    name = input("👤 أدخل الاسم: ")
    for number, owner in phone_book.items():
        if owner.lower() == name.lower():
            print("📞 الرقم: ", number)
            return
    print("❌ الاسم غير موجود")

def add_new_contact():
    name = input("👤 الاسم الجديد: ")
    number = input("📞 الرقم الجديد: ")
    if is_valid_number(number):
        phone_book[number] = name
        print("✅ تم إضافة جهة الاتصال")
    else:
        print("⚠️ الرقم غير صحيح")

# تجربة الدوال:
find_name_by_number()
find_number_by_name()
add_new_contact()
```

هذا المشروع يغطي كل المفاهيم الأساسية ويعطي تجربة حقيقية لبناء تطبيق بسيط 🎯📱

