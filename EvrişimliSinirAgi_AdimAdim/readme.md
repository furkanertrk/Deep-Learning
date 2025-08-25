Proje Adı: Evrişimsel Sinir Ağları (CNN) - Adım Adım Uygulama
Proje Hakkında
Bu depo, bir yapay sinir ağı mimarisi olan Evrişimsel Sinir Ağları (CNN)'nin temel bileşenlerini Python ve NumPy kütüphanesi kullanarak uygulamalı olarak ele almaktadır. Proje, Dr. Merve Ayyuce Kizrak'ın Udemy'deki "Deep Learning A-Z™| Python ile Derin Öğrenme" kursu kapsamında geliştirilmiştir.

Uygulamada, CNN'in temel yapı taşları olan ileri yayılım (forward propagation) ve geri yayılım (backward propagation) işlemleri adım adım incelenmiştir. Özellikle, aşağıdaki temel fonksiyonlar sıfırdan kodlanmıştır:

##Sıfır Dolgulama (Zero Padding): Girdinin kenarlarına sıfır ekleyerek evrişim işlemi sonrası boyut kaybını önleme.
##Evrişimsel Adım (Conv Single Step): Evrişim filtresinin tek bir pencere üzerindeki işlemini gerçekleştirme.
##Evrişimsel İleri Yayılım (Conv Forward): Giriş verisi üzerinde tüm evrişim işlemini gerçekleştirerek çıktı (Z) matrisini oluşturma.
##Havuzlama (Pooling): Girişin boyutunu küçültme ve önemli özellikleri vurgulama (Max Pooling ve Average Pooling).
##Geriye Yayılım (Backward Propagation): Evrişim ve havuzlama katmanlarında geriye yayılım işlemini hesaplayarak gradyanları bulma.

Bu uygulama, derin öğrenme kütüphanelerinin (TensorFlow, PyTorch vb.) perde arkasında çalışan mekanikleri anlamak için ideal bir başlangıç noktasıdır.

#Kullanılan Teknolojiler
-Python
-NumPy
-Matplotlib
-h5py
-scipy

###Kurulum
Bu depoyu bilgisayarınıza klonlayın:
git clone https://github.com/KullaniciAdiniz/ProjeAdi.git

###Gerekli kütüphaneleri yükleyin:
pip install numpy matplotlib h5py scipy

Proje dosyasını (EvrişimliSinirAgi_AdimAdim.ipynb) çalıştırmak için Jupyter Notebook veya Google Colab kullanın.

Nasıl Kullanılır?
EvrişimliSinirAgi_AdimAdim.ipynb dosyasını açarak, her bir kod bloğunu sırayla çalıştırın.
