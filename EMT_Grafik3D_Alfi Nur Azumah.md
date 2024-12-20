# Menggambar Plot 3D dengan EMT

Ini adalah pengenalan plot 3D di Euler. Kita membutuhkan plot 3D untuk
memvisualisasikan fungsi dari dua variabel.


Euler menggambar fungsi tersebut menggunakan algoritma pengurutan
untuk menyembunyikan bagian di latar belakang. Secara umum, Euler
menggunakan proyeksi pusat. Standarnya adalah dari kuadran x-y positif
menuju titik asal x=y=z=0, tetapi sudut=0° terlihat dari arah sumbu y.
Sudut pandang dan tinggi dapat diubah.


Euler dapat merencanakan

- permukaan dengan bayangan dan garis level atau rentang level,
- awan poin,
- kurva parametrik,
- permukaan implisit.


Plot 3D dari suatu fungsi menggunakan plot3d. Cara termudah adalah
dengan memplot ekspresi dalam x dan y. Parameter r mengatur kisaran
plot di sekitar (0,0).


\>aspect(1.5); plot3d("x^2+sin(y)",r=pi): 


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-001.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-001.png)

### 4.1 Menggambar Grafik Fungsi Dua Variabel dalam Bentuk

**Ekspresi Langsung**

Grafik fungsi dua variabel dalam bentuk ekspresi langsung adalah
representasi visual dari hubungan matematis antara dua variabel
independen yang dinyatakan dalam bentuk persamaan atau ekspresi
matematis. Biasanya, grafik ini digunakan untuk menggambarkan hubungan
antara dua variabel dalam bidang dua dimensi dan tiga dimensi. Dalam
konteks ini, variabel independen (x dan y) adalah variabel input,
sedangkan variabel dependen (z) adalah variabel output yang dihasilkan
oleh ekspresi matematis.


Rumus umum untuk menggambar grafik fungsi dua variabel dalam bentuk
ekspresi langsung adalah:


$$z = f(x, y)$$Dalam rumus ini:


- z adalah variabel dependen yang ingin kita gambar dalam grafik.

- f(x, y) adalah ekspresi matematis yang menghubungkan variabel z dengan variabel independen x dan y. Ekspresi ini dapat berupa fungsi linear, fungsi kuadrat, fungsi akar kuadrat, eksponensial, logaritma, trigonometri, nilai mutlak, atau jenis fungsi matematis lainnya, tergantung pada hubungan yang ingin diilustrasikan.

**1. Grafik Fungsi Linear**


Fungsi linear dua variabel biasanya dinyatakan dalam bentuk

$$f(x,y)=ax+by+c$$

dimana a,b, dan c adalah konstanta.  Grafik fungsi linear ini adalah
sebuah bidang datar, dan bentuknya akan bervariasi tergantung pada
nilai a dan b.


Contoh:


$$f(x,y)=2x+3y+5$$\>plot3d("2\*x+3\*y+5"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-005.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-005.png)

$$f(x,y)=-2x-3y-5$$\>plot3d("-2\*x-3\*y-5"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-007.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-007.png)

$$f(x,y)=5x-7y+9$$\>plot3d("5\*x-7\*y+9"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-009.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-009.png)

**2. Grafik Fungsi Kuadrat**



Fungsi kuadrat dua variabel biasanya dinyatakan dalam bentuk


$$f(x,y)=ax^2+by^2+cxy+dx+ey+f$$

dimana a, b, c, d, e, dan f adalah konstanta. Grafik fungsi kuadrat
ini adalah sebuah permukaan yang dapat memiliki berbagai bentuk
tergantung pada nilai-nilai konstantanya.


Contoh:


$$f(x,y)= x^2+y^2+4xy+8x+3y+1$$\>plot3d("x^2+y^2+4\*x\*y+8\*x+3\*y+1"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-012.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-012.png)

$$f(x,y)= 3x^2-y^2+7xy-5$$\>plot3d("3\*x^2-y^2+7\*x\*y-5"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-014.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-014.png)

**3. Grafik Fungsi Akar Kuadrat**



Grafik fungsi akar kuadrat dua variabel


$$f(x,y)=\sqrt{x^2+y^2}$$

adalah grafik permukaan yang menggambarkan jarak titik (x, y) dari
titik asal (0, 0) dalam ruang tiga dimensi.


Contoh:


$$f(x,y)=\sqrt{x^2+y^2}$$\>plot3d("sqrt(x^2+y^2)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-017.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-017.png)

$$f(x,y)=\sqrt{2x^2+7y^2}$$\>plot3d("sqrt(2\*x^2+7\*y^2)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-019.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-019.png)

$$f(x,y)=\sqrt{10x^2+y^2}$$\>plot3d("sqrt(10\*x^2+y^2)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-021.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-021.png)

**4. Grafik Fungsi Eksponensial**



Fungsi eksponensial dua variabel bisa dinyatakan


$$f(x,y)=a.b^{xy}$$

dimana a dan b adalah konstanta, x dan y adalah variabel. Fungsi ini
menggambarkan pertumbuhan eksponensial yang bergantung pada nilai x
dan y.


Contoh:


$$f(x,y)= 2.3^{xy}$$\>plot3d("2\*3^(x\*y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-024.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-024.png)

$$f(x,y)= -3.8^{xy}$$\>plot3d("-3\*8^(x\*y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-026.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-026.png)

**5. Grafik Fungsi Logaritma**



Grafik fungsi logaritma dua variabel adalah grafik yang menggambarkan
nilai logaritma dari suatu ekspresi yang melibatkan dua variabel
(biasanya x dan y). Fungsi logaritma dua variabel ini dinyatakan
sebagai


$$f(x,y)=log_b(xy)$$

dimana b adalah basis logaritma. Basis logaritma ini dapat
berbeda-beda.


Contoh:


$$f(x,y)=log(xy), basis 10$$\>plot3d("log(x\*y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-029.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-029.png)

$$f(x,y)=log(2x.9y), basis 10$$\>plot3d("log(2x\*9y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-031.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-031.png)

**6. Grafik Fungsi Trigonometri**

Fungsi trigonometri dua variabel adalah fungsi matematika yang
melibatkan operasi trigonometri (seperti sin, cos, tan) pada kedua
variabel x dan y.


Contoh:


$$f(x,y)=sin(x).cos(y)$$\>plot3d("sin(x)\*cos(y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-033.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-033.png)

$$f(x,y)=sin(2x).cos(y)$$\>plot3d("sin(2x)\*cos(y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-035.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-035.png)

$$f(x,y)=sin(x).tan(y)$$\>plot3d("sin(x)\*tan(y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-037.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-037.png)

$$f(x,y)=cos(x).tan(y)$$\>plot3d("cos(x)\*tan(y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-039.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-039.png)

$$f(x,y)=cosec(x).sec(y)$$\>plot3d("cosec(x)\*sec(y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-041.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-041.png)

$$f(x,y)=cot(x).cosec(y)$$\>plot3d("cot(x)\*cosec(y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-043.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-043.png)

**7. Grafik Fungsi Nilai Mutlak**

Fungsi nilai mutlak dua variabel, juga dikenal sebagai fungsi modul
dua variabel, dinyatakan sebagai


$$f(x,y)=|g(x,y)|$$

dimana g(x,y) adalah fungsi dua variabel.


Contoh:


$$f(x,y)=|x^2 - y^2|$$\>plot3d("abs(x^2 - y^2)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-046.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-046.png)

$$f(x,y)=|x^2 + y^2|$$\>plot3d("abs(x^2 + y^2)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-048.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-048.png)

$$f(x,y)=|-2x^2 - 5y^2|$$\>plot3d("abs(-2x^2 - 5y^2)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-050.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-050.png)

$$f(x,y)=|x^2 - 8y^2|$$\>plot3d("abs(x^2 - 8y^2)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-052.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-052.png)

**Latihan soal**

Buatkan grafik dari fungsi berikut:


1. $$f(x,y)=8x-3y+7$$\>plot3d("8\*x - 3\*y +7"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-054.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-054.png)

2. $$f(x,y)=cos(5x).sin(9y)$$\>plot3d("cos(5\*x)\*sin(9\*y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-056.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-056.png)

3. $$f(x,y)=\sqrt{x^2+20y^2}$$\>plot3d("sqrt(x^2+20\*y^2)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-058.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-058.png)

### 4.2 Menggambar Grafik Fungsi Dua Variabel yang Rumusnya Disimpan dalam Variabel Ekspresi

**Apa yang dimaksud dengan Grafik Fungsi Dua Variabel?**

Grafik fungsi dua variabel adalah representasi visual dari hubungan
antara sebuah fungsi matematika dengan dua variabel independen
(biasanya disebut sebagai "x" dan "y") dan variabel dependen (biasanya
disebut sebagai "z" atau "f(x, y)").


Dalam grafik ini, sumbu x dan sumbu y digunakan untuk menggambarkan
nilai-nilai dua variabel independen, sementara permukaan atau grafik
3D digunakan untuk menggambarkan nilai-nilai variabel dependen yang
dihasilkan oleh fungsi tersebut.


Grafik fungsi dua variabel membantu memvisualisasikan bagaimana nilai
variabel dependen (z) berubah seiring perubahan kedua variabel
independen (x dan y) sesuai dengan aturan fungsi tersebut.


**Fungsi matematika yg terlibat dalam Menggambar Grafik**

**A. Fungsi Dua Variabel**

1. Fungsi Linear

Bentuk umum

f(x, y) = ax + by + c, di mana a, b, dan c adalah konstanta. Grafiknya
adalah bidang datar.

2. Fungsi Kuadratik

Bentuk umum f(x, y) = ax^2 + by^2 + cxy + dx + ey + f.

Grafiknya dapat berupa permukaan yang berbentuk paraboloid, baik
terbuka ke atas atau ke bawah.

3. Fungsi Trigonometri

Bentuk umum sinus dan cosinus

(x, y) = sin(x) + cos(y)

akan menghasilkan permukaan yang berulang-ulang naik dan turun.

4. Fungsi Pecahan

Bentuk umum f(x, y) = g(x, y) / h(x, y), di mana g(x, y) dan h(x, y)
adalah fungsi-fungsi lain.

grafiknya dapat menghasilkan berbagai pola yang tergantung pada sifat
fungsi g dan h.


**Menggambar Grafik Fungsi**

Perintah yang digunakan untuk menggambar grafik fungsi dalam EMT yaitu
dengan menggunakan plot3d.


Untuk menampilkan grafik, akhiri perintah plot3d dengan tanda (:).


Tanda (:) akan menampilkan grafik di layar yang berbeda.


\>plot3d("x^2+y^2"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-059.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-059.png)

\>plot3d("x^3+x\*sin(y)",-5,5,0,6\*pi):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-060.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-060.png)

**Menyimpan Variabel Ekspresi**

Untuk menyimpan sebuah fungsi, dapat dilakukan dengan menggunakan
perintah function. Lalu, ketika ingin memanggil atau membuat grafik
dari fungsi tersebut, cukup dengan memanggil nama fungsi tersebut.


\>function a(x,y):= x^2+y^3

\>plot3d("a"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-061.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-061.png)

\>function f(x,y):= x^3-y^2

\>plot3d("f"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-062.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-062.png)

**Contoh Latihan Soal**

$$f(x,y)= x^3+y^4$$\>function f(x,y):= x^3+y^4

\>plot3d("f"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-064.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-064.png)

\>plot3d("a",\>user, ...  
\>   title="Turn with the vector keys (press return to finish)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-065.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-065.png)

Perintah ini mengizinkan pengguna untuk menggambar grafik 3D dari
fungsi yang mereka masukkan sendiri, serta memberikan petunjuk
interaktif tentang cara berinteraksi dengan grafik. Pengguna dapat
memutar tampilan grafik menggunakan tombol arah pada keyboard, dan
menekan "return" untuk menyelesaikan interaksi.


\>plot3d("a",r=5,n=80,fscale=4,scale=1.2,frame=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-066.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-066.png)

perintah ini akan menggambar grafik tiga dimensi dari fungsi "a" dalam
rentang x dan y dari -5 hingga 5, dengan 80 titik untuk detail yang
lebih halus. Nilai fungsi akan diperbesar 4 kali, dan grafik akan
ditampilkan dengan skala 1.2 untuk tampilan yang lebih jelas. Bingkai
grafis akan ditentukan oleh parameter frame=3.


\>view


    [5,  2.6,  2,  0.4]

\>plot3d("a",distance=3,zoom=2,angle=0,height=0):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-067.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-067.png)

\>plot3d("x^4+y^2",a=0,b=1,c=-1,d=1,angle=-20°,height=20°, ...  
\>   center=[0.4,0,0],zoom=5):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-068.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-068.png)

\>plot3d("a",r=2,<fscale,<scale,distance=13,height=50°, ...  
\>    center=[0,0,-2],frame=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-069.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-069.png)

\>plot3d("a",r=5,\>polar, ...  
\>   fscale=2,\>hue,n=100,zoom=4,\>contour,color=blue):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-070.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-070.png)

\>plot3d("x","a","y",r=2,zoom=3.5,frame=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-071.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-071.png)

**B. Fungsi Linear**

\>function e(x,y):= 20x+10y-5

\>plot3d("e"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-072.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-072.png)

\>plot3d("e",\>user, ...  
\>   title="Turn with the vector keys (press return to finish)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-073.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-073.png)

\>plot3d("e",r=10,n=80,fscale=4,scale=1.2,frame=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-074.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-074.png)

\>view


    [5,  2.6,  2,  0.4]

\>plot3d("e",distance=3,zoom=2,angle=0,height=0):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-075.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-075.png)

\>plot3d("e",a=0,b=1,c=-1,d=1,angle=-20°,height=20°, ...  
\>   center=[0.4,0,0],zoom=5):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-076.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-076.png)

\>plot3d("e",r=2,<fscale,<scale,distance=13,height=50°, ...  
\>   center=[0,0,-2],frame=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-077.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-077.png)

\>plot3d("e",r=5,\>polar, ...  
\>   fscale=2,\>hue,n=100,zoom=4,\>contour,color=gray):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-078.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-078.png)

\>plot3d("x","e","y",r=2,zoom=3.5,frame=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-079.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-079.png)

**C. Fungsi Trigonometri**


\>function f(x,y):= sin(x+y)

\>plot3d("f")

\>plot3d("f",\>user, ...  
\>   title="Turn with the vector keys (press return to finish)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-080.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-080.png)

\>plot3d("f",r=10,n=80,fscale=4,scale=1.2,frame=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-081.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-081.png)

\>view


    [5,  2.6,  2,  0.4]

\>plot3d("f",distance=3,zoom=2,angle=0,height=0):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-082.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-082.png)

\>plot3d("f",a=0,b=1,c=-1,d=1,angle=-20°,height=20°, ...  
\>   center=[0.4,0,0],zoom=5):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-083.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-083.png)

\>plot3d("f",r=5,\>polar, ...  
\>   fscale=2,\>hue,n=100,zoom=4,\>contour,color=gray):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-084.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-084.png)

### 4.3 Menggambar Grafik Fungsi Dua Variabel yang Fungsinya

**Didefinisikan sebagai Fungsi Numerik**

Sebelum masuk ke cara memvisualisasikan grafik, perlu diketahui apa
itu fungsi dua variabel dan apa itu fungsi numerik.


1. Fungsi Dua Variabel

Fungsi dua variabel adalah jenis fungsi di mana ada dua variabel bebas
(biasanya dinotasikan sebagai x dan y) yang menentukan nilai dari
fungsi tersebut. Dengan kata lain, untuk setiap kombinasi nilai dari x
dan y, fungsi ini akan menghasilkan satu nilai output tertentu. Fungsi
dari dua variabel yang mana setiap kombinasi nilai dari kedua variabel
tersebut menghasilkan sebuah nilai tunggal.

2. Fungsi Numerik

Fungsi dimana setiap pasangan variabel independen adalah angka atau
bilangan nyata. Secara sederhana, ketika memasukkan angka atau
bilangan nyata ke variabel-variabel dalam fungsi maka hasil akhir yang
dihasilkan juga angka atau bilangan nyata, bukan simbol atau ekspresi
yang belum dihitung.


Contoh:

ada fungsi


$$f(x,y)=2x+y$$Ketika kita memasukkan bilangan nyata ke x dan y maka akan dihasilkan
suatu bilangan nyata juga. Misal masukkan x=1 dan y=1. Akan diperoleh


$$2(1)+1=3$$
**Visualisasi Grafik**

Untuk memvisualisaikan fungsi dua variabel dengan fungsinya
didefinisikan sebagai fungsi numerik, akan dibuat grafik 3D dengan
sintaks plot3d. Untuk membedakan fungsi numerik dengan simbolik, pada
kali ini untuk setiap fungsi numerik dua variabel hanya akan memuat
variabel x dan y. Namun, dalam pemakaian secara umum, bisa digunakan
variabel apapun.


Penulisan Sintaks:


1) definisikan fungsi numerik


function f(x,y):= ax+by dengan a dan b adalah suatu konstanta dan
fungsi tidak selalu direpresentastikan dengan f tetapi bisa dengan
huruf apapun. Contoh : g(x,y)


2) sintaks plot3d


plot3d("f"):


Contoh Visualisasi Grafik:


1. Visualisasi grafik fungsi linear dua variabel


$$f(x,y) = 3x+7y$$\>function f(x,y):= 2\*x+5\*y

\>plot3d("f"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-088.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-088.png)

2. Visualisasi grafik fungsi kuadrat dua variabel


$$f(x,y)=x^2+2xy+y^2$$\>function f(x,y):= x^2+2\*x\*y+y^2 

\>plot3d("f"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-090.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-090.png)

3. Visualisasi Grafik Fungsi Eksponen Dua Variabel


$$g(x,y) = x^{2y+8}$$\>function g(x,y):= x^(2y+8)

\>plot3d("g"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-092.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-092.png)

4. Grafik Fungsi Logaritma Dua Variabel


$$f(x,y)=\log(xy)$$\>function f(x,y):= log(x\*y)

\>plot3d("f"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-094.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-094.png)

5. Grafik Fungsi Trigonometri Dua Variabel


$$h(x,y)=sin(xy)cos(y)$$\>function h(x,y):= sin(x\*y)\*cos(y)

\>plot3d("h"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-096.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-096.png)

6. Grafik Fungsi Nilai Mutlak Dua Variabel


$$i(x,y)=|(2x+y)|$$\>function i(x,y):= abs(2x+y)

\>plot3d("i"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-098.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-098.png)

**Latihan Soal**

Buatlah visualisasi grafik dari fungsi berikut ini!


1.


$$f(x,y)=2^x+3y$$\>function f(x,y):=2^x+3\*y

\>plot3d ("f"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-100.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-100.png)

2.


$$g(x,y)=sin(x^2y+1)$$\>function g(x,y):= sin(x^2\*y+1)

\>plot3d("g"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-102.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-102.png)

3. 


$$h(x,y)=|4x+sin(y^3+1)|$$\>function h(x,y):=abs(4\*x + sin(y^3+1))

\>plot3d("h"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-104.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-104.png)

### 4.4 Menggambar Grafik Fungsi Dua Variabel yang Fungsinya

**Didefinisikan sebagai Fungsi Simbolik**

Grafik Fungsi dua variabel yang fungsinya didefinisikan sebagai fungsi
simbolik adalah suatu grafik yang memvisualisasikan Persamaan Linear
Dua Variabel (PLDV) dalam koordinat kartesius dengan fungsinya
merupakan fungsi simbolik.


Proses visualisasi ini memungkinkan Kita untuk melihat dan memahami
bagaimana fungsi tersebut berperilaku dalam tiga dimensi.


Sedangkan yang dimaksud dengan fungsi simbolik yaitu fungsi yang
didefinisikan dalam bentuk matematika simbolik, artinya kita memiliki
ekspresi matematika yang menggambarkan hubungan antara dua variabel.
misalnya, jika kita memiliki fungsi


$$f(x, y) = x^2 + y^2$$

kita dapat menggambar grafiknya untuk melihat bentuk permukaan yang
dihasilkan oleh fungsi ini dalam tiga dimensi. Grafik ini mungkin akan
berupa tumpukan parabola yang membentuk kerucut.


Karakteristik fungsi simbolik adalah dengan mengganti tanda := menjadi
&amp;=


Perbedaan utama antara fungsi numerik dan fungsi simbolik adalah bahwa
fungsi numerik memberikan hasil numerik secara langsung (menghasilkan
angka), sementara fungsi simbolik memungkinkan kita untuk bekerja
dengan simbol matematika sebelum menghitung nilai numeriknya. Pilihan
antara keduanya tergantung pada kebutuhan analisis matematika yang
kita lakukan.


Tujuan menggambar grafik fungsi dua variabel adalah untuk memahami
pola, sifat, dan hubungan antara dua variabel tersebut secara visual,
yang dapat membantu dalam analisis dan pemahaman masalah matematika
atau ilmu pengetahuan yang melibatkan fungsi ini.


**Langkah-langkah Membuat Grafik**

1) Definisikan fungsinya terlebih dahulu. Tentukan fungsi dua variabel
yang akan divisualisasikan dalam bentuk simbolik.


Misal diambil fungsi


$$f(x,y)=x^2+y^2$$

Maka perintah yang dapat dituliskan yaitu:


\>function f(x,y)&= x^2+y^2;


2) Panggil fungsinya


\>plot3d("f(x,y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-107.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-107.png)

3) Tentukan rentang variabelnya


\>plot3d("f(x,y)",-5,5,0,6\*pi):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-108.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-108.png)

**Membuat Grafik Fungsi Linear**

$$g(x,y)=x+3y$$\>function g(x,y) &= x+3\*y;

\>plot3d("g(x,y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-110.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-110.png)

$$M(x,y)=-2x-4y$$\>function M(x,y) &= -2\*x-4\*y;

\>plot3d("M(x,y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-112.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-112.png)

Rentang variabel:


\>plot3d("M(x,y)",-2,2,0,6\*pi):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-113.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-113.png)

**Membuat Grafik Fungsi Kuadrat**

$$Q(x,y)=x^2-y^2$$\>function Q(x,y) &= x^2 - y^2;

\>plot3d("Q(x,y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-115.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-115.png)

$$P(x,y)=3x^2-4xy+2y^2$$\>function P(x,y) &= 3\*x^2-4\*x\*y+2\*y^2;

\>plot3d("P(x,y)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-117.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-117.png)

Rentang variabel:


\>plot3d("P(x,y)",-10,10,0,9\*pi):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-118.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-118.png)

**Membuat Grafik Fungsi Akar Kuadrat**

$$A(x,y)= \sqrt{10x^2+2y^2}$$\>function A(x,y) &= sqrt(10\*x^2+2\*y^2);

\>plot3d("A"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-120.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-120.png)

$$W(x,y)= \sqrt{x^2+2y^2}$$\>function W(x,y) &= sqrt(x^2+2\*y^2);

\>plot3d("W"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-122.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-122.png)

Rentang Variabel:


\>plot3d("W(x,y)",-20,100,0,5\*pi):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-123.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-123.png)

**Membuat Grafik Fungsi Eksponensial**

$$F(x,y)= 9.12^{xy}$$\>function F(x,y) &= 9\*12^(x\*y);

\>plot3d("F"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-125.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-125.png)

$$H(x,y)=5.(-20)^{xy}$$\>function H(x,y) &= 5\*-12^(x\*y);

\>plot3d("H"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-127.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-127.png)

$$T(x,y)=(-21).5^{xy}$$\>function T(x,y) &= -21\*-5^(x\*y);

\>plot3d("T"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-129.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-129.png)

**Membuat Grafik Fungsi Logaritma**

$$B(x,y)=log(x.2y), Basis 10$$\>function B(x,y) &= log(x\*2\*y);

\>plot3d("B"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-131.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-131.png)

$$C(x,y)=log(30x.5y), basis 10$$\>function C(x,y) &= log(30\*x\*5\*y);

\>plot3d("C"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-133.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-133.png)

**Membuat Grafik Fungsi Trigonometri**

$$D(x,y)=sin(2x).cos(3y)$$\>function D(x,y) &= sin(2\*x)\*cos(3\*y);

\>plot3d("D"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-135.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-135.png)

$$J(x,y)=sin(2x).tan(y)$$\>function J(x,y) &= sin(2\*x)\*tan(y);

\>plot3d("J"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-137.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-137.png)

$$G(x,y)=sec(2x).cot(5y)$$\>function G(x,y) &= sec(2\*x)\*cot(y);

\>plot3d("G"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-139.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-139.png)

**Membuat Grafik Fungsi Nilai Mutlak**

$$T(x,y)=|2x^2-y^2|$$\>function T(x,y) &= abs(2\*x^2 - y^2);

\>plot3d("T"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-141.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-141.png)

$$M(x,y)=|-10x^2-3y^2|$$\>function M(x,y) &= abs(-10\*x^2 - 3\*y^2);

\>plot3d("M"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-143.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-143.png)

Rentang Variabel :


\>plot3d("M(x,y)",-15,2,0,8\*pi):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-144.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-144.png)

**Latihan**

Buatlah grafik dari fungsi berikut:


$$A(x,y)=x^2y+3y^2$$\>function A(x,y) &= x^2\*y+3\*y^2;

\>plot3d ("A"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-146.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-146.png)

$$B(x,y)=y^2-2x^2y+4x^3+20x^2$$\>function B(x,y)&= y^2-2\*x^2\*y+4\*x^3+20\*x^2;

\>plot3d("B"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-148.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-148.png)

$$C(x,y)=cosec(9x)-tan(2y)$$\>function C(x,y)&= cosec(9\*x)-tan(2\*y);

\>plot3d ("C"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-150.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-150.png)

Beri rentang variabel untuk fungsi C(x,y):


-100,50,0,2*pi


\>plot3d("C(x,y)",-100,50,0,2\*pi): 


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-151.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-151.png)

### 4.5 Menggambar Data $x$, $y$, $z$ pada ruang Tiga Dimensi (3D)

  Menggambar data pada ruang tiga dimensi (3D) adalah proses  

visualisasi data yang mengubah informasi dalam tiga dimensi, yaitu
panjang, lebar, dan tinggi, menjadi representasi visual yang dapat
dipahami dan dianalisis.


Tujuan dari menggambar data 3D adalah untuk membantu pemahaman dan  

interpretasi data yang lebih baik, terutama ketika data tersebut
memiliki komponen yang tidak dapat direpresentasikan dengan baik dalam
dua dimensi.


Sama seperti plot2d, plot3d menerima data. Untuk objek 3D, kita perlu
menyediakan matriks nilai x-, y- dan z, atau tiga fungsi atau ekspresi
fx(x,y), fy(x,y), fz(x,y).


$$\gamma(t,s) = (x(t,s),y(t,s),z(t,s))$$Karena x,y,z adalah matriks, kita asumsikan bahwa (t,s) melalui sebuah
kotak persegi. Hasilnya, kita dapat memplot gambar persegi panjang di
ruang angkasa.


Kita dapat menggunakan bahasa matriks Euler untuk menghasilkan
koordinat secara efektif.


Dalam contoh berikut, kami menggunakan vektor nilai t dan vektor kolom
nilai s untuk membuat parameter permukaan bola. Dalam gambar kita
dapat menandai daerah, dalam kasus kita daerah kutub.


**Contoh 1 grafik fungsi**

\>t=-1:0.1:1; s=(-1:0.1:1)'; plot3d(t,s,t\*s):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-153.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-153.png)

Penjelasan sintaks dari plot


- plot3d = membawa euler untuk mengetahui perintah apa yang harus
dilakukan


- (” ...”) = tempat kita untuk memasukkan perintah yang kita inginkan


**Contoh 2**

kita akan memebentuk plot dengan fungsi dibawah ini


$$x^2 + y^2$$\>plot3d("x^2+y^2"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-155.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-155.png)

Selanjutnya kita akan menggambar garis pada plot dengan menggunakan
grid


\>plot3d("x^2+y^2",grid=2):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-156.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-156.png)

Jika kita ingin memodifikasi plot dengan menambahkan warna pada plot,
bisa menggunakan fillcolor.


Fillcolor dapat diisi dengan 1 warna yang sama atau 2 warna yang
berbeda


\>plot3d("x^2+y^2",grid= 2,fillcolor=[blue,blue]):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-157.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-157.png)

**Contoh 3**

Jika kita ingin membuat plot 3d pada fungsi


$$2x^2+y^3$$kita bisa menggunakan perintah seperti dibawah ini


\>plot3d("2x^2+y^3",grid=10,\>hue, color=red);

\>insimg()


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-159.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-159.png)

Jika kita mau menebalkan warna pada gambar diatas makam bisa
menggunakan perintah


\>plot3d("2x^2+y^3",grid=10,fillcolor=[red,red]);

\>insimg()


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-160.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-160.png)

**Contoh 4**

Tentu saja, titik cloud juga dimungkinkan. Untuk memplot data titik
dalam ruang, kita membutuhkan tiga vektor untuk koordinat titik-titik
tersebut.


Gayanya sama seperti di plot2d dengan points=true;


\>n=500;...  
\>   plot3d(normal(1,n),normal(1,n),normal(1,n),points=true,style="."):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-161.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-161.png)

**Contoh Soal 5**

Dalam contoh berikut, kita membuat tampilan bayangan dari bola yang  

terdistorsi. Koordinat biasa untuk bola adalah


$$\gamma(t,s) = (\cos(t)\cos(s),\sin(t)\sin(s),\cos(s))$$dengan


$$0 \le t \le 2\pi, \quad \frac{-\pi}{2} \le s \le \frac{\pi}{2}.$$Kami mendistorsi ini dengan sebuah faktor


$$d(t,s) = \frac{\cos(4t)+\cos(8s)}{4}$$\>t=linspace(0,2pi,320); s=linspace(-pi/2,pi/2,160)';...  
\>   d=1+0.2\*(cos(4\*t)+cos(8\*s));...  
\>   plot3d(cos(t)\*cos(s)\*d,sin(t)\*cos(s)\*d,sin(s)\*d,hue=1,...  
\>   light=[1,0,1],frame=0,zoom=5):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-165.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-165.png)

### 4.6 Membuat Gambar Grafik Tiga Dimensi (3D) yang Bersifat Interaktif dan animasi grafik 3D

Membuat gambar grafik tiga dimensi (3D) yang bersifat interaktif
adalah proses menciptakan visualisasi tiga dimensi yang memungkinkan
pengguna berinteraksi dengan objek-objek 3D. Interaktivitas dalam
gambar 3D memungkinkan pengguna untuk melakukan tindakan seperti
mengubah sudut pandang, memindahkan objek, atau berinteraksi dengan
elemen-elemen dalam adegan 3D. Sedangkan animasi grafik 3D dapat
mencakup pergerakan, tetapi juga dapat berarti perubahan dalam
tampilan atau atribut objek tanpa pergerakan fisik yang mencolok.


Interaksi user dimungkinkan dengan parameter &gt;user. dengan perintah
&gt;user kita dapat menekan tombol berikut.


- kiri, kanan, atas, bawah: memutar sudut pandang

- +,-: memperbesar atau memperkecil

- a: menghasilkan anaglyph (lihat di bawah)

- l : tombol nyalakan sumber cahaya (lihat dibawah)

- spasi: reset ke default

- kembali: akhiri interaksi


\>plot3d("exp(-x^2+y^2)",\>user,...  
\>   title="Coba gerakkan"): 


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-166.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-166.png)

\>plot3d("exp(x^2+y^2)",\>user,...  
\>   title="Coba gerakkan)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-167.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-167.png)

**Animasi 3D**

\>function testplot () := plot3d("x^2+y^3");...  
\>   rotate("testplot"); testplot():


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-168.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-168.png)

Fungsi rotate yaitu untuk memutar plot.


Fungsi ini akan membuat animasi plot 3D dari fungsi


$$x^2 + y^3$$

yang berputar di sekitar sumbu z dari sudut 0 hingga 360 derajat


\>plot3d("exp(-(x^2+y^2)/5)",r=10,n=80,fscale=8,scale=1.2,frame=3,\>user):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-170.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-170.png)

Ada beberapa parameter untuk menskalakan fungsi atau mengubah tampilan
grafik.


fscale: menskalakan ke nilai fungsi (defaultnya adalah &lt;fscale).


scale: angka atau vektor 1x2 untuk diskalakan ke arah x dan y.


frame: jenis bingkai (default 1).


\>plot3d("x^2+y",distance=10,zoom=5,angle=0,height=5):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-171.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-171.png)

Tampilan dapat diubah dengan berbagai cara.


- distance: jarak pandang ke plot.
- zoom: nilai zoom.
- angle: sudut terhadap sumbu y negatif dalam radian.
- height: ketinggian tampilan dalam radian.


\>plot3d("x^4+y^2",a=0,b=1,c=-1,d=1,angle=-20°,height=20°,...  
\>   center=[0,0,1],zoom=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-172.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-172.png)

Plot selalu terlihat berada di tengah kubus plot. Kita dapat
memindahkan bagian tengah dengan center parameter.


\>plot3d("x^2+1",a=-1,b=1,rotate=true,grid=5):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-173.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-173.png)

Parameter memutar memutar fungsi dalam x di sekitar sumbu x.


- rotate=1: Menggunakan sumbu x
- rotate=2: Menggunakan sumbu z


### 4.7 Menggambar Fungsi Parametrik Tiga Dimensi (3D)

**Pengertian**

Fungsi parametrik adalah jenis fungsi matematika yang menggambarkan
hubungan antara dua atau lebih variabel, di mana setiap variabel
dinyatakan sebagai fungsi dari satu atau lebih parameter. Fungsi
parametrik digunakan untuk menggambarkan kurva, lintasan, atau
hubungan antara berbagai variabel yang bergantung pada
parameter-parameter tertentu.


Fungsi parametrik merupakan salah satu cara mendefinisikan kurva atau
permukaan dalam ruang 2D atau 3D menggunakan satu atau lebih parameter
independen.


- Dalam 2D, kurva dinyatakan sebagai x(t) dan y(t), di mana adalah t adalah parameter yang mengontrol posisi sepanjang kurva.
- Dalam 3D, kita menggunakan tiga persamaan parametrik untuk mendeskripsikan posisi x,y,z sebagai fungsi dari parameter t.Fungsi ini ditulis sebagai:
   x=f(t),
   y=g(t),
   z=h(t),


**Contoh Soal**

\>plot3d("cos(x)\*cos(y)","sin(x)\*cos(y)","sin(y)", a=0,b=2\*pi,c=pi/2,d=-pi/2,...  
\>   \>hue,color=red,light=[0,1,0],<frame,...  
\>   n=90,grid=[25,50],wirecolor=black,zoom=4):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-174.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-174.png)

\>aspect(16/9); allwindow; ...  
\>   x:=linspace(0,2\*pi,100); y:=(-1:0.1:1)'; ...  
\>   plot3d(sin(x)\*(y/2\*sin(x/2)),cos(x)\*(y/2\*sin(x/2)),y/2\*cos(x/2), ...  
\>   <frame,hue=2,max=0.5,scale=1.5):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-175.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-175.png)

\>aspect(16/9); allwindow;...  
\>   x:=linspace(0,2\*pi,100); y:=(-1:0.1:1)';...  
\>   plot3d(sin(x)\*(y/2\*sin(x/2)),cos(x)\*(y/2\*sin(x/2)),y/2\*cos(x/2),...  
\>   \>lines,<frame,xmin=0,xmax=10,n=10,\>user):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-176.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-176.png)

\>reset;...  
\>   S:=normal(10,1250); plot3d(S[3],S[6],S[9],\>points,style="."):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-177.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-177.png)

\>S:=normal(10,1250); T:=cumsum(normal(10,1250));...  
\>   plot3d(T[2],T[5],T[8],\>wire,...  
\>   linewidth=2,\>anaglyph,zoom=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-178.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-178.png)

\>P=cumsum(normal(5,75));...  
\>   plot3d(P[3],P[4],P[5],\>anaglyph,\>wire):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-179.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-179.png)

### 4.8 Menggambar Fungsi Implisit Tiga Dimensi (3D)

Fungsi implisit (implicit function) adalah fungsi yang memuat lebih
dari satu variabel, berjenis variabel bebas dan variabel terikat yang
berada dalam satu ruas sehingga tidak bisa dipisahkan pada ruas yang
berbeda.


$$F(x,y,z)=0$$

(1 persamaan dan 3 variabel), terdiri dari 2 variabel bebas dan 1
terikat


Misalnya, F(x, y, z) = x^2 + y^2 + z^2 - 1 = 0 adalah persamaan
implisit yang menggambarkan bola dengan jari-jari 1 dan pusat di
(0,0,0).


**Plot Implisit**

Ada juga plot implisit dalam tiga dimensi. Euler menghasilkan
pemotongan melalui objek. Fitur plot3d mencakup plot implisit. Plot
ini menunjukkan himpunan nol suatu fungsi dalam tiga variabel.
Solusi dari


$$f(x,y,z) = 0$$dapat divisualisasikan dalam potongan yang sejajar dengan bidang x-y,
x-z, z-x dan y-z.

- implisit=1: dipotong sejajar bidang y-z
- implisit=2: dipotong sejajar dengan bidang x-z
- implisit=3: dipotong sejajar dengan bidang z-x (yang berarti pemotongan dilakukan dengan mempertahankan nilai y konstan)
- implisit=4: dipotong sejajar bidang x-y

Tambahkan nilai-nilai ini, jika Anda mau. Dalam contoh kita memplot


$$M = \{ (x,y,z) : x^2+y^3+zy=1 \}$$
**Contoh Fungsi Implisit**

\>plot3d("x^2+y^3+z\*y-1",r=7,implicit=4):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-183.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-183.png)

\>plot3d("2\*x^2 + 3\*y^2 + z^2 - 25",r=8,implicit=2):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-184.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-184.png)

\>plot3d("4\*x^3 + 3\*y^4 + 6\*z^2 - 10",r=3,implicit=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-185.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-185.png)

\>plot3d("x^5 + 5\*y^3 + 3\*z^2 - 5\*x - 7\*y - 5\*z + 10",r=5,implicit=2):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-186.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-186.png)

\>plot3d("x^2 + y^2 - z^2",r=5,implicit=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-187.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-187.png)

\>plot3d("x^3 + 2\*y^2 +3\*z^3-4",r=5,implicit=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-188.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-188.png)

\>plot3d("x^2+y^2+z^2+2\*x\*y+4\*y\*z+8\*z\*x-20",r=5,implicit=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-189.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-189.png)

\>c=1; d=1;

\>plot3d("((x^2+y^2-c^2)^2+(z^2-1)^2)\*((y^2+z^2-c^2)^2+(x^2-1)^2)\*((z^2+x^2-c^2)^2+(y^2-1)^2)-d",r=2,<frame,\>implicit,\>user):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-190.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-190.png)

\>c=1; d=1;

\>plot3d("((x^2+y^2+c^2)^2+(z^2-1)^2)\*((y^2+z^2-c^2)^2+(x^2-1)^2)\*((z^2+x^2-c^2)^2+(y^2-1)^2)-d",r=2,<frame,\>implicit,\>user):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-191.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-191.png)

\>plot3d("x^3+y^5+5\*x\*z+z^3",\>implicit,r=3,zoom=2):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-192.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-192.png)

\>plot3d("x^2+y^2+4\*x\*z+z^3-2",\>implicit,r=2,zoom=2.5):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-193.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-193.png)

\>plot3d("x^2\*y^2+x^3+y^3\*x",\>implicit,r=5,zoom=2.5):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-194.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-194.png)

\>plot3d("x\*y-z^2+2\*x\*y\*z-0",\>implicit,r=5,zoom=2.5):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-195.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-195.png)

**Latihan soal**

1. Gambarlah Fungsi implisit berikut dalam 3D


$$f(x,y,z)=x^2+y^2-z^2-1$$\>plot3d("x^2+y^2-z^2-1",r=8,implicit=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-197.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-197.png)

2. Gambarlah fungsi 3D dari fungsi implisit berikut ini


$$f(x,y,z)=xy+x^3y^2+xz^3-9=0$$

dengan r=4


\>plot3d("x\*y+x^3\*y^2+x\*z^3-9", r=4, implicit=3):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-199.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-199.png)

### 4.9 Mengatur tampilan, warna dan sudut pandang gambar permukaan

**Tiga Dimensi (3D) Dan Menampilkan kontur dan bidang kontur permukaan Tiga Dimensi(3D)**

Untuk plot, Euler menambahkan garis grid. Sebagai gantinya
dimungkinkan untuk menggunakan garis level dan rona satu warna atau
rona berwarna spektral. Euler dapat menggambar tinggi fungsi pada plot
dengan bayangan. Di semua plot 3D, Euler dapat menghasilkan anaglyph
merah/sian.


- hue: Menyalakan bayangan cahaya alih-alih kabel.

- kontur: Memplot garis kontur otomatis pada plot.

- level=... (atau level): Sebuah vektor nilai untuk garis kontur.


Standarnya adalah level="auto", yang menghitung beberapa garis level
secara otomatis. Seperti yang Anda lihat di plot, level sebenarnya
adalah rentang level.


Gaya default dapat diubah. Untuk plot kontur berikut, kami menggunakan
grid yang lebih halus untuk 100x100 poin, skala fungsi dan plot, dan
menggunakan sudut pandang yang berbeda.


\>plot3d("exp(-x^2-y^2)",r=2,n=100,level="thin", ...  
\>    \>contour,\>spectral,fscale=1,scale=1.1,angle=45°,height=20°):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-200.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-200.png)

\>plot3d("exp(x\*y)",angle=100°,\>contour,color=green):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-201.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-201.png)

Bayangan default menggunakan warna abu-abu. Tetapi rentang warna
spektral juga tersedia.


-&gt; spektral: Menggunakan skema spektral default


- color=...: Menggunakan warna khusus atau skema spektral


Untuk plot berikut, kami menggunakan skema spektral default dan
menambah jumlah titik untuk mendapatkan tampilan yang sangat halus.


\>plot3d("x^2+y^2",\>spectral,\>contour,n=100):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-202.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-202.png)

Alih-alih garis level otomatis, kita juga dapat mengatur nilai garis
level. Ini akan menghasilkan garis level tipis alih-alih rentang
level.


\>plot3d("x^2-y^2",0,1,0,1,angle=220°,level=-1:0.2:1,color=redgreen):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-203.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-203.png)

Dalam plot berikut, kami menggunakan dua pita level yang sangat luas
dari -0,1 hingga 1, dan dari 0,9 hingga 1. Ini dimasukkan sebagai
matriks dengan batas level sebagai kolom.


Selain itu, kami melapisi kisi dengan 10 interval di setiap arah.


\>plot3d("x^2+y^3",level=[-0.1,0.9;0,1], ...  
\>     \>spectral,angle=30°,grid=10,contourcolor=gray):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-204.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-204.png)

Dalam contoh berikut, kami memplot himpunan, di mana


$$f(x,y) = x^y-y^x = 0$$Kami menggunakan satu garis tipis untuk garis level.


\>plot3d("x^y-y^x",level=0,a=0,b=6,c=0,d=6,contourcolor=red,n=100):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-206.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-206.png)

Dimungkinkan untuk menunjukkan bidang kontur di bawah plot. Warna dan
jarak ke plot dapat ditentukan.


\>plot3d("x^2+y^4",\>cp,cpcolor=green,cpdelta=0.2):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-207.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-207.png)

Berikut adalah beberapa gaya lagi. Kami selalu mematikan frame, dan
menggunakan berbagai skema warna untuk plot dan grid.


\>figure(2,2); ...  
\>   expr="y^3-x^2"; ...  
\>   figure(1);  ...  
\>     plot3d(expr,<frame,\>cp,cpcolor=spectral); ...  
\>   figure(2);  ...  
\>     plot3d(expr,<frame,\>spectral,grid=10,cp=2); ...  
\>   figure(3);  ...  
\>     plot3d(expr,<frame,\>contour,color=gray,nc=5,cp=3,cpcolor=greenred); ...  
\>   figure(4);  ...  
\>     plot3d(expr,<frame,\>hue,grid=10,\>transparent,\>cp,cpcolor=gray); ...  
\>   figure(0):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-208.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-208.png)

Ada beberapa skema spektral lainnya, bernomor dari 1 hingga 9. Tetapi
Anda juga dapat menggunakan warna=nilai, di mana nilai


- spektral: untuk rentang dari biru ke merah
- putih: untuk rentang yang lebih redup
- kuningbiru,ungu hijau,birukuning,hijaumerah
- birukuning, hijau ungu, kuning biru, merah hijau


\>figure(3,3); ...  
\>   for i=1:9;  ...  
\>     figure(i); plot3d("x^2+y^2",spectral=i,\>contour,\>cp,<frame,zoom=4);  ...  
\>   end; ...  
\>   figure(0):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-209.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-209.png)

Sumber cahaya dapat diubah dengan l dan tombol kursor selama interaksi
pengguna. Itu juga dapat diatur dengan parameter.

- cahaya: arah untuk cahaya
- amb: cahaya sekitar antara 0 dan 1


Perhatikan bahwa program tidak membuat perbedaan antara sisi plot.
Tidak ada bayangan. Untuk ini, Anda perlu Povray.


\>plot3d("-x^2-y^2", ...  
\>     hue=true,light=[0,1,1],amb=0,user=true, ...  
\>     title="Press l and cursor keys (return to exit)"):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-210.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-210.png)

Parameter warna mengubah warna permukaan. Warna garis level juga dapat
diubah.


\>plot3d("-x^2-y^2",color=rgb(0.2,0.2,0),hue=true,frame=false, ...  
\>     zoom=3,contourcolor=red,level=-2:0.1:1,dl=0.01):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-211.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-211.png)

Warna 0 memberikan efek pelangi khusus.


\>plot3d("x^2/(x^2+y^2+1)",color=0,hue=true,grid=10):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-212.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-212.png)

Permukaannya juga bisa transparan.


\>plot3d("x^2+y^2",\>transparent,grid=10,wirecolor=red):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-213.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-213.png)

### 4.10 Menggambar Diagram Batang Tiga Dimensi

Bar plots/plot batang juga dimungkinkan. Untuk itu, kita harus
menyediakannya

- x: vektor baris dengan n+1 elemen
- y: vektor kolom dengan n+1 elemen
- z: matriks nilai nxn.


z bisa lebih besar, tetapi hanya nilai nxn yang akan digunakan.


Dalam contoh ini, pertama-tama kita menghitung nilainya. Kemudian kita
sesuaikan x dan y, sehingga vektor-vektornya berpusat pada nilai yang
digunakan.


\>x=-1:0.1:1; y=x'; z=x^2+y^2; ...  
\>   xa=(x|1.1)-0.05; ya=(y\_1.1)-0.05; ...  
\>   plot3d(xa,ya,z,bar=true):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-214.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-214.png)

\>x=-0.01:0.1:1; y=x'; z=x+2/3\*y; ...  
\>   xa=(x|1.1)-0.05; ya=(y\_1.1)-0.05; ...  
\>   plot3d(xa,ya,z,bar=true):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-215.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-215.png)

\>x=-0.01:0.1:1; y=x'; z=1/2\*x+1/2\*y; ...  
\>   xa=(x|1.1); ya=(y\_1.1); ...  
\>   plot3d(xa,ya,z,bar=true):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-216.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-216.png)

Dimungkinkan untuk membagi plot suatu permukaan menjadi dua bagian
atau lebih.


\>x=-1:0.1:1; y=x'; z=1/10\*x+1/10\*y; d=zeros(size(x)); ...  
\>   plot3d(x,y,z,disconnect=2:2:5):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-217.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-217.png)

\>x=-1:0.1:1; y=x'; z=x+y; d=zeros(size(x)); ...  
\>   plot3d(x,y,z,disconnect=2:2:20):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-218.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-218.png)

Jika memuat atau menghasilkan matriks data M dari file dan perlu
memplotnya dalam 3D, Anda dapat menskalakan matriks ke [-1,1] dengan
skala(M), atau menskalakan matriks dengan &gt;zscale. Hal ini dapat
dikombinasikan dengan faktor penskalaan individual yang diterapkan
sebagai tambahan.


\>i=1:20; j=i'; ...  
\>   plot3d(i\*j^2+100\*normal(20,20),\>zscale,scale=[1,1,1.5],angle=-40°,zoom=1.8):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-219.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-219.png)

\>Z=intrandom(5,100,6); v=zeros(5,6); ...  
\>   loop 1 to 5; v[#]=getmultiplicities(1:6,Z[#]); end; ...  
\>   columnsplot3d(v',scols=1:5,ccols=[1:5]):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-220.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-220.png)

\>Z=intrandom(6,100,6); v=zeros(6,2); ...  
\>   loop 1 to 6; v[#]=getmultiplicities(1:2,Z[#]); end; ...  
\>   columnsplot3d(v',scols=1:6,ccols=[1:6]):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-221.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-221.png)

\>Z=intrandom(7,1000,6); v=zeros(7,1); ...  
\>   loop 1 to 7; v[#]=getmultiplicities(1:1,Z[#]); end; ...  
\>   columnsplot3d(v',scols=1:7,ccols=[1:7]):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-222.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-222.png)

### 4.11 Menggambar Permukaan Benda Putar

\>plot2d("(x^2+y^2-1)^3-x^2\*y^3",r=1.3, ...  
\>   style="#",color=red,<outline, ...  
\>   level=[-2;0],n=100):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-223.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-223.png)

\>ekspresi &= (x^2+y^2-1)^3-x^2\*y^3; $ekspresi


$$\left(y^2+x^2-1\right)^3-x^2\,y^3$$Kami ingin memutar kurva jantung di sekitar sumbu y. Berikut adalah
ungkapan, yang mendefinisikan hati:


$$f(x,y)=(x^2+y^2-1)^3-x^2.y^3.$$Selanjutnya kita atur


$$x=r.cos(a),\quad y=r.sin(a).$$\>function fr(r,a) &= ekspresi with [x=r\*cos(a),y=r\*sin(a)] | trigreduce; $fr(r,a)


$$\left(r^2-1\right)^3+\frac{\left(\sin \left(5\,a\right)-\sin \left(3\,a\right)-2\,\sin a\right)\,r^5}{16}$$Hal ini memungkinkan untuk mendefinisikan fungsi numerik, yang
memecahkan r, jika a diberikan. Dengan fungsi itu kita dapat memplot
jantung yang diputar sebagai permukaan parametrik.


\>function map f(a) := bisect("fr",0,2;a); ...  
\>   t=linspace(-pi/2,pi/2,100); r=f(t);  ...  
\>   s=linspace(pi,2pi,100)'; ...  
\>   plot3d(r\*cos(t)\*sin(s),r\*cos(t)\*cos(s),r\*sin(t), ...  
\>   \>hue,<frame,color=red,zoom=4,amb=0,max=0.7,grid=12,height=50°):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-228.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-228.png)

Berikut ini adalah plot 3D dari gambar di atas yang diputar di sekitar
sumbu z. Kami mendefinisikan fungsi, yang menggambarkan objek.


\>function f(x,y,z) ...


    r=x^2+y^2;
    return (r+z^2-1)^3-r*z^3;
     endfunction
</pre>
\>plot3d("f(x,y,z)", ...  
\>   xmin=0,xmax=1.2,ymin=-1.2,ymax=1.2,zmin=-1.2,zmax=1.4, ...  
\>   implicit=1,angle=-30°,zoom=2.5,n=[10,60,60],\>anaglyph):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-229.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-229.png)

### 4.12 Menggambar Grafik 3D dengan Povray di EMT

Menggambar Povray Dengan bantuan file Euler povray.e, Euler dapat
menghasilkan file Povray. Hasilnya sangat bagus untuk dilihat.


Untuk dapat menjalankan sintaks dalam povray perlu menginstal Povray
(32bit atau 64bit) dari http://www.povray.org/, dan meletakkan
sub-direktori "bin" dari Povray ke pathway, atau mengatur variabel
"defaultpovray" dengan path lengkap yang menunjuk ke "pvengine.exe".


Interface Povray dari Euler menghasilkan file Povray di direktori home
pengguna, dan memanggil Povray untuk mengurai file-file ini. Nama file
default adalah current.pov, dan direktori default adalah eulerhome(),
biasanya c:\Users\Username\Euler. Povray menghasilkan file PNG, yang
dapat dimuat oleh Euler ke dalam buku catatan. Untuk membersihkan
file-file ini, gunakan povclear().


Sintaks yang digunakan untuk menjalankan povray adalah pov3d. Fungsi
pov3d memiliki komponen yang sama dengan plot3d. Ini dapat
menghasilkan grafik fungsi f(x,y), atau permukaan dengan koordinat
X,Y,Z dalam matriks, termasuk garis level opsional. Fungsi ini memulai
raytracer secara otomatis, dan memuat gambar ke dalam notebook Euler.


Selain pov3d(), ada banyak fungsi yang menghasilkan objek Povray.
Fungsi-fungsi ini mengembalikan string, yang berisi kode Povray untuk
objek. Untuk menggunakan fungsi ini, mulai file Povray dengan
povstart(). Kemudian gunakan writeln(...) untuk menulis objek ke file
gambar. Terakhir, akhiri file dengan povend(). Secara default,
raytracer akan dimulai, dan PNG akan dimasukkan ke dalam notebook
Euler.


Fungsi objek memiliki parameter yang disebut "look", yang membutuhkan
string dengan kode Povray untuk tekstur dan hasil akhir objek. Fungsi
povlook() dapat digunakan untuk menghasilkan string ini. Ini memiliki
parameter untuk warna, transparansi, Phong Shading dll.


Lingkup Povray memiliki sistem koordinat lain. Interface ini
menerjemahkan semua koordinat ke sistem Povray. Jadi Anda dapat terus
berpikir dalam sistem koordinat Euler dengan z menunjuk vertikal ke
atas, dan x,y,z sumbu dalam arti tangan kanan.


Anda perlu memuat file povray.


\>load povray;


Pastikan, direktori bin Povray ada di path. Jika tidak, edit variabel
berikut sehingga berisi path ke povray yang dapat dieksekusi.


\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

**Contoh Penggunaan**

Akan diberikan contoh sederhana penggunaan povray pada EMT


Perintah berikut menghasilkan file povray di direktori pengguna dan
menjalankan Povray untuk ray tracing file ini.


Jika memulai perintah berikut, GUI Povray akan terbuka, menjalankan
file, dan menutup secara otomatis. Karena alasan keamanan, akan
ditanya, apakah ingin mengizinkan file exe untuk dijalankan. Agar
pertanyaan tersebut tidak muncul lagi bisa dipilih batal.


\>pov3d("x^2+y^2",zoom=4);


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-230.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-230.png)

hasil visualisasi fungsi dapat dibuat menjadi transparan dan
menambahkan hasil akhir lainnya.


\> pov3d("(x^2+y^3)",axiscolor=green,angle=30°, ...  
\>     look=povlook(yellow,0.2),level=-1:0.5:1,zoom=3);


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-231.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-231.png)

\>pov3d("((x-1)^2+(y+1)^2)\*((x+1)^2+y^2)/40",r=1.5, ...  
\>     angle=120°,level=1/40,dlevel=0.005,light=[-1,1,1],height=45°,n=50, ...  
\>     <fscale,zoom=3.8);


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-232.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-232.png)

**Object Povray**

Contoh-contoh di atas tadi merupakan visualisasi permukaan fungsi
dengan menggunakan sintaks pov3d. Untuk menghasilkan objek dalam
povray perlu ditulis menjadi file povray.


Untuk menghasilkan output dimulai dengan povstart()


\>load povray; ...  
\>   defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

\>povstart(zoom=3.5)

\>c1=povcylinder(-povx,povx,1,povlook(orange)); ...  
\>   c2=povcylinder(-povy,povy,1,povlook(yellow)); ...  
\>   c3=povcylinder(-povz,povz,1,povlook(lightblue));


Di atas telah didefinisikan tiga silinder yang disimpan dalam string di Euler. Fungsi povx(), povy(), dll. hanya mengembalikan vektor [1,0,0] yang dapat digunakan sebagai gantinya.


\>c1


    cylinder { &lt;-1,0,0&gt;, &lt;1,0,0&gt;, 1
     texture { pigment { color rgb &lt;0.941176,0.509804,0.392157&gt; }  } 
     finish { ambient 0.2 } 
     }

Akan ditambahkan tekstur ke objek dengan tiga warna berbeda yaitu
orange, yellow, dan lightblue.


Untuk menamahkan tekstur ini dapat digunakan sintaks povlook(), yang
mengembalikan string dengan kode Povray yang relevan. Selain
menambahkan warna, ditambahkan juga transparansi dan cahaya.


\>povlook(rgb(0.1,0.2,0.3),0.1,0.5)


     texture { pigment { color rgbf &lt;0.101961,0.2,0.301961,0.1&gt; }  } 
     finish { ambient 0.5 } 
    

\>writeln(povintersection([c1,c2,c3]));

\>povend;


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-233.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-233.png)

**Contoh Lain**

Akan ditampilkan fungsi untuk membuat sebuah donat


\>povstart(angle=0,height=45°); //height untuk menampilkan fungsi dengan suatiu derajat tertentu 

\>function povdonat (r1,r2,look="") := "torus {"+r1+","+r2+look+"}"; //fungsi untuk menampilkan sebuah donat

\>writeln(povobject(povdonat(1,0.5),povlook(lightblue,\>phong),xrotate(90°)));

\>povend();


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-234.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-234.png)

### 4.13 Menggambar Grafik Tiga Dimensi alam modus anaglif

Untuk menghasilkan anaglyph untuk kacamata merah/sian, Povray harus
berjalan dua kali dari posisi kamera yang berbeda. Ini menghasilkan
dua file Povray dan dua file PNG, yang dimuat dengan fungsi
loadanaglyph().


Tentu saja, Anda memerlukan kacamata merah/sian untuk melihat contoh
berikut dengan benar.


Fungsi pov3d() memiliki sakelar sederhana untuk menghasilkan
anaglyphs.


\>pov3d("-exp(-x^2-y^2)/2",r=2,height=45°,\>anaglyph, ...  
\>     center=[0,0,0.5],zoom=3.5);


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-235.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-235.png)

Jika Anda membuat adegan dengan objek, Anda perlu menempatkan generasi
adegan ke dalam fungsi, dan menjalankannya dua kali dengan nilai yang
berbeda untuk parameter anaglyph.


\>function myscene ...


      s=povsphere(povc,1);
      cl=povcylinder(-povz,povz,0.5);
      clx=povobject(cl,rotate=xrotate(90°));
      cly=povobject(cl,rotate=yrotate(90°));
      c=povbox([-1,-1,0],1);
      un=povunion([cl,clx,cly,c]);
      obj=povdifference(s,un,povlook(red));
      writeln(obj);
      writeAxes();
    endfunction
</pre>
Fungsi povanaglyph() melakukan semua ini. Parameternya seperti di
povstart() dan povend() digabungkan.


\>povanaglyph("myscene",zoom=4.5);


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-236.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-236.png)

### 4.14 Fungsi Implisit menggunakan Povray

Povray dapat memplot himpunan di mana f(x,y,z)=0, seperti parameter
implisit di plot3d. Namun hasilnya terlihat jauh lebih baik.


Sintaks untuk fungsinya sedikit berbeda. Anda tidak dapat menggunakan
keluaran ekspresi Maxima atau Euler.


\>load povray;

\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

\>povstart(angle=25°,height=10°);

\>writeln(povsurface("pow(x,2)+pow(y,2)\*pow(z,2)-1",povlook(blue),povbox(-2,2,"")));

\>povend();


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-237.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-237.png)

\>load povray;

\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

\>povstart(angle=70°,height=50°,zoom=4);

\>writeln(povsurface("pow(x,2)\*y-pow(y,3)-pow(z,2)",povlook(green))); ...  
\>   writeAxes(); ...  
\>   povend();


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-238.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-238.png)

\>load povray;

\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

\>povstart(angle=70°,height=30°);

\>writeln(povsurface("pow(x,2)+pow(y,2)\*pow(z,2)-1",povlook(red),povbox(-2,2,"")));

\>povend();


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-239.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-239.png)

### 4.15 Menggambar Titik pada ruang Tiga Dimensi (3D)

Alih-alih fungsi, kita dapat memplot dengan koordinat. Seperti pada plot3d, kita membutuhkan tiga matriks untuk mendefinisikan objek.


Dalam contoh kita memutar fungsi di sekitar sumbu z.


\>function f(x) := x^3-x+1; ...  
\>   x=-1:0.01:1; t=linspace(0,2pi,8)'; ...  
\>   Z=x; X=cos(t)\*f(x); Y=sin(t)\*f(x); ...  
\>   pov3d(X,Y,Z,angle=40°,height=20°,axis=0,zoom=4,light=[10,-5,5]);


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-240.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-240.png)

Dalam contoh berikut, kami memplot gelombang teredam. Kami
menghasilkan gelombang dengan bahasa matriks Euler.


Kami juga menunjukkan, bagaimana objek tambahan dapat ditambahkan ke
adegan pov3d. Untuk pembuatan objek, lihat contoh berikut. Perhatikan
bahwa plot3d menskalakan plot, sehingga cocok dengan kubus satuan.


\>r=linspace(0,1,80); phi=linspace(0,2pi,80)'; ...  
\>   x=r\*cos(phi); y=r\*sin(phi); z=exp(-5\*r)\*cos(8\*pi\*r)/3;  ...  
\>   pov3d(x,y,z,zoom=5,axis=0,add=povsphere([0,0,0.5],0.1,povlook(green)), ...  
\>     w=500,h=300);


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-241.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-241.png)

Dengan metode bayangan canggih dari Povray, sangat sedikit titik yang
dapat menghasilkan permukaan yang sangat halus. Hanya di perbatasan
dan dalam bayang-bayang triknya mungkin menjadi jelas.


Untuk ini, kita perlu menambahkan vektor normal di setiap titik
matriks.


\>Z &= x^2\*y^3


    
                                     2  3
                                    x  y
    

Persamaan permukaannya adalah [x,y,Z]. Kami menghitung dua turunan ke
x dan y ini dan mengambil produk silang sebagai normal.


\>dx &= diff([x,y,Z],x); dy &= diff([x,y,Z],y);


Kami mendefinisikan normal sebagai produk silang dari turunan ini, dan
mendefinisikan fungsi koordinat.


\>N &= crossproduct(dx,dy); NX &= N[1]; NY &= N[2]; NZ &= N[3]; N,


    
                                   3       2  2
                           [- 2 x y , - 3 x  y , 1]
    

Kami hanya menggunakan 25 poin.


\>x=-1:0.5:1; y=x';

\>pov3d(x,y,Z(x,y),angle=10°, ...  
\>     xv=NX(x,y),yv=NY(x,y),zv=NZ(x,y),<shadow);


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-242.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-242.png)

Berikut ini adalah simpul Trefoil yang dilakukan oleh A. Busser di
Povray. Ada versi yang ditingkatkan dari ini dalam contoh.


  <a href="Contoh\Trefoil Simpul.html">Simpul trefoil</a>  

Untuk tampilan yang bagus dengan tidak terlalu banyak titik, kami
menambahkan vektor normal di sini. Kami menggunakan Maxima untuk
menghitung normal bagi kami. Pertama, ketiga fungsi koordinat sebagai
ekspresi simbolik.


\>X &= ((4+sin(3\*y))+cos(x))\*cos(2\*y); ...  
\>   Y &= ((4+sin(3\*y))+cos(x))\*sin(2\*y); ...  
\>   Z &= sin(x)+2\*cos(3\*y);


Kemudian kedua vektor turunan ke x dan y.


\>dx &= diff([X,Y,Z],x); dy &= diff([X,Y,Z],y);


Sekarang normal, yang merupakan produk silang dari dua turunan.


\>dn &= crossproduct(dx,dy);


Kami sekarang mengevaluasi semua ini secara numerik.


\>x:=linspace(-%pi,%pi,40); y:=linspace(-%pi,%pi,100)';


Vektor normal adalah evaluasi dari ekspresi simbolik dn[i] untuk
i=1,2,3. Sintaks untuk ini adalah &amp;"expression"(parameters). Ini
adalah alternatif dari metode pada contoh sebelumnya, di mana kita
mendefinisikan ekspresi simbolik NX, NY, NZ terlebih dahulu.


\>pov3d(X(x,y),Y(x,y),Z(x,y),axis=0,zoom=5,w=450,h=350, ...  
\>     <shadow,look=povlook(gray), ...  
\>     xv=&"dn[1]"(x,y), yv=&"dn[2]"(x,y), zv=&"dn[3]"(x,y));


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-243.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-243.png)

Kami juga dapat menghasilkan grid dalam 3D.


\>povstart(zoom=4); ...  
\>   x=-1:0.5:1; r=1-(x+1)^2/6; ...  
\>   t=(0°:30°:360°)'; y=r\*cos(t); z=r\*sin(t); ...  
\>   writeln(povgrid(x,y,z,d=0.02,dballs=0.05)); ...  
\>   povend();


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-244.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-244.png)

With povgrid(), curves are possible.


\>povstart(center=[0,0,1],zoom=3.6); ...  
\>   t=linspace(0,2,1000); r=exp(-t); ...  
\>   x=cos(2\*pi\*10\*t)\*r; y=sin(2\*pi\*10\*t)\*r; z=t; ...  
\>   writeln(povgrid(x,y,z,povlook(red))); ...  
\>   writeAxis(0,2,axis=3); ...  
\>   povend();


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-245.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-245.png)

**Latihan Soal**

1. Buatlah plot 3D dari fungsi


$$f(x,y)=x^3+3y^2$$

dengan zoom 3 dan angle 55 derajat menggunakan povray


\>pov3d("x^3+3\*y^2",zoom=3,angle=55°);


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-247.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-247.png)

2. Buatlah gabungan 2 silinder dengan fungsi povx() berwarna merah dan
povz() berwarna kuning dan zoom 4


\>povstart(zoom=4)

\>c1 = povcylinder (-povx,povx,1,povlook(red));

\>c2 = povcylinder (-povz,povz,1,povlook(yellow));

\>writeln(povintersection([c1,c2]));

\>povend();


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-248.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-248.png)

\> 


3. Buatlah grafik 3D dari fungsi kuadrat berikut ini dengan parameter
tambahan:


$$z=4x^2-2y^2$$

Tampilkan grafik tersebut dengan transparent, dan menggunakan grid
dengan resolusi 50, dengan warna biru pada garis di plot tersebut


\>plot3d("4\*x^2-2\*y^2",\>transparent,grid=50,wirecolor=blue):


![images/EMT_Grafik3D_Alfi%20Nur%20Azumah-250.png](images/EMT_Grafik3D_Alfi%20Nur%20Azumah-250.png)

