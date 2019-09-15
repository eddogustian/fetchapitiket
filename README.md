# fetchapitiket
Fetching API to Get data Tiket.com

Generate Secret Key and Token
Oke, pertama buatlah sebuah akun dengan meng-click http://www.tiket.com/affiliate
Kemudian masukan semua data-data anda lengkap sehingga ada akan bisa melakukan login pada : https://www.tiket.com/partner/login

Setelah melakukan login, pada bagian API anda akan melihat secret key milik anda yg akan dipakai untuk mendapatkan token yg berfungsi sebagai hak akses anda membaca data dari API yg disediakan.
Secret Key bisa anda lihat pada bagian : API secret key development

sebagai contoh gambaran saja : 
Setelah mendapatkan secret key, sekarang proses selanjutnya adalah generate Token. Pada address bar anda, silahkan copas link berikut :
https://api.master18.tiket.com/apiv1/payexpress?method=getToken&secretkey=DiisiDenganSeretKeyAnda

Pada bagian akhir link diatas, terlihat saya memberi perintah untuk memasukan secret key milik anda. Contoh :
https://api.master18.tiket.com/apiv1/payexpress?method=getToken&secretkey=e10adc3949ba59abbe56e057f20f883e

Setelah mengisi scret key yg valid, tekan enter / proses. Anda kemudian akan mendapatkan return data TOKEN anda. Balasan yg didapat kira-kira seperti ini :

Bentuk XML :
<tiket>
    <output_type>xml</output_type>
    <diagnostic>
        <elapstime>0.1385</elapstime>
        <memoryusage>4.49MB</memoryusage>
        <status>200</status>
        <lang>en</lang>
        <currency>IDR</currency>
    </diagnostic>
    <token>38d1996c567c688e1b285f464a12ea83</token>
</tiket>

Bentuk JSON :
{"output_type":"json","diagnostic":{"elapstime":"0.1201","memoryusage":"4.46MB","status":"200","lang":"en","currency":"IDR"},"token":"38d1996c567c688e1b285f464a12ea83"}

Biasanya sih dalam bentuk array, tapi bisa anda lihat token-nya seperti pada contoh : "token":"38d1996c567c688e1b285f464a12ea83"

Sampai disini langkah anda mendapatkan token sudah selesai.

