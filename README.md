# SMS Spam Classification

Bu proje, SMS veya e-posta mesajlarını **Spam** ya da **Spam Değil** olarak sınıflandıran bir **Streamlit web uygulamasıdır**. Bu sınıflandırma, eğitilmiş bir makine öğrenimi modeli kullanılarak gerçekleştirilir.

## Özellikler

- Kullanıcıdan girilen metin mesajını (SMS veya e-posta) kabul eder.
- Metni ön işler (tokenizasyon, stopword çıkarma, kök bulma).
- Eğitilmiş bir modeli kullanarak mesajın Spam olup olmadığını tahmin eder.
- **Streamlit** aracılığıyla kullanıcı dostu bir arayüz sunar.

## Nasıl Çalışır?

1. **Ön İşleme**: 
   - Metin küçük harfe dönüştürülür.
   - Metin tokenlere ayrılır.
   - Stopword'ler ve noktalama işaretleri çıkarılır.
   - Kalan kelimeler köklerine indirilir.
   
2. **Vektörizasyon**:
   - **TF-IDF (Term Frequency-Inverse Document Frequency)** vektörizasyonu kullanılarak metin sayısal bir formata dönüştürülür.

3. **Tahmin**:
   - Ön işleme tabi tutulmuş ve vektörleştirilmiş giriş, bir makine öğrenimi modeline (Logistic Regression veya başka bir sınıflandırıcı) aktarılır.
   - Model, mesajın spam olup olmadığını tahmin eder.

## Kurulum

Projeyi yerel ortamda çalıştırmak için aşağıdaki adımları izleyin:

### Depoyu Klonlayın:

```bash
git clone https://github.com/your-username/sms-spam-classification.git
cd sms-spam-classification
