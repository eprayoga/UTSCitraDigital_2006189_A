# UTSCitraDigital_2006189_A
UTS Citra Digital Kelas A NIM 2006189

Nama : Endang Prayoga Hidayatulloh
NIM  : 2006189

## Google Colab
Maaf bu karena file yang terlalu besar tidak bisa ditampilkan langsung di Github
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DsIGhVwSGIcFO8eLIuwVxHzUkIqvqmoe) (Online Demo)

# Import Module yang di butuhkan
Beberapa module yang dibutuhkan yaitu:
*   cv2
*   numpy
*   matplotlib.plt
*   cv2_imshow dari google.colab.patches
*   io dari skimage
*   Image dari PIL

#Image
!(image)[https://lh4.googleusercontent.com/UzZJxATg_h4WnrZL1W8rSgbEAioX5Q9MJPWDqy2QCNfsTSn22-7BK6xqQ1TkU2vCMMI=w2400]

# Pembahasan
## Mengambil dan menampilkan Image
membuat variabel "url" yang menampung link dari gambar,

membuat variabel image yang menampung file gambar yang diperoleh dengan menggunakan function io.imread dengan parameter url yang telah dibuat,

Mengconvert image yang asalnya GBR menjadi RGB katena hasil return dari variabel image mempunyai mode warna GBR. Konversi itu menggunakan modul dari cv2 dengan method cvtColor argumen image dan ditambah parameter cv.COLOR_BGR2RGB

menggabungkan 2 variabel image dengan menggunakan fungsi hconcat dari cv2. yang ditampung pada variabel final_frame.

menampilkan hasil gabungan image yaitu variabel final_frame dengan menggunakan cv2_imshow


## Membuat Histogram dan Menampilkan Histogram
Membuat histogram dengan menggunakan module dari numpy dengan metod hist.
Menampilkan histogram dengan menggunakan modul dari matplotlob.pyplot yanf didalamnya berisi hasil dari varibel yang menampung hsitogram

## Membuat split Chanel RGB
Memilahkan chanel RGB bisa menggunakan function image
- Blue chanel = image[:,:,0]
- Green chanel = image[:,:,1]
- Red chanel = image[:,:,2]

## Grayscale image
menggunakan module dari CV dengan merhod cvtColor dan dengan parameter image, dan BGR2GRAY

## Invert Image
Menggunakan rumus gray image yang menggunakan gray scale
invert_gray = 255 - gray_image

## Bright Image
bright_image = (100.0/255)*gray_image + 100

## Drak Image
darken_image = 255.0*(gray_image/255.0)**2

# Kesimpulan
Dengan mengunakan plot dari modul numpy dan ditampilkan dengan modul dari matplotlin.pyplot, kita dapat melihat histogram dari image yang kita gunakan. Dari image yang telah saya gunakan dapat dilihat bahwa image yang digunakan mempunyai citra terang karena plot berada di bagian kanan.


Note : Maaf Bu File yang di upload terlalu besar dan tidak bisa di buka di github langsung
