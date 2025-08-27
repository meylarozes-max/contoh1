# Fungsi untuk menghitung kecepatan
def hitung_kecepatan(jarak, waktu):
    return jarak / waktu

# Data kendaraan
mobil_A_jarak = 2000  # dalam meter
mobil_A_waktu = 90    # dalam detik

motor_B_jarak = 1500  # dalam meter
motor_B_waktu = 50     # dalam detik

sepeda_C_jarak = 800   # dalam meter
sepeda_C_waktu = 40     # dalam detik

# Menghitung kecepatan masing-masing kendaraan
kecepatan_mobil_A = hitung_kecepatan(mobil_A_jarak, mobil_A_waktu)
kecepatan_motor_B = hitung_kecepatan(motor_B_jarak, motor_B_waktu)
kecepatan_sepeda_C = hitung_kecepatan(sepeda_C_jarak, sepeda_C_waktu)

# Menampilkan hasil kecepatan
print(f"Kecepatan Mobil A: {kecepatan_mobil_A:.2f} m/s")
print(f"Kecepatan Motor B: {kecepatan_motor_B:.2f} m/s")
print(f"Kecepatan Sepeda C: {kecepatan_sepeda_C:.2f} m/s")

# Menentukan kendaraan dengan kecepatan tertinggi
kecepatan_tertinggi = max(kecepatan_mobil_A, kecepatan_motor_B, kecepatan_sepeda_C)

if kecepatan_tertinggi == kecepatan_mobil_A:
    kendaraan_tercepat = "Mobil A"
elif kecepatan_tertinggi == kecepatan_motor_B:
    kendaraan_tercepat = "Motor B"
else:
    kendaraan_tercepat = "Sepeda C"

print(f"Kendaraan dengan kecepatan tertinggi adalah: {kendaraan_tercepat} dengan kecepatan {kecepatan_tertinggi:.2f} m/s")
