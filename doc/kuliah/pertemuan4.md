**Resume matakuliah “Sistem Informasi Geografis” Pertemuan 4**

**Poin** dalam peta biasanya menunjukan sebuah tempat misalnya restoran

**Polygon** dalam peta biasanya menunjukan sebuah pulau

Perbedaan **Polygon** dan **Polyline** adalah titik awal dan akhir polygon selalu bertemu sedangkan tidak dengan polyline

**Implementasi Retrieve Data Geospasial dalam python :**

&gt;&gt;sf = shapefile.Reader(‘namafile.shp’)

**sf** adalah variable

**shapefile** adalah nama class

**Reader** adalah nama method

**Perintah untuk mengambil data perkolom :**

&gt;&gt;sf.record(n)\[n\]

**Perintah untuk melihat isi shapefile :**

&gt;&gt;a = sf.shape(0)

&gt;&gt;dir(a)

**Untuk melihat type :**

&gt;&gt; a.shapetype

**Mencari negara :**

&gt;&gt; for a in sf.records():

&gt;&gt; if a\[8\] == “indonesia”

&gt;&gt; print a

**Melihat Baris :**

&gt;&gt; Print i

&gt;&gt; i = i + 1
