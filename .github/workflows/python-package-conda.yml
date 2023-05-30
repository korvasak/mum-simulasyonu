import time
import random

def mum_simulasyonu():
    # Rastgele mum bitiş süresini belirleme
    bitis_suresi = random.randint(30, 180)  # 30 dakika ile 3 saat arası
    
    # Mum bitene kadar çalışma döngüsü
    while bitis_suresi > 0:
        # Mumun kalan süresini hesaplama
        saatler = bitis_suresi // 60
        dakikalar = bitis_suresi % 60
        
        # Kullanıcıya kalan süreyi gösterme
        print(f"Mum bitene kadar kalan süre: {saatler} saat {dakikalar} dakika")
        
        # 1 dakika bekletme
        time.sleep(60)
        
        # Mum bitiş süresini azaltma
        bitis_suresi -= 1
        
    # Mum bittiğinde çalışma tamamlandı mesajı
    print("Mum tamamen bitti. Ders çalışma veya kitap okuma tamamlandı.")

# Mum simülasyonunu başlatma
mum_simulasyonu()
