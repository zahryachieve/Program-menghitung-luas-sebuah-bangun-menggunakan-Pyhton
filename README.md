# Program-menghitung-luas-sebuah-bangun-menggunakan-Pyhton
Membuat sebuah program untuk menghitung  luas sebuah bangun menggunakan python
def get_float_input(prompt):
    while True:
        try:
            return float(input(prompt))
        except ValueError:
            print("Input tidak valid. Harap masukkan angka.")

alas = get_float_input("Masukkan alas segitiga: ")
tinggi = get_float_input("Masukkan tinggi segitiga: ")

luas = 0.5 * alas * tinggi

print(f"Luas segitiga dengan alas {alas} dan tinggi {tinggi} adalah {luas}")

def hitung_balok(panjang, lebar, tinggi):
    luas_permukaan = 2 * (panjang * lebar + panjang * tinggi + lebar * tinggi)
    volume = panjang * lebar * tinggi
    return luas_permukaan, volume

# Input dari pengguna
panjang = float(input("Masukkan panjang balok: "))
lebar = float(input("Masukkan lebar balok: "))
tinggi = float(input("Masukkan tinggi balok: "))

# Hitung luas dan volume
luas, volume = hitung_balok(panjang, lebar, tinggi)

# Tampilkan hasil
print(f"Luas Permukaan Balok: {luas}")
print(f"Volume Balok: {volume}")

def hitung_kubus(sisi):
    luas_permukaan = 6 * (sisi ** 2)
    volume = sisi ** 3
    return luas_permukaan, volume

# Input dari pengguna
sisi = float(input("Masukkan panjang sisi kubus: "))

# Hitung luas dan volume
luas, volume = hitung_kubus(sisi)

# Tampilkan hasil
print(f"Luas Permukaan Kubus: {luas}")
print(f"Volume Kubus: {volume}")
