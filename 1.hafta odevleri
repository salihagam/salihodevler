# salihodevler
#1. HAFTA ÖDEVLER

#1-Input ile kullanıcıdan bir kelime yazmasını isteyip, bu kelimeyi altı çizili ve etrafı desenli bir şekilde printleyin.

a=input("Sizce bu gunun sozu nedir?")
print("X"*(len(a)+12))
print("X",(len(a)+8)*" ","X")
print("X",(len(a)+8)*" ","X")
print("X",(len(a)+8)*" ","X")
print("X",(len(a)+8)*" ","X")
print("X",3*" ",a,3*" ","X")
print("X",3*" ",len(a)*"_",3*" ","X")
print("X",(len(a)+8)*" ","X")
print("X",(len(a)+8)*" ","X")
print("X",(len(a)+8)*" ","X")
print("X",(len(a)+8)*" ","X")
print("X"*(len(a)+12))


#2-Kullanıcıdan input ile km cinsinden mesafe bilgisi alıp, bu bilgiyi mile dönüştürün ve sonucu ekrana printleyin.


x=input("Haftalik ortalama kac KM yol yaiyorsunuz?")
#Bir Kara Mili 1.609,344 metre ye eşittir.  1 mil = 1,61 km'dir. 
#Bir Deniz Mili 1.852,2 metre ye eşittir.  1 mil = 1,85 km'dir.
y=int(x)*(1/1.61)
z=int(x)*(1/1.85)
print("Amerikada olsaydiniz",int(y), "kara mili", "Denizde olsaniz",int(z), "deniz mili yapmis olacaktiniz")


#3-Oğrenci not ortalama programi

#Icerik:Kullanicidan input ile ad-soyad, vize, final ve ders takip bilgilerini alip bu degerleri yuzdelik oranlarina 
#gore hesaplayin ve yil sonu notunu cikarin.

#Yontem:-Sinav puanlari ve ders takip puani 0-100 arasidir.
#-Bir öğrencinin gitmesi gereken toplam ders sayısı 20’dir. Kaçırılan her ders için 5 puan kırılacaktır. 
#(Orn: 3 ders kaciran bir ogrencinin ders takip puani: 100-(3x5)=85 )
#Oranlar :
#- Vize Notu ( 30%)
#- Final Notu (50%)
#- Ders takip (20%)

#Sonuc:
#    0.    Output olarak ogrencinin yil sonu puanini ekrana pritleyin.
#    0.    Ogrenci ad-soyad, vize-final-ders takip bilgilerini ve hesapladiginiz yil sonu puanini 
#    “ogrenciNotHesaplama” isimli bir dosyaya kaydedin.

a=input("Adiniz ve Soyadiniz:")
print("""
- Sinav puanlari ve ders takip puani 0-100 arasidir.
- Bir öğrencinin gitmesi gereken toplam ders sayısı 20’dir.
""")
v=input("Vize notunuz:")
#v<0<101 bunu nasil saglayacagiz?
f=input ("Final notunuz:")
#f<0<101
t=input("kacirdiginiz ders sayisi:")
#t<0<20
dtp=100-int(t)*5
ysn=dtp+int(v)*(30/100)+int(f)*(50/100)
print("SAYIN", a, "YIL SONU PUANINIZ:",ysn, "dir.")
dosya=open("Ogrenci_Not_Hesaplama.txt", "w")
print('Sayin',a,"Vize notunuz:",v, "Final notunuz:",f,"kacirdiginiz ders sayisi:",t,"YIL SONU PUANINIZ:",ysn, file=dosya)
dosya.close()


#4-Faiz hesaplama programi
#Icerik:Kullanicidan gerekli bilgileri alip faiz tutarini hesaplayin.

#Yontem:Bu programi calistirabilmeniz icin asagida belirtilen bilgileri input yardimi ile kullanicidan almaniz gerekmektedir.
#    ⁃    Ana para
#   ⁃    Faiz suresi (yil)
#   ⁃    Faiz orani

#Faiz hesaplama formulu:
#Ana para x faiz suresi x faiz orani / 100

#Sonuc:Gerekli islemleri yaptiktan sonra output olarak toplam faiz tutarini, aylik ve gunluk ortalama faiz tutarini, 
#toplam para miktarini (faiz+ana para);
# 1) print ile ekrana yazin,
# 2) ”faizHesaplama” isimli bir dosyaya
#     kaydedin.

a=int(input("Anaparayi TL olarak giriniz: "))
s=int(input("Faiz suresini YIL olarak giriniz: ",))
o=float(input("Yillik faiz orani: "))

Faiz=(a*s*o)/100

print("Toplam faiz tutari:", Faiz, "\nAylik ortalama faiz tutari:", float(Faiz/(s*12)),
      "\nGunluk ortalama faiz tutari:", float(Faiz/(s*365)), "\nToplam para miktari:", a + Faiz)

dosya=open("faizHesaplama.txt", "w")
print("Toplam faiz tutari:", Faiz, "\nAylik ortalama faiz tutari:", float(Faiz/(s*12)),
      "\nGunluk ortalama faiz tutari:", float(Faiz/(s*365)), "\nToplam para miktari:", a + Faiz, file=dosya)
dosya.close()


#5-Aylik masraf programi

#Icerik:Aylık giderleri ve bu giderlerin aylik gelire oranini hesaplayan bir program yapmanız istenmektedir.

#Yontem:Asagida belirtilen harcama kalemlerini ve aylik geliri kullanicidan input ile alip gerekli hesaplamalari yapin

#Harcama kalemleri:
#-mutfak,
#-egitim,
#-giyim,
#-ulasim.

#Sonuc:
#1-Kullanicinin aylik toplam masrafini ve bu masrafin aylik gelirine oranini ekrana printleyin.
#2- Ayni sonucu “aylikmasraf” isimli bir dosyaya kaydedin.

a=input("Aylik toplam gelirinizi TL olarak giriniz: ")
b=input("Aylik mutfak masrafinizi Tl olarak gíriniz: ")
c=input("Aylik egitim masrafinizi Tl olarak gíriniz: ")
d=input("Aylik giyim masrafinizi Tl olarak gíriniz: ")
e=input("Aylik ulasim masrafinizi Tl olarak gíriniz: ")
#x=toplam gider
x=int(b)+int(c)+int(d)+int(e)
o=(x/int(a)*100)
print("Aylik toplam masrafiniz:",x,"TL","Aylik masrafinizin aylik gelirinize orani:%",o)
dosya=open("aylik_masraf.txt", "w")
print("Aylik toplam masrafiniz:",x,"TL","Aylik masrafinizin aylik gelirinize orani:%",o, file=dosya)
dosya.close()

#6-Asagidaki ciktiyi 3 farkli yontem ile printleyin.

Python’un kurucusu Guido Van Rossum, Hollanda’nin Amsterdam’daki  "Universiteit Van Amsterdam" okulundan  1982’de mezun olmuştur.


print("""\nPython’un kurucusu Guido Van Rossum, Hollanda’nin Amsterdam’daki  "Universiteit Van Amsterdam" okulundan  1982’de mezun olmuştur.\n""")


print('\nPython’un kurucusu Guido Van Rossum, Hollanda’nin Amsterdam’daki  "Universiteit Van Amsterdam" okulundan  1982’de mezun olmuştur.\n')


print("\nPython’un kurucusu Guido Van Rossum, Hollanda’nin Amsterdam’daki \"Universiteit Van Amsterdam\" okulundan  1982’de mezun olmuştur.\n")
