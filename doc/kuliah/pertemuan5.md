**Resume matakuliah “Sistem Informasi Geografis” Pertemuan 5**

**Membuat Data Geospasial**

1.  &gt;&gt; Import Shapefile

2.  &gt;&gt; a = shapefile.Writer(*param*)

> Param dalam writer ini menunjukan shapetype apa yang akan kita buat contohnya **polygon, polyline,** dan **point**.

1.  &gt;&gt; a.point(x,y)

    Atau,

    &gt;&gt; a.poly(\[x,y\],\[v,w\])

    Perintah ini digunakan jika akan membuat file shp.

2.  &gt;&gt; a.field(‘nama’,’typedata’,’90’)

    Perintah ini digunakan jika akan membuat file dbf.

&gt;&gt; a.record(‘isi’)

Perintah ini digunakan untuk mengisi file dbf.

1.  &gt;&gt; a.shp(‘namafile.shp’)

    &gt;&gt; save(‘namafile’)

> Perintah untuk menyimpan file.

**Contoh Pembuatan field dalam dbf**

&gt;&gt; field(‘kota’,’c’,’40’)

Peritah ini berarti kita membuat sebuah atribut table bernama **kota** dengan tipedata **varchar** dengan panjang **40** karakter, kemudian jika ingin menambahkan data maka dapat dilakukan dengan perintah :

&gt;&gt; Record(‘Bandung’)
