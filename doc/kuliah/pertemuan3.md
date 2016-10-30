**Resume matakuliah “Sistem Informasi Geografis” Pertemuan 3**

**Shapefile** adalah sebuah formatdata spasial model vector , di dalam shapefile terdapat beberapa file diantaranya **shp** dan **dbf**.

**SHP** adalah salah satu file yang berada didalam shapefile yang menyimpan data geometri.

Didalam file shp terdapat beberapa data seperti :

1.  **Bbox** adalah sebuah boundary box(koordinat 4 titik) atau koordinat batas view pada peta

2.  **Point** adalah titik koordinat

3.  **Shapetype** adalah jenis data geometri yang mempunyai standar nomor yang ditetapkan oleh ESRI seperti nomor 1 untuk poin, 2 untuk polygon, 3 untukpolyline ,dll.

> Membaca jumlah data geometri dengan python :

1.  &gt;&gt; import shapefile

    &gt;&gt; sf = shapefile.Reader(“namafile.shp”)

    &gt;&gt; sf.shapes()

    &gt;&gt;a = sf.shapes()

    &gt;&gt;len(a)

**DBF** adalah sebuah file yang menyimpan file tabular yang menyimpan data atribut.

Membaca data dbf :

1.  &gt;&gt; import shapefile

    &gt;&gt; sf.records()

    &gt;&gt; sf.records(n)
