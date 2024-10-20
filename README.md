**PROJE ÖZETİ**
Proje kapsamında kullanılan veri seti yüklenmiştir. Bu aşamada, verilerin kaynağından alınması ve işlenmesi sağlanmıştır. Veri seti, CSV formatında hazırlanmış olup, gerekli kütüphane yüklenmiştir.
Yüklenen veriler üzerinde gerekli ön işleme adımları uygulanmıştır. Eksik veriler, fillna yöntemi kullanılarak doldurulmuş; kategorik veriler, LabelEncoder ile sayısal verilere dönüştürülmüştür.
Veriler, modelin eğitimi ve test edilmesi için eğitim ve test setlerine ayrılmıştır. train_test_split fonksiyonu kullanılarak %80 eğitim ve %20 test oranları belirlenmiştir.
Keras kütüphanesi kullanılarak derin öğrenme modeli oluşturulmuştur. Model, katmanlar eklenerek derinleştirilmiş ve yapay sinir ağı mimarisi ile tanımlanmıştır.
Oluşturulan model, kayıp fonksiyonu ve optimizasyon yöntemi belirlenerek derlenmiştir. Bu aşamada, modelin performansını artırmak için adam optimizasyon algoritması kullanılmıştır. 
  'model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])'
Model, eğitim verileri üzerinde fit fonksiyonu ile eğitilmiştir. Eğitimin süresi ve batch boyutu belirlenmiştir.
Eğitilen model, test verileri üzerinde değerlendirilmiş ve doğruluk oranı hesaplanmıştır. Bu aşamada, evaluate fonksiyonu kullanılmıştır.
  'test_loss, test_accuracy = model.evaluate(X_test, y_test)  # Test sonuçları alınmıştır.'
Elde edilen sonuçlar analiz edilmiş ve modelin başarısı değerlendirilmiştir. Bu aşamada, grafiklerle sonuçlar görselleştirilmiş ve performans metrikleri yorumlanmıştır.

Her adımda kullanılan terimler:
Eğitim (Training): Modelin verilerle öğrenme süreci.
Test (Testing): Modelin öğrenilen bilgileri yeni verilere uygulama süreci.
Katman (Layer): Yapay sinir ağındaki bilgi işleme birimi.
Optimizasyon (Optimization): Modelin kayıp fonksiyonunu minimize etme süreci.
Aktivasyon Fonksiyonu (Activation Function): Katmanların çıktısını belirleyen matematiksel fonksiyonlar.

**Proje Linki:** https://www.kaggle.com/code/atahankarata/fish-classification
