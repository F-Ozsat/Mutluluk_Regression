# Dünya Mutluluk Raporu 2019 - Regresyon Analizi

Bu projede 2019 Dünya Mutluluk Raporu verisi kullanılarak mutluluk skorunu etkileyen faktörler incelenmiştir. Çalışmada **Lineer Regresyon** ve **Polinomsal Regresyon (2. ve 3. derece)** modelleri karşılaştırılmıştır.

## 🔎 Kullanılan Veri Seti
- **2019 Dünya Mutluluk Verisi**
- Kolonlar: GDP per capita, Social support, Healthy life expectancy, Freedom to make life choices, Generosity, vb.

## 📊 Proje Adımları
1. Veri setinin yüklenmesi ve incelenmesi
2. Korelasyon analizi ve görselleştirme
3. Eğitim ve test verilerinin hazırlanması
4. Lineer Regresyon ve Polinomsal Regresyon modellerinin eğitilmesi
5. Model performanslarının R², MSE ve MAE ile karşılaştırılması
6. Sonuçların görselleştirilmesi

## 📈 Sonuçlar
- En iyi sonuç **2. Derece Polinomsal Regresyon** modelinde elde edilmiştir.
- Ancak R², MSE ve MAE değerleri mükemmel seviyede değildir, bu sebeple farklı algoritmalarla (Random Forest, Gradient Boosting) çalışılabilir.

| Model                     | R² Skoru | MSE   | MAE   |
|----------------------------|----------|-------|-------|
| 2. Derece Polinomsal Model | 0.6551588159503554      | 0.3588842809031423   | 0.44647699837668686   |
| 3. Derece Polinomsal Model | 0.3436397549522613      | 0.6830894494419099   | 0.592618896484375   |
| Lineer Model               | 0.6056836483464102      | 0.4103742443106109   | 0.4958602742165801   |

*(Değerler notebook çıktısından alınabilir.)*

## 🛠️ Kullanılan Teknolojiler
- Python (NumPy, Pandas, Scikit-learn, Matplotlib, Seaborn)
- Jupyter Notebook

## 🚀 Nasıl Çalıştırılır?
```bash
# Gerekli kütüphaneleri yükle
pip install -r requirements.txt

# Notebook'u çalıştır
jupyter notebook main.ipynb
