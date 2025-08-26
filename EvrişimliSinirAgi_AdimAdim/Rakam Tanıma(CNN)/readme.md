# MNIST Rakam Tanıma (El Yazısı Rakam Tanıma)

Bu proje, bir evrişimli sinir ağı (Convolutional Neural Network - CNN) kullanarak el yazısıyla yazılmış rakamları tanımayı amaçlayan temel bir derin öğrenme uygulamasıdır. Proje, popüler **MNIST veri kümesi** üzerinde eğitilmiştir.

## Proje Amacı

Bu projenin temel amacı, bir derin öğrenme modelinin görüntü sınıflandırma görevini nasıl gerçekleştirdiğini göstermektir. Proje kapsamında kullanılan evrişimli sinir ağları, görüntü verilerindeki örüntüleri (patterns) ve özellikleri (features) öğrenerek rakamları yüksek doğrulukla sınıflandırabilir.

## Veri Kümesi

Projede, makine öğrenmesi ve derin öğrenme alanında en sık kullanılan veri kümelerinden biri olan **MNIST** (Modified National Institute of Standards and Technology) veri kümesi kullanılmıştır. Bu veri kümesi, 0'dan 9'a kadar olan el yazısı rakamlarından oluşan 60.000 eğitim görüntüsü ve 10.000 test görüntüsü içerir. Her bir görüntü, 28x28 piksel boyutunda ve gri tonlamalıdır.

## Kullanılan Teknolojiler

  * **Python**: Projenin ana programlama dilidir.
  * **TensorFlow**: Yüksek performanslı sayısal hesaplamalar ve büyük ölçekli makine öğrenmesi için kullanılan açık kaynaklı bir kütüphanedir.
  * **Keras**: TensorFlow üzerinde çalışan ve derin öğrenme modellerinin oluşturulmasını ve eğitilmesini kolaylaştıran üst düzey bir API'dir.
  * **Jupyter Notebook**: Kodun etkileşimli olarak geliştirilmesi ve belgelerin oluşturulması için kullanılmıştır.

## Model Mimarisi

Bu projede kullanılan CNN modeli, aşağıdaki katmanlardan oluşmaktadır:

  * **Evrişim Katmanları (`Conv2D`)**: Görüntülerdeki farklı özellikleri çıkarmak için kullanılır. Bu katmanlarda, 3x3 boyutunda filtreler (kernels) kullanılarak görüntüler taranır.
  * **Maksimum Havuzlama Katmanı (`MaxPooling2D`)**: Görüntü boyutunu küçülterek hesaplama maliyetini düşürür ve en önemli özellikleri korur.
  * **Düzleştirme Katmanı (`Flatten`)**: Matris formatındaki veriyi, tam bağlantılı katmana beslemek için tek bir vektöre dönüştürür.
  * **Tam Bağlantılı Katmanlar (`Dense`)**: Görüntünün sınıflandırılması için kullanılır.
  * **Çıkış Katmanı (`Dense`)**: Son katmandır ve 0-9 arasındaki rakamlar için 10 farklı olasılık değeri üretir.
  * **Bırakma Katmanı (`Dropout`)**: Modelin aşırı öğrenmesini (overfitting) önlemek için kullanılır.

## Nasıl Çalıştırılır?

Projeyi kendi ortamınızda çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

1.  Gerekli kütüphaneleri yükleyin:
    ```bash
    pip install tensorflow keras matplotlib
    ```
2.  Jupyter Notebook veya Google Colab gibi bir ortamda `Rakam_Tanıma.ipynb` dosyasını açın.
3.  Dosyadaki hücreleri sırasıyla çalıştırarak veri kümesini yükleyebilir, modeli eğitebilir ve test sonuçlarını gözlemleyebilirsiniz.

## Sonuçlar

Eğitilen model, test veri kümesi üzerinde %79.20 doğruluk oranı elde etmiştir. Modelin performansı, `model.evaluate()` fonksiyonuyla hesaplanan doğruluk (`accuracy`) ve kayıp (`loss`) değerleriyle gözlemlenebilir.

-----