# Medical-Cost-Analysis
Bu Python kodu, sağlık sigortası masraflarını tahmin etmek için bir regresyon modeli oluşturmayı ve optimize etmeyi amaçlar. 
Veri Yükleme ve Görselleştirme:

İlk bölümde, sağlık sigortası veri seti yüklenir ve bazı temel veri görselleştirmeleri yapılır. seaborn ve matplotlib.pyplot kullanılarak BMI dağılımı, sigara içiciliği ile masraflar arasındaki ilişki, bölge ile sigara içiciliği arasındaki ilişki gibi çeşitli grafikler çizilir.
Veri Ön İşleme ve Özellik Mühendisliği:

sklearn kütüphanesinden LabelEncoder ve StandardScaler kullanılarak kategorik değişkenler işlenir ve bağımsız değişkenler (X) ile hedef değişken (y) ayrılır.
Veri, eğitim ve test kümelerine bölünerek ölçeklendirilir.
Çeşitli Regresyon Modellerini Eğitme:

Linear Regression, Decision Tree Regression, ve Random Forest Regression modelleri kullanılarak eğitim yapılır. Modellerin performansları, cross-validation kullanılarak değerlendirilir.
Grid Search ile Hiperparametre Optimizasyonu:

Random Forest Regression modeli için Grid Search yöntemi kullanılarak en iyi hiperparametreler bulunur. Bu adım, modelin performansını artırmak ve overfitting/underfitting durumlarını önlemek için önemlidir.

# Sağlık Sigortası Masrafı Tahmini

Bu proje, sağlık sigortası masraflarını tahmin etmek amacıyla çeşitli regresyon modellerini kullanmayı ve en iyi modeli seçmek için Grid Search yöntemini uygulamayı amaçlamaktadır.

## Veri Yükleme ve Görselleştirme

Proje, bir sağlık sigortası veri setini içermektedir. Veri seti, sağlık sigortası masraflarını etkileyebilecek çeşitli faktörleri içermektedir. Veri seti yüklenir ve bazı temel görselleştirmeler yapılır.

![Bmi Distribution](images/bmi_distribution.png)
*Bmi Distribution*

![Relationship between Smoker and Charges](images/smoker_vs_charges.png)
*Relationship between Smoker and Charges*

...

## Veri Ön İşleme ve Özellik Mühendisliği

Veri seti içeriğine uygun ön işleme adımları yapılır. Kategorik değişkenler işlenir, bağımsız ve bağımlı değişkenler ayrılır, veri ölçeklendirilir.

## Çeşitli Regresyon Modellerini Eğitme

Proje, çeşitli regresyon modellerini kullanarak sağlık sigortası masrafı tahmini yapmayı içermektedir. Eğitim sonuçları görselleştirilir ve modellerin performansı karşılaştırılır.

## Grid Search ile Hiperparametre Optimizasyonu

Random Forest Regression modeli için Grid Search yöntemi uygulanarak en iyi hiperparametreler bulunur. Bu adım, modelin performansını artırmak için önemlidir.

## Kullanım

1. Proje dosyalarını indirin.
2. Jupyter Notebook veya başka bir Python ortamında açın.
3. Proje dosyalarını çalıştırarak sonuçları inceleyin.

## Gereksinimler

Bu projeyi çalıştırmak için aşağıdaki Python kütüphanelerine ihtiyaç vardır:

- pandas
- numpy
- seaborn
- matplotlib
- sklearn

Gereksinimleri yüklemek için terminal veya komut istemcisine şu komutu yazabilirsiniz:


Bu, projenin başlangıç düzeyinde bir README dosyasıdır. İhtiyaca göre daha fazla bölüm ve açıklama ekleyebilirsiniz.

## Proje Yapısı
data/ Klasörü:
insurance.csv: Sağlık sigortası veri seti. İlgili özellikleri içeren bir CSV dosyası.
images/ Klasörü:
bmi_distribution.png: BMI dağılımını gösteren bir histogram grafiği.
smoker_vs_charges.png: Sigara içiciliği ile masraflar arasındaki ilişkiyi gösteren bir kutu grafiği.
...
models/ Klasörü:
random_forest_model.pkl: Random Forest modelinin kaydedilmiş versiyonu.
Ana Dizin:
README.md: Proje hakkında genel bilgilerin ve kullanım talimatlarının bulunduğu Markdown dosyası.
requirements.txt: Projenin çalışması için gereken Python paketlerini içeren dosya.
main.ipynb: Jupyter Notebook formatında yazılmış ana çalıştırılabilir dosya. Projenin temelini oluşturur ve adım adım açıklamalar içerir.
helper_functions.py: Yardımcı işlevleri içeren Python betiği. Projenin temiz ve düzenli olmasına yardımcı olur.
LICENSE: Projenin lisans bilgilerini içeren dosya.
.gitignore: Git tarafından izlenmemesi gereken dosya ve klasörleri belirten dosya.

## Sonuçlar ve Değerlendirme

Projede kullanılan modellerin performansı ve Grid Search sonuçları değerlendirilir. En iyi model seçimi ve projenin genel değerlendirmesi yapılır.
