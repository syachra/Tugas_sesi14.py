# Meminta input nama barang
nama_barang = input("Masukkan nama barang: ")

# Meminta input harga barang
harga_barang = input("Masukkan harga barang: ")

# Meminta input jumlah barang
jumlah_barang = input("Masukkan jumlah barang: ")

# Menghitung total harga
total_harga = int(harga_barang) * int(jumlah_barang)

# Menampilkan nota
print("Nota Pembayaran")
print("Nama Barang:", nama_barang)
print("Harga Barang: Rp", harga_barang)
print("Jumlah Barang:", jumlah_barang)
print("Total Harga: Rp", total_harga)

# Menyimpan nota ke dalam file
f = open("nota.txt", "w")
f.write("Nota Pembayaran\n")
f.write("Nama Barang: " + nama_barang + "\n")
f.write("Harga Barang: Rp" + harga_barang + "\n")
f.write("Jumlah Barang: " + jumlah_barang + "\n")
f.write("Total Harga: Rp" + str(total_harga) + "\n")
f.close()

print("\nNota telah disimpan dalam file nota.txt")
