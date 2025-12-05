**Expense Tracker Application (C++)**

A simple console-based **Expense Tracker** built using C++.
Program ini memungkinkan pengguna untuk:

* Menambahkan pengeluaran
* Melihat semua pengeluaran
* Mengedit dan menghapus pengeluaran
* Menyimpan data ke file JSON
* Melihat total pengeluaran berdasarkan kategori
* Menggunakan file input/output secara otomatis

Repositori ini juga menyertakan file **input.txt** dan **output.txt** untuk melakukan pengujian seluruh fitur.

---

## ** Project Structure**

```
ProjectExpense-Tracker-Application/
│── SourceCode_CPP              # Main program (C++)
│── input.txt                   # Sample input (for testing)
│── output.txt                  # Program output after running
│── json.hpp                    # JSON library (nlohmann/json)
│── README.md                   # Documentation
```

---

## **📝 Input Data Example (input.txt)**

Berikut contoh format JSON yang digunakan program:

```json
{
  "expenses": [
    {
      "id": 1,
      "date": "2025-01-01",
      "category": "Food",
      "description": "Milk tea",
      "amount": 10000.0,
      "created_at": ""
    },
    {
      "id": 7,
      "date": "2025-01-04",
      "category": "Snacks",
      "description": "Bakso",
      "amount": 13000.0,
      "created_at": ""
    }
  ],
  "next_id": 45,
  "saved_at": "2025-12-05 21:38:35"
}
```

File ini dapat langsung digunakan oleh program untuk memuat data.

---

## **▶️ Cara Menjalankan Program di VS Code (Windows / Mac / Linux)**

### **1. Pastikan Anda memiliki:**

* VS Code
* MinGW / g++ compiler (Windows)
  atau Clang/GCC (Mac/Linux)
* VS Code C/C++ extension (Microsoft)

---

### **2. Clone Repository**

```bash
git clone https://github.com/ChenaniahChen/ProjectExpense-Tracker-Application
cd ProjectExpense-Tracker-Application
```

---

### **3. Buka Folder di VS Code**

```
File → Open Folder → pilih folder project
```

---

### **4. Compile Program**

Di terminal VS Code:

```bash
g++ SourceCode_CPP -o expense_app
```

Jika json.hpp tidak satu folder:

```bash
g++ SourceCode_CPP -I . -o expense_app
```

---

### **5. Jalankan Program**

```bash
./expense_app
```

---

## **📌 Catatan Penggunaan**

* Program akan otomatis membaca data dari file JSON (input.txt).
* Setelah program dijalankan dan fitur digunakan, output akan tersimpan di **output.txt**.
* Anda dapat mengganti isi input.txt untuk mencoba skenario lain.
* Pastikan json.hpp berada dalam satu folder agar compiler dapat mengakses library JSON.

---

## **📦 Dependencies**

* **nlohmann/json.hpp** (sudah tersedia di repo)
* C++11 atau lebih baru

---

## **👥 Author**

**Chenaniah Chen**

Jika butuh bantuan tambahan (seperti penulisan dokumentasi laporan, flowchart, atau perbaikan kode), tinggal bilang saja!
