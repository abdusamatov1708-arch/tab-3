# tab-3
# ==============================================================================
# DASTUR TAVSIFI:
# Ushbu dastur foydalanuvchidan ikkita son qabul qiladi va ular ustida to'rt asosiy
# arifmetik amalni (+, -, *, /) bajaradi. Dasturda casting (tur o'zgartirish),
# 0 ga bo'lish xavfsizligi, ma'lumot turini tekshirish va f-string formatlash ishlatilgan.
# ==============================================================================

print("=" * 50)
print("             MINI-KALKULYATOR                 ")
print("=" * 50)

# 1. Input va Casting (Kiritilgan qiymatni float turiga o'tkazamiz)
son1 = float(input("Birinchi sonni kiriting: "))
son2 = float(input("Ikkinchi sonni kiriting: "))

print("-" * 50)

# 2. type() yordamida o'zgaruvchi turlarini aniqlash va chiqarish
print(f"Birinchi o'zgaruvchi turi: {type(son1)}")
print(f"Ikkinchi o'zgaruvchi turi: {type(son2)}")

print("-" * 50)
print("ARIFMETIK AMALLAR NATIJASI:")
print("-" * 50)

# 3. Arifmetik amallar va f-string yordamida 2 ta raqamgacha yaxlitlab chiqarish
print(f"Qo'shish: {son1} + {son2} = {son1 + son2:.2f}")
print(f"Ayrish:   {son1} - {son2} = {son1 - son2:.2f}")
print(f"Ko'paytirish: {son1} * {son2} = {son1 * son2:.2f}")

# 4. Nolga bo'lishni tekshirish (Xavfsizlik)
if son2 != 0:
    bo_lish_natijasi = son1 / son2
    print(f"Bo'lish:  {son1} / {son2} = {bo_lish_natijasi:.2f}")
else:
    print("Bo'lish:  Xatolik! Sonni nolga bo'lish mumkin emas.")

print("=" * 50)
