def main():
    a=int(input("Kaç tane öğrenci verisi gireceksiniz? "))
    while not a==0:
        y=input("Öğrencinin okul numarasını girin=")
        x=input("Öğrencinin ismini giriniz=")
        v=int(input("Öğrencinin vize notunu giriniz="))
        f=int(input("Öğrencinin final notunu giriniz="))
        ö=int(input("Öğrencinin ödev notunu giriniz="))
        toplam=0.5*f+0.3*v+0.2*ö
        if toplam>=90:
            sonuc="Geçti, AA"
        elif 90>toplam>=85:
            sonuc="Geçti, BA"
        elif 85>toplam>=80:
            sonuc="Geçti, BB"
        elif 80>toplam>=75:
            sonuc="Geçti, CB"
        elif 75>toplam>=70:
            sonuc="Geçti, CB"
        elif 70>toplam>=65:
            sonuc="Geçti, CC"
        elif 65>toplam>=55:
            sonuc="Geçti, DC"
        elif toplam<55:
            sonuc="Kaldı, FF"
        a-=1
    save="""
    -------------------------------
    Öğrencinin adı soyadı=%s
    Öğrencinin numarası=%s
    Öğrencinin vize notu=%s
    Öğrencinin final notu=%s
    Öğrencinin ödev notu=%s
    Sonuç=%s
    """%(y,x,v,f,ö,toplam)
    with open("OgrenciNotListesi.txt", "a", encoding="utf-8") as ÖğrenciListesi:
        ÖğrenciListesi.write(save)
    if toplam > 55:
        with open("TumGecenOgrenciListesi.txt", "a", encoding="utf-8") as GeçenÖğrenciListesi:
            GeçenÖğrenciListesi.write(save)
    x = input("Çıkış yapmak için E'ye veri eklemek için Y'ye basınız.")
    if x == "E":
        pass
    if x == "Y":
        return main()
main()

   
