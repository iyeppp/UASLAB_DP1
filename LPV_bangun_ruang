program LP_dan_V_BangunRuang;
uses crt;

const total = 7; //konstanta untuk jumlah bangun ruang dan phi untuk bola
    phi = 3.14;

type bangun_ruang1 = record //array of record untuk nama setiap bangun ruang
    nama: string;
    end;

var bangun_ruang : array[1..total] of bangun_ruang1;
    sisi, panjang, lebar, tinggi, llingkaran, klingkaran, kalas, lalas,lselimut, jari, sisi_tegak, lp, v : real; //variabel yang dibutuhkan untuk perhitungan
    pilih : integer; //variabel untuk memilih bangun ruang
    lagi : char; //variabel untuk perulangan


procedure inisialisasi_nama; //subprogram pertama untuk menginisialisasi setiap nama bangun ruang
begin
    bangun_ruang[1].nama := 'Kubus';
    bangun_ruang[2].nama := 'Balok';
    bangun_ruang[3].nama := 'Tabung';
    bangun_ruang[4].nama := 'Prisma';
    bangun_ruang[5].nama := 'Kerucut';
    bangun_ruang[6].nama := 'Bola';
    bangun_ruang[7].nama := 'Limas';
end;

procedure header; //subprogram kedua untuk header atau tampilan awal program
var i : integer;
begin
    writeln('Selamat Datang di Program Pencari LP/V Bangun Ruang');
    for i := 1 to total do //perulangan
    begin
        writeln(i, '. ', bangun_ruang[i].nama);
    end;
end;

begin
inisialisasi_nama; //subprogram pertama
    repeat //memulai perulangan
    clrscr;   
    header; //subprogram kedua
    write('Silahkan Pilih Bangun Ruang Yang Anda Inginkan : ');
    readln(pilih); //pilihan bangun ruang
writeln;
    case pilih of //operasi kondisi untuk setiap bangun ruang
    1: begin
       writeln('Anda Memilih Bangun Ruang   : ', bangun_ruang[1].nama);
       write('Masukkan Panjang Sisi kubus : '); readln(sisi);
       lp := 6 * sisi * sisi;
       v := sisi * sisi * sisi;
       writeln('Luas Permukaan Kubus Adalah : ', lp:0:2);
       writeln('Volume Kubus Adalah         : ', v:0:2);
       end;

    2: begin
       writeln('Anda Memilih Bangun Ruang   : ', bangun_ruang[2].nama);
       write('Masukkan Panjang Balok      : '); readln(panjang);
       write('Masukkan Lebar Balok        : '); readln(lebar);
       write('Masukkan Tinggi Balok       : '); readln(tinggi);
       lp := 2 * ((panjang * lebar) + (panjang * tinggi) + (lebar * tinggi));
       v := panjang * lebar * tinggi;
       writeln('Luas Permukaan Balok Adalah : ', lp:0:2);
       writeln('Volume Balok Adalah         : ', v:0:2);
       end;

    3: begin
       writeln('Anda Memilih Bangun Ruang   : ', bangun_ruang[3].nama);
       write('Masukkan Luas Lingkaran     : '); readln(llingkaran);
       write('Masukkan Keliling Lingkaran : '); readln(klingkaran);
       write('Masukkan Tinggi Tabung      : '); readln(tinggi);
       lp := 2 * llingkaran + klingkaran * tinggi;
       v := llingkaran * tinggi;
       writeln('Luas Permukaan Tabung Adalah: ', lp:0:2);
       writeln('Volume Tabung Adalah        : ', v:0:2);
       end;

    4: begin
       writeln('Anda Memilih Bangun Ruang   : ', bangun_ruang[4].nama);
       write('Masukkan Jumlah Sisi Tegak  : '); readln(sisi_tegak);
       write('Masukkan Keliling Alas      : '); readln(kalas);
       write('Masukkan Luas Alas          : '); readln(lalas);
       write('Masukkan Tinggi Prisma      : '); readln(tinggi);
       lp := (sisi_tegak * kalas) +  (2 * lalas);
       v := lalas * tinggi;
       writeln('Luas Permukaan Prisma Adalah: ', lp:0:2);
       writeln('Volume Prisma Adalah        : ', v:0:2);
       end;

    5: begin
       writeln('Anda Memilih Bangun Ruang    : ', bangun_ruang[5].nama);
       write('Masukkan Luas Selimut        : '); readln(lselimut);
       write('Masukkan Tinggi              : '); readln(tinggi);
       write('Masukkan Luas Alas           : '); readln(lalas);
       lp := lalas + lselimut;
       v := (lalas * tinggi) / 3;
       writeln('Luas Permukaan Kerucut Adalah: ', lp:0:2);
       writeln('Volume Kerucut Adalah        : ', v:0:2);
       end;

    6: begin
       writeln('Anda Memilih Bangun Ruang    : ', bangun_ruang[6].nama);
       write('Masukkan Luas Lingkaran      : '); readln(llingkaran);
       write('Masukkan Jari-Jari Lingkaran : '); readln(jari);
       lp := 4 * llingkaran;
       v := 4 * phi * jari * jari * jari / 3;
       writeln('Luas Permukaan Bola Adalah   : ', lp:0:2);
       writeln('Volume Bola Adalah           : ', v:0:2);
       end;

    7: begin
       writeln('Anda Memilih Bangun Ruang    : ', bangun_ruang[7].nama);
       write('Masukkan Luas Alas           : '); readln(lalas);
       write('Masukkan Jumlah Sisi Tegak   : '); readln(sisi_tegak);
       write('Masukkan Tinggi Limas        : '); readln(tinggi);
       lp := lalas + sisi_tegak;
       v := lalas * tinggi / 3;
       writeln('Luas Permukaan Limas Adalah  : ', lp:0:2);
       writeln('Volume Limas Adalah          : ', v:0:2);
       end;

    else writeln('Bangun Ruang Yang Anda Pilih Tidak Tersedia!'); //jika tidak memilih diantara 7 
    end; //akhir dari operasi kondisi

    writeln('Terima Kasih Telah Menggunakan Program Kami.');
    write('Ulangi? (Y/T) : '); readln(lagi);
    until (lagi<>'y') and (lagi<>'Y'); //akhir dari perulangan
end.
