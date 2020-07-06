# Baturaja1337
import datetime
import os
import time
from random import choice

from pyfiglet import Figlet

cutom = Figlet(font='graffiti')

AreaCode = {
    # -> Daerah Jawa (DKI Jakarta,Banten,Jawa Barat)
    'A': ['Serang', 'Pandeglang', 'Cilegon', 'Lebak', 'Tangerang'],
    'B': ['DKI Jakarta', 'Bekasi', 'Tangerang', 'Depok'],
    'D': ['Bandung', 'Cimahi', 'Bandung Barat'],
    'E': ['Indramayu', 'Majalengka', 'Kuningan', 'Cirebon'],
    'F': ['Bogor', 'Cianjur', 'Sukabumi'],
    'T': ['Karawang', 'Subang', 'Purwakarta'],
    'Z': ['Garut', 'Tasikmalaya', 'Sumedang', 'Ciamis', 'Banjar'],

    # -> Jawa Tengah & DI Yogyakarta
    'G': ['Pekalongan', 'Tegal', 'Brebes', 'Batang', 'Pemalang', 'Siawi'],
    'H': ['Semarang', 'Salatiga', 'Kendal', 'Demak'],
    'K': ['Pati', 'Kudus', 'Jepara', 'Rembang', 'Blora', 'Grobogan', 'Cepu'],
    'R': ['Banyumas', 'Cilacap', 'Purbalingga', 'Banjarnegara'],
    'AA': ['Magelang', 'Purworejo', 'Kebumen', 'Temanggung', 'Wonosobo'],
    'AB': ['Yogyakarta', 'Bantul', 'Kidul', 'Sleman', 'Kulon Progo'],
    'AD': ['Sragen', 'Karang Anyar', 'Wonogiri', 'Klaten', 'Surakarta', 'Sukoharjo', 'Boyolali'],

    # -> Jawa Timur
    'L': ['Surabaya'],
    'M': ['Madura', 'Pamekasan', 'Sumenep', 'Sampang', 'Bangkalan'],
    'N': ['Malang', 'Probolinggo', 'Pasuruan', 'Lumajang', 'Batu'],
    'P': ['Bondowoso', 'Situbondo', 'Jember', 'Banyuwangi'],
    'S': ['Bojonegoro', 'Mojokerto', 'Tuban', 'Lamongan', 'Jombang'],
    'W': ['Sidoarjo', 'Gresik'],
    'AE': ['Madiun', 'Ngawi', 'Magetan', 'Ponorogo', 'Pacitan'],
    'AG': ['Kediri', 'Blitar', 'Tulung Agung', 'Nganjuk', 'Trenggalek'],

    # -> Bali & Nusa Tenggara
    'DK': ['Bali'],
    'DR': ['Lombok', 'Mataram'],
    'EA': ['Sumbawa', 'Sumbawa Barat', 'Dompu', 'Bima'],
    'DH': ['NTT', 'Kupang', 'Rote Ndao'],
    'EB': ['Flores', 'Manggarai', 'Ngada', 'Ende', 'Sikka', 'Flores Timur', 'Lemata', 'Alor'],
    'ED': ['Sumba', 'Sumba Barat', 'Sumba Timur'],

    # -> Kalimantan
    'KB': ['Kalimantan Barat'],
    'DA': ['Kalimantan Selatan'],
    'KH': ['Kalimantan Tengah'],
    'KT': ['Kalimantan Timur'],
    'KU': ['Kalimantan Utara'],

    # -> Sulawesi
    'DB': ['Manado', 'Tomohon', 'Bitung', 'Bolang Mongondow', 'Minahasa', 'Minahasa Utara', 'Minahasa Selatan'],
    'DL': ['Sulawesi Utara', 'Talaud', 'Sitaro'],
    'DM': ['Gorontalo'],
    'DN': ['Sulawesi Tengah'],
    'DT': ['Sulawesi Tenggara'],
    'DD': ['Sulawesi Utara'],
    'DC': ['Sulawesi Barat'],

    # -> Maluku & Papua
    'DE': ['Maluku'],
    'DG': ['Maluku Utara'],
    'PA': ['Papua'],
    'PB': ['Papua Barat'],

    # -> Sumatera
    'BL': ['Nanggroe Aceh Darusalam'],
    'BB': ['Sumatera Utara'],
    'BK': ['Sumatera B'],
    'BA': ['Sumatera Barat'],
    'BM': ['Riau'],
    'BH': ['Jambi'],
    'BD': ['Bengkulu'],
    'BP': ['Kepulauan Riau'],
    'BG': ['Sumatera Selatan'],
    'BE': ['Lampung']
}


def cek():
    jam = datetime.datetime.now()
    global tmp2
    os.system('cls')
    print('-' * 50)
    print('\t\t\t{ Baturaja1337 }\n', cutom.renderText("Zearch"))
    print('-' * 50)

    tmp1 = []
    area = input('~> Enter Area Code\n~> Ex : BG \nCoder@Baturaja1337 >>> ').upper()
    if len(area) > 2 or len(area) == " " or area not in AreaCode:
        print('Code Area is Wrong or not valid !')
        time.sleep(2)
        os.system('cls')
        return cek()
    elif area in AreaCode:
        for x in AreaCode[area]:
            tmp1.append(x)
    else:
        os.system('cls')
        return cek()

    try:
        tmp2 = []
        Plat = int(input('\n~> Enter Number Plat\n~> Ex : 9999 \nCoder@Baturaja1337 >>> '))
        if Plat <= 1 or Plat <= 1999:
            tmp2.append('Kendaraan Penumpang')
            tmp2.append('Kendaraan Pribadi')
        elif Plat <= 2000 or Plat <= 6999:
            tmp2.append('Sepeda Motor')
        elif Plat <= 7000 or Plat <= 7999:
            tmp2.append('Kendaraan Bus')
        elif Plat <= 8000 or Plat <= 9999:
            tmp2.append('Kendaraan Beban')
            tmp2.append('Kendaraan Besar')
            tmp2.append('Kendaraan Muatan')
        else:
            pass
    except KeyboardInterrupt:
        print('Good Bye....')

    y = (choice(tmp2))
    x = (choice(tmp1))
    print()

    print('+', '-' * 60, '+')
    print("|    TIME\t\t|     AREA\t\t   |    Tipe\t\t|")
    print('+', '-' * 60, '+')
    print('|', jam.strftime("%d"), jam.strftime("%m"), jam.strftime("%y"), '\t\t|', x, '\t|', y, '\t|')
    print('+', '-' * 60, '+')
    print()

    print("""1. Start Program\n2. Exit Program""")

    try:
        ulang = int(input('>>>'))
        if ulang == 1:
            cek()
        elif ulang == 2:
            print("See you next time...\nBye...")
            time.sleep(3)
            os.system('cls')
            os.system('exit')
        else:
            print("Tidak ada :(")
    except KeyboardInterrupt:
        print('See you Brother...')
        os.system('exit')


if "__name__" == cek():
    run()
