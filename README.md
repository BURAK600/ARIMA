# ARIMA (AutoRegressive Integrated Moving Average)
Arima tahmin yapmak veya verileri daha iyi anlamak için zaman serisi verilerine uygulanır. -------------------> Timeseries forecasting


Arima algoritması temel olarak 3 bileşenden oluşur ve her bir bileşen için 0,1 veya 2 değerini atayarak oluşturduğu model üzerinden katsayılar hesaplayıp tahminleme yapmaktadır. Buradaki katsayılar AR – I – MA şeklinde belirlenip ARIMA(0, 1, 0) şeklinde ifade edilir. Bunun yanı sıra incelenen zaman serisi sezonsallık içeriyorsa modelin yanına bir de sezonsal bölümün analizi çıkar. ARIMA(0, 1, 1)(0, 1, 0)[12] gibi bir model bize 12 aylık sezonlara ait bir zaman serisini incelediğimiz bilgisini verir.


AutoRegressive (AR) modeli -------------> 

Bağımlı değişkenin önceki değerlerinin lineer kombinasyonunu kullanarak bağımlı değişkenin tahmini. Yani bağımlı değişkeninin kendisini kullanarak regresyon yapılır, “otoregresif” ifadesi de buradan geliyor. Bir AR(p) modeli aşağıdaki gibidir:( “p” ifadesi, bu modelde kaç gecikmeye kadar geri gidileceğini gösterir.) Yani AR(2) dediğimizde, 2 gecikmeye kadar giderek bağımsız değişkenin bu gecikmelerdeki değerlerini oto-regresyon modelinde kullanıyoruz.
(Burada gecikme değerlerinin yani bir diğer ifadeyle tahminci değişkenlerin katsayılarının 0 olduğunu düşünelim. Bu durumda oto-regresyon denkleminde sadece c sabiti ve epsilon kalacaktır. Bu da aslında bizim için beyaz gürültü(white noise) serisini temsil eden denklem demektir.)

x'in t zamanındaki değeri, sabit terim C ile x'in bir önceki değerinin sabit beta sayısı ile hata teriminin toplamına eşitleyen değeri 
Xt = C + β* Xt-1 + 

Integrated (I)  değeri durağan olmayan verileri durağana çevirirken alınan farkın değerini alır.

Moving Average (MA): 
Tahminlemeye çalıştığımız değişkenin geçmiş değerlerini tahminciler olarak kullanmak yerine, geçmiş tahmin hatalarını modelde tahminciler olarak kullanıyoruz. 



Durağanlık (Stationality)
ARIMA modelleri sadece durağan verilerde uygulanabilir. Bu, zaman içinde bir eğilime sahip olmak istemediğimiz anlamına gelir. Zaman serisinin bir trendi varsa, o zaman durağan değildir ve onu durağan hale getirmek için fark almamız gerekir. Verinin “durağan” olması demek, o serinin özelliklerinin zamandan etkilenmemesi, ondan bağımsız olması demektir.




Serinin durağan olup olmadığına karar vermemize yardımcı olması için Augmented Dickey-Fuller(ADF) testi kullanılır.

ACF(Autocorrelation) ve PACF(Partial Autocorrelation Plots) grafikleri  p, q, P, Q parametrelerinin tahmin edilmesinde yardımcı olur.


-897+













