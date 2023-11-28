# AndroidStudio_Versi2

Nama            : Dhea Dwi Adelia

NIM             : 312210116

Kelas           : TI.22.A.1

Mata Kuliah     : Pemrograman Mobile 1

Dosen Pengampu  : Donny Maulana, S.Kom., M.M.S.I

# Perintah Tugas

![image](https://github.com/adeliadhea06/AndroidStudio_Versi2/assets/115794875/5db59965-fe4c-4c9b-8734-ce44e638e5af)


# Langkah - Langkah

1. Kita membuat sebuah drawable resource file nya terlebih dahulu. Disini kita akan memberi nama filenya itu adalah backgroundicon.xml, dengan root elementnya adalah shape.

2. Kemudian didalam backgroundicon.xml itu kita tambahkan code berikut.

        <?xml version="1.0" encoding="utf-8"?>
        <shape xmlns:android="http://schemas.android.com/apk/res/android">
          <solid android:color="@color/colorPrimaryDark"/>
          <corners android:radius="80dp"/>
          <size android:width="80dp" android:height="80dp"/>
        </shape>

   * Untuk warna dan ukuran dapat disesuaikan dengan keinginan masing-masing.

3. Untuk iconnya kita bisa menggunakan icon yang sudah kita punya atau kalau ingin lebih mudah kita dapat menggunakan icon yang sudah disediakan di android studionya. Caranya adalah dengan menambah vector asset pada drawable file.

   * Sesuaikan nama, ukuran, dan warna dengan kebutuhannya masing-masing.
  
4. Jika semua hal diatas sudah selesai, kemudian kita lanjut untuk mengedit activity_main.xml untuk mengganti tombol yang awalnya button menjadi image button. Bertujuan untuk merubah dari tombol teks menjadi icon.

5. Selanjutnya, kita diharuskan untuk menghapus terlebih dahulu semua button kecuali imageview untuk background, tetapi lebih baik salin code button sebelumnya dikarenakan nanti kita akan pakai lagi. Langsung saja masuk ke tahap pengeditan

   a. Pertama kita tambahkan linear layoutnya terlebih dulu dengan orientasi vertical untuk dasar dari penempatan tombol.

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical"
                    android:gravity="center_horizontal">
                
                </LinearLayout>

   b. Selanjutnya yang kedua, didalam LinearLayout vertical nya. Kita tambahkan lagi LinearLayout, tetapi dengan orientasi horizontal agar tombol berjajar kesamping.

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical"
                    android:gravity="center_horizontal">
                
                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:orientation="horizontal"
                        android:gravity="center">
                
                    </LinearLayout>
                </LinearLayout>

   c. Kemudian yang ketiga, kita tambahkan terlebih hanya sebanyak tiga button. Supaya buttonnya sesuai dengan apa yang diperintahkan yaitu tiga buah berjajar kesamping.

              <LinearLayout
                  android:layout_width="match_parent"
                  android:layout_height="match_parent"
                  android:orientation="vertical"
                  android:gravity="center_horizontal">
              
                  <LinearLayout
                      android:layout_width="match_parent"
                      android:layout_height="wrap_content"
                      android:orientation="horizontal"
                      android:gravity="center">
              
                      <ImageButton
                          android:id="@+id/btnHelloWorld"
                          android:layout_width="wrap_content"
                          android:layout_height="wrap_content"
                          android:layout_margin="20dp"
                          android:background="@drawable/backgroundicon"
                          android:onClick="btnHelloWorld"
                          android:src="@drawable/icon_helloword"
                          tools:ignore="UsingOnClickInXml,SpeakableTextPresentCheck" />
              
                      <ImageButton
                          android:id="@+id/btnProjectCount"
                          android:layout_width="wrap_content"
                          android:layout_height="wrap_content"
                          android:layout_margin="20dp"
                          android:background="@drawable/backgroundicon"
                          android:onClick="btnCount"
                          android:src="@drawable/icon_count1"
                          tools:ignore="UsingOnClickInXml,SpeakableTextPresentCheck" />
              
                      <ImageButton
                          android:id="@+id/btnProjectSianida"
                          android:layout_width="wrap_content"
                          android:layout_height="wrap_content"
                          android:layout_margin="20dp"
                          android:background="@drawable/backgroundicon"
                          android:onClick="btnSianida"
                          android:src="@drawable/icon_sianida1"
                          tools:ignore="UsingOnClickInXml,SpeakableTextPresentCheck" />
              
                  </LinearLayout>
              </LinearLayout>

     * Tujuan dari salin code tadi ada disini. Jadi kita tidak serta merta menghapus code lalu membuat ulang, tetapi hanya mengeditnya menjadi ImageButton. Masukkan juga background dan icon yang sudah kita buat dan tambahkan sebelumnya pada setiap buttonnya.

   d. Selanjutnya yang terakhir, kita akan menambahkan lagi sebuah LinearLayout Horizontal untuk tombol yang tersisa.

                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical"
                    android:gravity="center_horizontal">
                
                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:orientation="horizontal"
                        android:gravity="center">
                
                        <ImageButton
                            android:id="@+id/btnHelloWorld"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_margin="20dp"
                            android:background="@drawable/backgroundicon"
                            android:onClick="btnHelloWorld"
                            android:src="@drawable/icon_helloword"
                            tools:ignore="UsingOnClickInXml,SpeakableTextPresentCheck" />
                
                        <ImageButton
                            android:id="@+id/btnProjectCount"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_margin="20dp"
                            android:background="@drawable/backgroundicon"
                            android:onClick="btnCount"
                            android:src="@drawable/icon_count1"
                            tools:ignore="UsingOnClickInXml,SpeakableTextPresentCheck" />
                
                        <ImageButton
                            android:id="@+id/btnProjectSianida"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_margin="20dp"
                            android:background="@drawable/backgroundicon"
                            android:onClick="btnSianida"
                            android:src="@drawable/icon_sianida1"
                            tools:ignore="UsingOnClickInXml,SpeakableTextPresentCheck" />
                    </LinearLayout>
                
                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:orientation="horizontal"
                        android:gravity="center">
                
                        <ImageButton
                            android:id="@+id/btnTwoActivity"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_margin="20dp"
                            android:background="@drawable/backgroundicon"
                            android:onClick="btnTwoActivity"
                            android:src="@drawable/icon_twoact1"
                            tools:ignore="UsingOnClickInXml, SpeakableTextPresentCheck" />
                
                        <ImageButton
                            android:id="@+id/btnSetAlarm"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_margin="20dp"
                            android:background="@drawable/backgroundicon"
                            android:onClick="btnSetAlarm"
                            android:src="@drawable/icon_alarm1"
                            tools:ignore="UsingOnClickInXml,SpeakableTextPresentCheck" />
                
                        <ImageButton
                            android:id="@+id/btnshowMap"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_margin="20dp"
                            android:background="@drawable/backgroundicon"
                            android:onClick="btnshowMap"
                            android:src="@drawable/icon_maps1"
                            tools:ignore="UsingOnClickInXml,SpeakableTextPresentCheck" />
                    </LinearLayout>
                </LinearLayout>
   
         * kita menambahkan sebuah button baru yaitu button untuk membuka maps.

   e. Selanjutnya kita akan mendapatkan tampilan design seperti ini.
   
![Screenshot_2023-11-28_082903 1](https://github.com/adeliadhea06/AndroidStudio_Versi2/assets/115794875/31e728f3-32d6-4b8d-9a57-1a77ff6cdd39)


7. Tampilan design activity_main.xml sudah selesai.

8. Selanjutnya kita mengedit pada bagian MainActivity.java, karena kemaren diperintahkannya untuk membuat tombol membuka maps. Maka disini kita akan tambahkan lagi code implicit intent untuk membuka mapsnya, tambahkan code berikut dibawah setContentView

        ImageButton btnshowMap = findViewById(R.id.btnshowMap);
              btnshowMap.setOnClickListener(v -> {
                  Intent map = new Intent(Intent.ACTION_VIEW, Uri.parse("geo:-6.324307,107.169273"));
                  map.setPackage("com.google.android.apps.maps");
                  startActivity(map);
              });

9. Semua code sudah berhasil ditambahkan dan diedit.

# Hasil Run

https://github.com/adeliadhea06/AndroidStudio_Versi2/assets/115794875/937b272a-c827-46f5-b30c-174ef8530536


# Sekian dan Terima Kasih
