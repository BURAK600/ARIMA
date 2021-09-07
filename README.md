# ARIMA (AutoRegressive Integrated Moving Average)
Arima tahmin yapmak veya verileri daha iyi anlamak için zaman serisi verilerine uygulanır. -------------------> Timeseries forecasting

Arima algoritması temel olarak 3 bileşenden oluşur ve her bir bileşen için 0,1 veya 2 değerini atayarak oluşturduğu model üzerinden katsayılar hesaplayıp tahminleme yapmaktadır. Buradaki katsayılar AR – I – MA şeklinde belirlenip ARIMA(0, 1, 0) şeklinde ifade ediliyor. Bunun yanı sıra incelenen zaman serisi sezonsallık içeriyorsa modelin yanına bir de sezonsal bölümün analizi çıkar. ARIMA(0, 1, 1)(0, 1, 0)[12] gibi bir model bize 12 aylık sezonlara ait bir zaman serisini incelediğimiz bilgisini verir.

Durağanlık (Stationality)
ARIMA modelleri sadece durağan verilerde uygulanabilir. Bu, zaman içinde bir eğilime sahip olmak istemediğimiz anlamına gelir. Zaman serisinin bir trendi varsa, o zaman durağan değildir ve onu durağan hale getirmek için fark almamız gerekir

Serinin durağan olup olmadığına karar vermemize yardımcı olması için Augmented Dickey-Fuller(ADF) testi kullanılabilir.


