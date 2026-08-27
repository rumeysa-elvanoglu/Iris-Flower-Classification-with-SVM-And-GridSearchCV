Bu proje, klasik Iris veri seti üzerinde Support Vector Machine (SVM) algoritması kullanılarak çiçek türlerinin sınıflandırılmasını amaçlamaktadır. Model performansını artırmak için GridSearchCV ile hiperparametre optimizasyonu yapılmıştır.
📊 Proje Hakkında
Iris veri seti, 3 farklı çiçek türüne (Setosa, Versicolor, Virginica) ait 150 örnek içerir. Her örnek için 4 özellik kullanılmıştır:
Sepal Length (Çanak Yaprak Uzunluğu)
Sepal Width (Çanak Yaprak Genişliği)
Petal Length (Taç Yaprak Uzunluğu)
Petal Width (Taç Yaprak Genişliği)
🛠️ Kullanılan Teknolojiler
Python 3
Pandas & NumPy
Matplotlib & Seaborn (veri görselleştirme)
Scikit-learn (modelleme ve değerlendirme)
🔍 Uygulanan Adımlar
Veri Keşfi (EDA): pairplot, scatterplot ve describe() ile veri setinin genel yapısı incelendi.
Ön İşleme:
Gereksiz Id sütunu kaldırıldı.
Species sütunu LabelEncoder ile sayısal değerlere dönüştürüldü.
Veri Bölme: Veri seti train_test_split ile eğitim (%75) ve test (%25) olarak ayrıldı.
Ölçeklendirme: Özellikler StandardScaler ile standartlaştırıldı.
Model Eğitimi: SVC modeli, GridSearchCV ile en iyi C, kernel ve gamma parametreleri bulunacak şekilde eğitildi.
Değerlendirme: Confusion matrix, accuracy score ve classification report ile model performansı ölçüldü.
📈 Sonuçlar
En iyi parametreler: {'C': 10, 'gamma': 'scale', 'kernel': 'rbf'}
Accuracy: 1.00 (test seti üzerinde %100 doğruluk)
🚀 Kurulum ve Çalıştırma
git clone https://github.com/kullanici-adi/iris-svm-classification.git
cd iris-svm-classification
pip install -r requirements.txt
jupyter notebook
📁 Veri Seti
Proje, herkese açık Iris veri seti kullanılarak hazırlanmıştır.
📝 Not
Bu proje eğitim amaçlı hazırlanmıştır ve makine öğrenmesi temel kavramlarını (veri ön işleme, model seçimi, hiperparametre optimizasyonu, model değerlendirme) uygulamalı olarak göstermeyi hedeflemektedir.
