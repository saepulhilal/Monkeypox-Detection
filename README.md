# Monkeypox Detection

---

## Tujuan

Program ini dibuat untuk mendeteksi penyakit monkeypox. Input pada program ini berupa gambar, gambar tersebut akan di prediksi dengan deep learning untuk mengetahui hasil dari gambar tersebut adalah terkena monkeypox atau bukan.

---

## Kesimpualan
1. **Jumlah Data:** Terdapat total 2142 data train dan 420 data validasi untuk pelatihan model.

2. **Arsitektur Model:**
   - Menggunakan model Sequential dengan base EfficientNetV2B0.
   - Total parameter model sebanyak 38,109,553, dengan 32,190,241 parameter yang dapat di-train.
   - Dilakukan beberapa lapisan Dense dengan dropout untuk menghindari overfitting.

3. **Pelatihan Model:**
   - Model dilatih selama 30 epoch.
   - Hasil dari Training pada data validasi mendapatkan akurasi sebesar 0.6905 dan untuk loss sebesar 0.6921

4. **Hasil Evaluasi:**
   - Setelah pelatihan, model berhasil mencapai akurasi validasi sebesar 80%.
   - Hasil evaluasi pada data uji menunjukkan bahwa model memiliki performa baik dalam mendeteksi Monkeypox (precision 58%, recall 90%) namun kurang baik dalam mendeteksi kategori lain (precision 86%, recall 48%).
   - Akurasi keseluruhan pada data uji adalah 67%, dengan nilai f1-score sebesar 0.66.

Model berhasil mencapai akurasi yang baik pada data validasi, terutama dalam mengenali Monkeypox. Namun, masih diperlukan perbaikan khususnya dalam meningkatkan recall untuk kategori lainnya agar hasil evaluasi lebih seimbang. Rekomendasi penggunaan format penyimpanan model yang lebih baru juga perlu dipertimbangkan.

---

Untuk hasil deployment dapa dilihat pada [HuggingFace](https://huggingface.co/spaces/saepulhilal/gc7)
