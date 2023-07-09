# Comparing `tmp/evds-0.2.0.tar.gz` & `tmp/evds-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/evds-0.2.0.tar", last modified: Mon May 25 21:06:26 2020, max compression
+gzip compressed data, was "evds-0.3.0.tar", last modified: Sun Jul  9 13:09:06 2023, max compression
```

## Comparing `evds-0.2.0.tar` & `evds-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 fthpi     (1000) fthpi     (1000)        0 2020-05-25 21:06:26.211354 evds-0.2.0/
--rw-r--r--   0 fthpi     (1000) fthpi     (1000)    10186 2020-05-25 21:06:26.211354 evds-0.2.0/PKG-INFO
--rw-r--r--   0 fthpi     (1000) fthpi     (1000)     8322 2020-05-25 21:00:47.000000 evds-0.2.0/README.md
-drwxr-xr-x   0 fthpi     (1000) fthpi     (1000)        0 2020-05-25 21:06:26.211354 evds-0.2.0/evds/
--rw-r--r--   0 fthpi     (1000) fthpi     (1000)     8812 2020-05-25 21:02:37.000000 evds-0.2.0/evds/__init__.py
-drwxr-xr-x   0 fthpi     (1000) fthpi     (1000)        0 2020-05-25 21:06:26.211354 evds-0.2.0/evds.egg-info/
--rw-r--r--   0 fthpi     (1000) fthpi     (1000)    10186 2020-05-25 21:06:26.000000 evds-0.2.0/evds.egg-info/PKG-INFO
--rw-r--r--   0 fthpi     (1000) fthpi     (1000)      174 2020-05-25 21:06:26.000000 evds-0.2.0/evds.egg-info/SOURCES.txt
--rw-r--r--   0 fthpi     (1000) fthpi     (1000)        1 2020-05-25 21:06:26.000000 evds-0.2.0/evds.egg-info/dependency_links.txt
--rw-r--r--   0 fthpi     (1000) fthpi     (1000)       16 2020-05-25 21:06:26.000000 evds-0.2.0/evds.egg-info/requires.txt
--rw-r--r--   0 fthpi     (1000) fthpi     (1000)        5 2020-05-25 21:06:26.000000 evds-0.2.0/evds.egg-info/top_level.txt
--rw-r--r--   0 fthpi     (1000) fthpi     (1000)       38 2020-05-25 21:06:26.211354 evds-0.2.0/setup.cfg
--rw-r--r--   0 fthpi     (1000) fthpi     (1000)      698 2020-05-25 20:07:16.000000 evds-0.2.0/setup.py
+drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2023-07-09 13:09:06.640123 evds-0.3.0/
+-rw-r--r--   0 ege       (1000) ege       (1000)     1071 2023-07-09 11:31:39.000000 evds-0.3.0/LICENCE
+-rw-r--r--   0 ege       (1000) ege       (1000)    10762 2023-07-09 13:09:06.640123 evds-0.3.0/PKG-INFO
+-rw-r--r--   0 ege       (1000) ege       (1000)    10356 2023-07-09 13:02:24.000000 evds-0.3.0/README.md
+drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2023-07-09 13:09:06.640123 evds-0.3.0/evds/
+-rw-r--r--   0 ege       (1000) ege       (1000)    10195 2023-07-09 13:02:24.000000 evds-0.3.0/evds/__init__.py
+drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2023-07-09 13:09:06.640123 evds-0.3.0/evds.egg-info/
+-rw-r--r--   0 ege       (1000) ege       (1000)    10762 2023-07-09 13:09:06.000000 evds-0.3.0/evds.egg-info/PKG-INFO
+-rw-r--r--   0 ege       (1000) ege       (1000)      182 2023-07-09 13:09:06.000000 evds-0.3.0/evds.egg-info/SOURCES.txt
+-rw-r--r--   0 ege       (1000) ege       (1000)        1 2023-07-09 13:09:06.000000 evds-0.3.0/evds.egg-info/dependency_links.txt
+-rw-r--r--   0 ege       (1000) ege       (1000)       24 2023-07-09 13:09:06.000000 evds-0.3.0/evds.egg-info/requires.txt
+-rw-r--r--   0 ege       (1000) ege       (1000)        5 2023-07-09 13:09:06.000000 evds-0.3.0/evds.egg-info/top_level.txt
+-rw-r--r--   0 ege       (1000) ege       (1000)       38 2023-07-09 13:09:06.640123 evds-0.3.0/setup.cfg
+-rw-r--r--   0 ege       (1000) ege       (1000)      709 2023-07-09 13:02:24.000000 evds-0.3.0/setup.py
```

### Comparing `evds-0.2.0/PKG-INFO` & `evds-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,194 +1,245 @@
-Metadata-Version: 2.1
-Name: evds
-Version: 0.2.0
-Summary: EVDS python wrapper
-Home-page: https://github.com/fatihmete/evds
-Author: Fatih Mete
-Author-email: fatihmete@live.com
-License: UNKNOWN
-Description: # EVDS
-        
-        [English](https://github.com/fatihmete/evds/blob/master/README_EN.md)
-        
-        EVDS paketi EVDS-API üzerinden Türkiye Cumhuriyet Merkez Bankası (TCMB) tarafından Elektronik Veri Dağıtım Sistemi (EVDS) aracılığıyla yayımlanan tüm istatistiki verilere python aracılığıyla erişmenize imkan sağlar.
-        
-        ## Kurulum
-        evds paketini pip paket yöneticisi aracılığıyla kurabilirsiniz:
-        ```
-        pip install evds --upgrade
-        ```
-        ## Yenilikler
-        0.2 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
-        1. `get_data`, `get_sub_categories` ve `get_series` fonksiyonlarına, `raw` parametresi eklendi. Bu parametre `True` olarak tanımlandığında ilgili verilere dictionary formatında erişebilirsiniz.
-        2. Çeşitli hatalar giderildi.
-        
-        0.1.1 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
-        1. formulas parametresindeki hata giderildi.
-        
-        0.1.0 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
-        1. API üzerinden erişilemeyen serilere ilişkin EVDS'de yapılan güncellemeye paralel olarak tüm serilere erişim olanağı sağlanmıştır.
-        2. Proxy desteği eklenmiştir. 
-        3. Küçük hatalar giderildi
-        
-        ## Kullanım
-        Örnek kullanım, 01-01-2019 - 01-01-2020 arası USD ve EUR alış kurlarına aşağıdaki şekilde erişilebilir.
-        ```python
-        from evds import evdsAPI
-        evds = evdsAPI('EVDS_API_ANAHTARI')
-        evds.get_data(['TP.DK.USD.A.YTL','TP.DK.EUR.A.YTL'], startdate="01-01-2019", enddate="01-01-2020")
-        ```
-        get_data fonksiyonu DataFrame return edecektir. İstenmesi halinde  `raw=True` parametresi ile dictionary formatında ham veriye ulaşılabilir.
-        ### API Anahtarı Alma
-        evds paketini kullanmak için öncelikle EVDS sistemi üzerinden API Anahtarı almanız gerekmektedir. API Anahtarı almak için aşağıdaki adımları izleyiniz:
-        1. [EVDS](https://evds2.tcmb.gov.tr/) sayfasına giriş yaptıktan sonra Giriş Yap ve Kayıt Ol bağlantılarını izleyerek bir EVDS hesabı oluşturun.
-        2. Ardından kullanıcı adınızın altında yer alan profil bağlantısına tıklayınız.
-        
-        ![01](01.png)
-        
-        3. Profil sayfanızın alt kısmında yer alan "API Anahtarı" butonuna tıklayınız ve açılan kutucukta yer alan değeri kopyalayınız.
-        
-        ![02](02.png)
-        
-        ### Detaylı Sorgulama
-        `get_data` fonksiyonu aşağıdaki parametreleri alır:
-        #### series
-        Bu parametre liste olarak tanımlanmalıdır. Ayrıca birden fazla seri bu liste içerisinde tanımlanabilir. Tanımlanması zorunludur.
-        #### startdate
-        Seride yer alan verilerin hangi tarihten itibaren seçileceği bu parametre ile belirlenir. Tanımlanması zorunludur.
-        #### enddate
-        Eğer seri üzerinde bir aralık seçimi yapılmak isteniyorsa aralığın bitiş tarihi bu parametre ile belirtilir. Tanımlanması ihtiyaridir. Tanımlanmadığı durumda `startdate` değerine eşit olarak tanımlanır.
-        #### raw
-        `True` olması halinde fonksiyon talep edilen veriyi DataFrame yerine dictionary return eder. 
-        Örnek kullanım:
-        ```python
-        ...
-        evds.get_data(['TP.DK.USD.A.YTL','TP.DK.EUR.A.YTL'], startdate="01-01-2019", enddate="01-01-2020", raw=True)
-        ```
-        #### aggregation_types
-        Seri içindeki verilerin getirilmesi esnasında kullanılacak olan toplululaştırma yöntemini ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı yöntem kullanılır. Ayrıca değer olarak string veya liste alabilir. String alması durumunda tüm seriler için aynı yöntem uygulanır. Liste olarak tanımlanırsa `series` parametresinde tanımlanan serilere sırasıyla belirtilen yöntemler uygulanır.
-        Kullanılabilecek yöntemler aşağıdaki gibidir:
-        
-        |Yöntem|Parametre Değeri|
-        |------|----------------|
-        |Ortalama| avg|
-        |En düşük| min|
-        |En yüksek| max|
-        |Başlangıç| first|
-        |Bitiş| last|
-        |Kümülatif| sum|
-        
-        #### formulas
-        Seri içindeki verilerin getirilmesi esnasında uygulanacak formülü ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı formül kullanılır. Ayrıca değer olarak string veya liste alabilir. String alması durumunda tüm seriler için aynı formül uygulanır. Liste olarak tanımlanırsa `series` parametresinde tanımlanan serilere sırasıyla belirtilen formüller uygulanır.
-        Kullanılabilecek yöntemler aşağıdaki gibidir:
-        
-        |Formül|Değer|
-        |-------------|-|
-        |Düzey (Öntanımlı)|0|
-        |Yüzde Değişim|1|
-        |Fark|2|
-        |Yıllık Yüzde Değişim |3|
-        |Yıllık Fark|4|
-        |Bir Önceki Yılın Sonuna Göre Yüzde Değişim| 5|
-        |Bir Önceki Yılın Sonuna Göre Fark| 6|
-        |Hareketli Ortalama| 7|
-        |Hareketli Toplam| 8|
-        
-        API formula parametresi uygulandığında orijinal değerleri `None` olarak yanıtladığı için, formula parametresi tanımladığınız serinin orijinal değerlere ulaşmak için aynı seriyi tekrar ekleyiniz ve formula parametresini 0 olarak tanımlayınız. Örneğin
-        ```python
-        evds.get_data(['TP.DK.USD.A.YTL','TP.DK.USD.A.YTL'], 
-                      startdate="01-01-2019", 
-                      enddate="01-01-2020",
-                      formulas=[1,0],
-                        )
-        ```
-        USD için yüzde değişim ve orijinal değerlere aynı anda yukarıdaki gibi ulaşabilirsiniz.
-        
-        #### frequency
-        Seri içerisinde yer alan verilerin hangi sıklıkla getireceğini ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı yayımlanma sıklığı kullanılır.Aşağıdaki değerleri alabilir.
-        
-        |Sıklık|Değer|
-        |------|-----|
-        |Günlük| 1|
-        |İşgünü| 2|
-        |Haftalık| 3|
-        |Ayda 2 Kez| 4|
-        |Aylık| 5|
-        |3 Aylık| 6|
-        |6 Aylık| 7|
-        |Yıllık| 8|
-        
-        ## Mevcut Serileri Listeleme
-        EVDS üzerinde veri serileri sırasıyla Ana Kategori, Alt Kategori ve Seri hiyerarşisinde sunulmaktadır. 
-        > `get_data` fonksiyonun kullanılması için aşağıda yer alan işlemlerin gerçekleştirilmesine gerek yoktur. Veri serisine ait kodun bilinmesi durumunda doğrudan `get_data` fonksiyonu kullanılabilir.
-        
-        ### Ana kategorileri listeleme
-        `main_categories` değişkeni ile ana kategorileri listeleyebilirsiniz.
-        
-        ```python
-        ...
-        evds.main_categories
-        ```
-        komut ile ana kategorileri listeleyebilirsiniz. 
-        
-        |CATEGORY_ID | TOPIC_TITLE_TR|
-        |------------|---------------|
-        | 1	|PİYASA VERİLERİ|
-        |	2	|KURLAR|
-        |	3	|FAİZ İSTATİSTİKLERİ|
-        |	4	|PARA VE BANKA İSTATİSTİKLERİ|
-        |	...	|...|
-        
-        ### Alt kategorileri listeleme
-        Ana kategori altında yer alan alt kategorilere aşağıdaki şekilde ulaşabilirsiniz. Ayrıca `raw=True` parametresi ile DataFrame yerine dictionary formatında alt kategorileri ulaşılabilir.
-        ```python
-        evds.get_sub_categories('Ana kategori ID'si veya Adı')
-        ```
-        Örnek kulllanım;
-        ```python
-        ...
-        evds.get_sub_categories(6)
-        ```
-        |CATEGORY_ID	|DATAGROUP_CODE	|DATAGROUP_NAME|
-        |-------------|---------------|--------------|
-        |6	|bie_dbafod	|Dış Borç Anapara ve Faiz Ödemeleri ile Diğer T...|
-        |6	|bie_dbdborc	|Dış Borçlar-Brüt (Hazine ve Maliye Bakanlığı)|
-        |6	|bie_kvdbs	|Kısa Vadeli Dış Borç Stoku (milyon ABD doları)|
-        |6	|bie_yssk	|Özel Sektörün Yurt Dışından Sağladığı Uzun Vad...|
-        
-        Yukarıda yer alan örnekte 6'nolu kategori altında yer alan alt kategoriler listelenmiştir. Ayrıca `get_sub_categories` fonksiyonunda CATEGORY_ID yerine doğrudan ana kategori adı ile kullanabilirsiniz. Örneğin 
-        ```python
-        ...
-        evds.get_sub_categories("KURLAR")
-        ```
-        ### Serileri listeleme
-        Alt kategori altında yer alan veri serilerine aşağıdaki şekilde ulaşabilirsiniz. Ayrıca `raw=True` parametresi ile DataFrame yerine dictionary formatında serilere ulaşılabilir.
-        ```python
-        evds.get_series('Alt kategori adı')
-        ```
-        Örnek kulllanım;
-        ```
-        ...
-        evds.get_series('bie_dbdborc')
-        ```
-        |SERIE_CODE|	SERIE_NAME|	START_DATE|
-        |----------|------------|-----------|
-        |TP.DB.B01|	1:TÜRKİYE BRÜT DIŞ BORÇ STOKU|	01-10-1989|
-        |TP.DB.B02|	2:KISA VADELİ BORÇLAR (Borçluya Göre)|	01-10-1989|
-        |TP.DB.B03|	2A:KAMU (Borçluya Göre)|	01-10-1989
-        |TP.DB.B04|	2A1:GENEL YÖNETİM (Borçluya Göre)|	01-10-1989|
-        |TP.DB.B05|	2A1a:Merkezi Yönetim|	01-10-1989|
-        
-        `get_data()` fonksiyonu aracılığıyla SERIE_CODE'u kullanarak serilere ait verilere ulaşabilirsiniz.
-        ## Proxy Tanımlama
-        Proxy adresinizi aşağıdaki gibi `proxies` parametresi ile tanımlayabilirsiniz. Ayrıca `httpsVerify` parametresi ile https kontrolünü devre dışı bırakabilirsiniz.
-        ```
-        proxies = { "https" : "HTTPS_PROXY_URL"}
-        evds = evdsAPI('EVDS_API_ANAHTARI', proxies=proxies, httpsVerify=False)
-        ```
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# EVDS
+
+[English](https://github.com/fatihmete/evds/blob/master/README_EN.md)
+
+EVDS paketi EVDS-API üzerinden Türkiye Cumhuriyet Merkez Bankası (TCMB) tarafından Elektronik Veri Dağıtım Sistemi (EVDS) aracılığıyla yayımlanan tüm istatistiki verilere python aracılığıyla erişmenize imkan sağlar.
+
+EVDS paketi resmi bir paket olmayıp açık kaynak kodlu olarak geliştirilmektedir.
+
+## Kurulum
+
+evds paketini pip paket yöneticisi aracılığıyla kurabilirsiniz:
+
+```
+pip install evds --upgrade
+```
+
+## Yenilikler
+
+0.3 sürümü ile aşağıdaki değişiklikler yapıldı:
+
+1. SSL hatalarının giderilmesi için legacySSL parametresi eklendi. [PR #8](https://github.com/fatihmete/evds/pull/8)
+2. Kod içerisinde düzeltmeler yapıldı. [PR #6](https://github.com/fatihmete/evds/pull/6) [PR #4](https://github.com/fatihmete/evds/pull/4)
+3. request session'un açık kalması nedeniyle ortaya çıkan ResourceWarning uyarısı giderildi. [PR #4](https://github.com/fatihmete/evds/pull/4)
+4. Pandas DataFrame numeric tiplere cast ederken ortaya çıkan FutureWarning uyarıları çıkıyordu. Bu sorun giderildi. [PR #9](https://github.com/fatihmete/evds/pull/9)
+
+0.2 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
+
+1. `get_data`, `get_sub_categories` ve `get_series` fonksiyonlarına, `raw` parametresi eklendi. Bu parametre `True` olarak tanımlandığında ilgili verilere dictionary formatında erişebilirsiniz.
+2. Çeşitli hatalar giderildi.
+
+0.1.1 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
+
+1. formulas parametresindeki hata giderildi.
+
+0.1.0 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
+
+1. API üzerinden erişilemeyen serilere ilişkin EVDS'de yapılan güncellemeye paralel olarak tüm serilere erişim olanağı sağlanmıştır.
+2. Proxy desteği eklenmiştir.
+3. Küçük hatalar giderildi
+
+## Kullanım
+
+Örnek kullanım, 01-01-2019 - 01-01-2020 arası USD ve EUR alış kurlarına aşağıdaki şekilde erişilebilir.
+
+```python
+from evds import evdsAPI
+evds = evdsAPI('EVDS_API_ANAHTARI')
+evds.get_data(['TP.DK.USD.A.YTL','TP.DK.EUR.A.YTL'], startdate="01-01-2019", enddate="01-01-2020")
+```
+
+get_data fonksiyonu DataFrame return edecektir. İstenmesi halinde `raw=True` parametresi ile dictionary formatında ham veriye ulaşılabilir.
+
+### API Anahtarı Alma
+
+evds paketini kullanmak için öncelikle EVDS sistemi üzerinden API Anahtarı almanız gerekmektedir. API Anahtarı almak için aşağıdaki adımları izleyiniz:
+
+1. [EVDS](https://evds2.tcmb.gov.tr/) sayfasına giriş yaptıktan sonra Giriş Yap ve Kayıt Ol bağlantılarını izleyerek bir EVDS hesabı oluşturun.
+2. Ardından kullanıcı adınızın altında yer alan profil bağlantısına tıklayınız.
+
+![01](01.png)
+
+3. Profil sayfanızın alt kısmında yer alan "API Anahtarı" butonuna tıklayınız ve açılan kutucukta yer alan değeri kopyalayınız.
+
+![02](02.png)
+
+### Detaylı Sorgulama
+
+`get_data` fonksiyonu aşağıdaki parametreleri alır:
+
+#### series
+
+Bu parametre liste olarak tanımlanmalıdır. Ayrıca birden fazla seri bu liste içerisinde tanımlanabilir. Tanımlanması zorunludur.
+
+#### startdate
+
+Seride yer alan verilerin hangi tarihten itibaren seçileceği bu parametre ile belirlenir. Tanımlanması zorunludur.
+
+#### enddate
+
+Eğer seri üzerinde bir aralık seçimi yapılmak isteniyorsa aralığın bitiş tarihi bu parametre ile belirtilir. Tanımlanması ihtiyaridir. Tanımlanmadığı durumda `startdate` değerine eşit olarak tanımlanır.
+
+#### raw
+
+`True` olması halinde fonksiyon talep edilen veriyi DataFrame yerine dictionary return eder.
+Örnek kullanım:
+
+```python
+...
+evds.get_data(['TP.DK.USD.A.YTL','TP.DK.EUR.A.YTL'], startdate="01-01-2019", enddate="01-01-2020", raw=True)
+```
+
+#### aggregation_types
+
+Seri içindeki verilerin getirilmesi esnasında kullanılacak olan toplululaştırma yöntemini ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı yöntem kullanılır. Ayrıca değer olarak string veya liste alabilir. String alması durumunda tüm seriler için aynı yöntem uygulanır. Liste olarak tanımlanırsa `series` parametresinde tanımlanan serilere sırasıyla belirtilen yöntemler uygulanır.
+Kullanılabilecek yöntemler aşağıdaki gibidir:
+
+| Yöntem    | Parametre Değeri |
+| --------- | ---------------- |
+| Ortalama  | avg              |
+| En düşük  | min              |
+| En yüksek | max              |
+| Başlangıç | first            |
+| Bitiş     | last             |
+| Kümülatif | sum              |
+
+#### formulas
+
+Seri içindeki verilerin getirilmesi esnasında uygulanacak formülü ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı formül kullanılır. Ayrıca değer olarak string veya liste alabilir. String alması durumunda tüm seriler için aynı formül uygulanır. Liste olarak tanımlanırsa `series` parametresinde tanımlanan serilere sırasıyla belirtilen formüller uygulanır.
+Kullanılabilecek yöntemler aşağıdaki gibidir:
+
+| Formül                                     | Değer |
+| ------------------------------------------ | ----- |
+| Düzey (Öntanımlı)                          | 0     |
+| Yüzde Değişim                              | 1     |
+| Fark                                       | 2     |
+| Yıllık Yüzde Değişim                       | 3     |
+| Yıllık Fark                                | 4     |
+| Bir Önceki Yılın Sonuna Göre Yüzde Değişim | 5     |
+| Bir Önceki Yılın Sonuna Göre Fark          | 6     |
+| Hareketli Ortalama                         | 7     |
+| Hareketli Toplam                           | 8     |
+
+API formula parametresi uygulandığında orijinal değerleri `None` olarak yanıtladığı için, formula parametresi tanımladığınız serinin orijinal değerlere ulaşmak için aynı seriyi tekrar ekleyiniz ve formula parametresini 0 olarak tanımlayınız. Örneğin
+
+```python
+evds.get_data(['TP.DK.USD.A.YTL','TP.DK.USD.A.YTL'],
+              startdate="01-01-2019",
+              enddate="01-01-2020",
+              formulas=[1,0],
+                )
+```
+
+USD için yüzde değişim ve orijinal değerlere aynı anda yukarıdaki gibi ulaşabilirsiniz.
+
+#### frequency
+
+Seri içerisinde yer alan verilerin hangi sıklıkla getireceğini ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı yayımlanma sıklığı kullanılır.Aşağıdaki değerleri alabilir.
+
+| Sıklık     | Değer |
+| ---------- | ----- |
+| Günlük     | 1     |
+| İşgünü     | 2     |
+| Haftalık   | 3     |
+| Ayda 2 Kez | 4     |
+| Aylık      | 5     |
+| 3 Aylık    | 6     |
+| 6 Aylık    | 7     |
+| Yıllık     | 8     |
+
+## Mevcut Serileri Listeleme
+
+EVDS üzerinde veri serileri sırasıyla Ana Kategori, Alt Kategori ve Seri hiyerarşisinde sunulmaktadır.
+
+> `get_data` fonksiyonun kullanılması için aşağıda yer alan işlemlerin gerçekleştirilmesine gerek yoktur. Veri serisine ait kodun bilinmesi durumunda doğrudan `get_data` fonksiyonu kullanılabilir.
+
+### Ana kategorileri listeleme
+
+`main_categories` değişkeni ile ana kategorileri listeleyebilirsiniz.
+
+```python
+...
+evds.main_categories
+```
+
+komut ile ana kategorileri listeleyebilirsiniz.
+
+| CATEGORY_ID | TOPIC_TITLE_TR               |
+| ----------- | ---------------------------- |
+| 1           | PİYASA VERİLERİ              |
+| 2           | KURLAR                       |
+| 3           | FAİZ İSTATİSTİKLERİ          |
+| 4           | PARA VE BANKA İSTATİSTİKLERİ |
+| ...         | ...                          |
+
+### Alt kategorileri listeleme
+
+Ana kategori altında yer alan alt kategorilere aşağıdaki şekilde ulaşabilirsiniz. Ayrıca `raw=True` parametresi ile DataFrame yerine dictionary formatında alt kategorileri ulaşılabilir.
+
+```python
+evds.get_sub_categories('Ana kategori ID'si veya Adı')
+```
+
+Örnek kulllanım;
+
+```python
+...
+evds.get_sub_categories(6)
+```
+
+| CATEGORY_ID | DATAGROUP_CODE | DATAGROUP_NAME                                    |
+| ----------- | -------------- | ------------------------------------------------- |
+| 6           | bie_dbafod     | Dış Borç Anapara ve Faiz Ödemeleri ile Diğer T... |
+| 6           | bie_dbdborc    | Dış Borçlar-Brüt (Hazine ve Maliye Bakanlığı)     |
+| 6           | bie_kvdbs      | Kısa Vadeli Dış Borç Stoku (milyon ABD doları)    |
+| 6           | bie_yssk       | Özel Sektörün Yurt Dışından Sağladığı Uzun Vad... |
+
+Yukarıda yer alan örnekte 6'nolu kategori altında yer alan alt kategoriler listelenmiştir. Ayrıca `get_sub_categories` fonksiyonunda CATEGORY_ID yerine doğrudan ana kategori adı ile kullanabilirsiniz. Örneğin
+
+```python
+...
+evds.get_sub_categories("KURLAR")
+```
+
+### Serileri listeleme
+
+Alt kategori altında yer alan veri serilerine aşağıdaki şekilde ulaşabilirsiniz. Ayrıca `raw=True` parametresi ile DataFrame yerine dictionary formatında serilere ulaşılabilir.
+
+```python
+evds.get_series('Alt kategori adı')
+```
+
+Örnek kulllanım;
+
+```
+...
+evds.get_series('bie_dbdborc')
+```
+
+| SERIE_CODE | SERIE_NAME                            | START_DATE |
+| ---------- | ------------------------------------- | ---------- |
+| TP.DB.B01  | 1:TÜRKİYE BRÜT DIŞ BORÇ STOKU         | 01-10-1989 |
+| TP.DB.B02  | 2:KISA VADELİ BORÇLAR (Borçluya Göre) | 01-10-1989 |
+| TP.DB.B03  | 2A:KAMU (Borçluya Göre)               | 01-10-1989 |
+| TP.DB.B04  | 2A1:GENEL YÖNETİM (Borçluya Göre)     | 01-10-1989 |
+| TP.DB.B05  | 2A1a:Merkezi Yönetim                  | 01-10-1989 |
+
+`get_data()` fonksiyonu aracılığıyla SERIE_CODE'u kullanarak serilere ait verilere ulaşabilirsiniz.
+
+## Proxy Tanımlama
+
+Proxy adresinizi aşağıdaki gibi `proxies` parametresi ile tanımlayabilirsiniz. Ayrıca `httpsVerify` parametresi ile https kontrolünü devre dışı bırakabilirsiniz.
+
+```
+proxies = { "https" : "HTTPS_PROXY_URL"}
+evds = evdsAPI('EVDS_API_ANAHTARI', proxies=proxies, httpsVerify=False)
+```
+
+## SSLError Hatası çözümü
+
+Sunucu sertifikası ve kullanılan python paketlerinden kaynaklı olarak SSL hatası alınabilmektedir. Bu hata durumunda legacySSL parametresi kullanılabilir:
+
+```
+evds = evdsAPI('EVDS_API_ANAHTARI', legacySSL=True)
+
+```
```

### Comparing `evds-0.2.0/README.md` & `evds-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,179 +1,259 @@
+Metadata-Version: 2.1
+Name: evds
+Version: 0.3.0
+Summary: EVDS python wrapper
+Home-page: https://github.com/fatihmete/evds
+Author: Fatih Mete
+Author-email: fatihmete@live.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
 # EVDS
 
 [English](https://github.com/fatihmete/evds/blob/master/README_EN.md)
 
 EVDS paketi EVDS-API üzerinden Türkiye Cumhuriyet Merkez Bankası (TCMB) tarafından Elektronik Veri Dağıtım Sistemi (EVDS) aracılığıyla yayımlanan tüm istatistiki verilere python aracılığıyla erişmenize imkan sağlar.
 
+EVDS paketi resmi bir paket olmayıp açık kaynak kodlu olarak geliştirilmektedir.
+
 ## Kurulum
+
 evds paketini pip paket yöneticisi aracılığıyla kurabilirsiniz:
+
 ```
 pip install evds --upgrade
 ```
+
 ## Yenilikler
+
+0.3 sürümü ile aşağıdaki değişiklikler yapıldı:
+
+1. SSL hatalarının giderilmesi için legacySSL parametresi eklendi. [PR #8](https://github.com/fatihmete/evds/pull/8)
+2. Kod içerisinde düzeltmeler yapıldı. [PR #6](https://github.com/fatihmete/evds/pull/6) [PR #4](https://github.com/fatihmete/evds/pull/4)
+3. request session'un açık kalması nedeniyle ortaya çıkan ResourceWarning uyarısı giderildi. [PR #4](https://github.com/fatihmete/evds/pull/4)
+4. Pandas DataFrame numeric tiplere cast ederken ortaya çıkan FutureWarning uyarıları çıkıyordu. Bu sorun giderildi. [PR #9](https://github.com/fatihmete/evds/pull/9)
+
 0.2 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
+
 1. `get_data`, `get_sub_categories` ve `get_series` fonksiyonlarına, `raw` parametresi eklendi. Bu parametre `True` olarak tanımlandığında ilgili verilere dictionary formatında erişebilirsiniz.
 2. Çeşitli hatalar giderildi.
 
 0.1.1 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
+
 1. formulas parametresindeki hata giderildi.
 
 0.1.0 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
+
 1. API üzerinden erişilemeyen serilere ilişkin EVDS'de yapılan güncellemeye paralel olarak tüm serilere erişim olanağı sağlanmıştır.
-2. Proxy desteği eklenmiştir. 
+2. Proxy desteği eklenmiştir.
 3. Küçük hatalar giderildi
 
 ## Kullanım
+
 Örnek kullanım, 01-01-2019 - 01-01-2020 arası USD ve EUR alış kurlarına aşağıdaki şekilde erişilebilir.
+
 ```python
 from evds import evdsAPI
 evds = evdsAPI('EVDS_API_ANAHTARI')
 evds.get_data(['TP.DK.USD.A.YTL','TP.DK.EUR.A.YTL'], startdate="01-01-2019", enddate="01-01-2020")
 ```
-get_data fonksiyonu DataFrame return edecektir. İstenmesi halinde  `raw=True` parametresi ile dictionary formatında ham veriye ulaşılabilir.
+
+get_data fonksiyonu DataFrame return edecektir. İstenmesi halinde `raw=True` parametresi ile dictionary formatında ham veriye ulaşılabilir.
+
 ### API Anahtarı Alma
+
 evds paketini kullanmak için öncelikle EVDS sistemi üzerinden API Anahtarı almanız gerekmektedir. API Anahtarı almak için aşağıdaki adımları izleyiniz:
+
 1. [EVDS](https://evds2.tcmb.gov.tr/) sayfasına giriş yaptıktan sonra Giriş Yap ve Kayıt Ol bağlantılarını izleyerek bir EVDS hesabı oluşturun.
 2. Ardından kullanıcı adınızın altında yer alan profil bağlantısına tıklayınız.
 
 ![01](01.png)
 
 3. Profil sayfanızın alt kısmında yer alan "API Anahtarı" butonuna tıklayınız ve açılan kutucukta yer alan değeri kopyalayınız.
 
 ![02](02.png)
 
 ### Detaylı Sorgulama
+
 `get_data` fonksiyonu aşağıdaki parametreleri alır:
+
 #### series
+
 Bu parametre liste olarak tanımlanmalıdır. Ayrıca birden fazla seri bu liste içerisinde tanımlanabilir. Tanımlanması zorunludur.
+
 #### startdate
+
 Seride yer alan verilerin hangi tarihten itibaren seçileceği bu parametre ile belirlenir. Tanımlanması zorunludur.
+
 #### enddate
+
 Eğer seri üzerinde bir aralık seçimi yapılmak isteniyorsa aralığın bitiş tarihi bu parametre ile belirtilir. Tanımlanması ihtiyaridir. Tanımlanmadığı durumda `startdate` değerine eşit olarak tanımlanır.
+
 #### raw
-`True` olması halinde fonksiyon talep edilen veriyi DataFrame yerine dictionary return eder. 
+
+`True` olması halinde fonksiyon talep edilen veriyi DataFrame yerine dictionary return eder.
 Örnek kullanım:
+
 ```python
 ...
 evds.get_data(['TP.DK.USD.A.YTL','TP.DK.EUR.A.YTL'], startdate="01-01-2019", enddate="01-01-2020", raw=True)
 ```
+
 #### aggregation_types
+
 Seri içindeki verilerin getirilmesi esnasında kullanılacak olan toplululaştırma yöntemini ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı yöntem kullanılır. Ayrıca değer olarak string veya liste alabilir. String alması durumunda tüm seriler için aynı yöntem uygulanır. Liste olarak tanımlanırsa `series` parametresinde tanımlanan serilere sırasıyla belirtilen yöntemler uygulanır.
 Kullanılabilecek yöntemler aşağıdaki gibidir:
 
-|Yöntem|Parametre Değeri|
-|------|----------------|
-|Ortalama| avg|
-|En düşük| min|
-|En yüksek| max|
-|Başlangıç| first|
-|Bitiş| last|
-|Kümülatif| sum|
+| Yöntem    | Parametre Değeri |
+| --------- | ---------------- |
+| Ortalama  | avg              |
+| En düşük  | min              |
+| En yüksek | max              |
+| Başlangıç | first            |
+| Bitiş     | last             |
+| Kümülatif | sum              |
 
 #### formulas
+
 Seri içindeki verilerin getirilmesi esnasında uygulanacak formülü ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı formül kullanılır. Ayrıca değer olarak string veya liste alabilir. String alması durumunda tüm seriler için aynı formül uygulanır. Liste olarak tanımlanırsa `series` parametresinde tanımlanan serilere sırasıyla belirtilen formüller uygulanır.
 Kullanılabilecek yöntemler aşağıdaki gibidir:
 
-|Formül|Değer|
-|-------------|-|
-|Düzey (Öntanımlı)|0|
-|Yüzde Değişim|1|
-|Fark|2|
-|Yıllık Yüzde Değişim |3|
-|Yıllık Fark|4|
-|Bir Önceki Yılın Sonuna Göre Yüzde Değişim| 5|
-|Bir Önceki Yılın Sonuna Göre Fark| 6|
-|Hareketli Ortalama| 7|
-|Hareketli Toplam| 8|
+| Formül                                     | Değer |
+| ------------------------------------------ | ----- |
+| Düzey (Öntanımlı)                          | 0     |
+| Yüzde Değişim                              | 1     |
+| Fark                                       | 2     |
+| Yıllık Yüzde Değişim                       | 3     |
+| Yıllık Fark                                | 4     |
+| Bir Önceki Yılın Sonuna Göre Yüzde Değişim | 5     |
+| Bir Önceki Yılın Sonuna Göre Fark          | 6     |
+| Hareketli Ortalama                         | 7     |
+| Hareketli Toplam                           | 8     |
 
 API formula parametresi uygulandığında orijinal değerleri `None` olarak yanıtladığı için, formula parametresi tanımladığınız serinin orijinal değerlere ulaşmak için aynı seriyi tekrar ekleyiniz ve formula parametresini 0 olarak tanımlayınız. Örneğin
+
 ```python
-evds.get_data(['TP.DK.USD.A.YTL','TP.DK.USD.A.YTL'], 
-              startdate="01-01-2019", 
+evds.get_data(['TP.DK.USD.A.YTL','TP.DK.USD.A.YTL'],
+              startdate="01-01-2019",
               enddate="01-01-2020",
               formulas=[1,0],
                 )
 ```
+
 USD için yüzde değişim ve orijinal değerlere aynı anda yukarıdaki gibi ulaşabilirsiniz.
 
 #### frequency
+
 Seri içerisinde yer alan verilerin hangi sıklıkla getireceğini ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı yayımlanma sıklığı kullanılır.Aşağıdaki değerleri alabilir.
 
-|Sıklık|Değer|
-|------|-----|
-|Günlük| 1|
-|İşgünü| 2|
-|Haftalık| 3|
-|Ayda 2 Kez| 4|
-|Aylık| 5|
-|3 Aylık| 6|
-|6 Aylık| 7|
-|Yıllık| 8|
+| Sıklık     | Değer |
+| ---------- | ----- |
+| Günlük     | 1     |
+| İşgünü     | 2     |
+| Haftalık   | 3     |
+| Ayda 2 Kez | 4     |
+| Aylık      | 5     |
+| 3 Aylık    | 6     |
+| 6 Aylık    | 7     |
+| Yıllık     | 8     |
 
 ## Mevcut Serileri Listeleme
-EVDS üzerinde veri serileri sırasıyla Ana Kategori, Alt Kategori ve Seri hiyerarşisinde sunulmaktadır. 
+
+EVDS üzerinde veri serileri sırasıyla Ana Kategori, Alt Kategori ve Seri hiyerarşisinde sunulmaktadır.
+
 > `get_data` fonksiyonun kullanılması için aşağıda yer alan işlemlerin gerçekleştirilmesine gerek yoktur. Veri serisine ait kodun bilinmesi durumunda doğrudan `get_data` fonksiyonu kullanılabilir.
 
 ### Ana kategorileri listeleme
+
 `main_categories` değişkeni ile ana kategorileri listeleyebilirsiniz.
 
 ```python
 ...
 evds.main_categories
 ```
-komut ile ana kategorileri listeleyebilirsiniz. 
 
-|CATEGORY_ID | TOPIC_TITLE_TR|
-|------------|---------------|
-| 1	|PİYASA VERİLERİ|
-|	2	|KURLAR|
-|	3	|FAİZ İSTATİSTİKLERİ|
-|	4	|PARA VE BANKA İSTATİSTİKLERİ|
-|	...	|...|
+komut ile ana kategorileri listeleyebilirsiniz.
+
+| CATEGORY_ID | TOPIC_TITLE_TR               |
+| ----------- | ---------------------------- |
+| 1           | PİYASA VERİLERİ              |
+| 2           | KURLAR                       |
+| 3           | FAİZ İSTATİSTİKLERİ          |
+| 4           | PARA VE BANKA İSTATİSTİKLERİ |
+| ...         | ...                          |
 
 ### Alt kategorileri listeleme
+
 Ana kategori altında yer alan alt kategorilere aşağıdaki şekilde ulaşabilirsiniz. Ayrıca `raw=True` parametresi ile DataFrame yerine dictionary formatında alt kategorileri ulaşılabilir.
+
 ```python
 evds.get_sub_categories('Ana kategori ID'si veya Adı')
 ```
+
 Örnek kulllanım;
+
 ```python
 ...
 evds.get_sub_categories(6)
 ```
-|CATEGORY_ID	|DATAGROUP_CODE	|DATAGROUP_NAME|
-|-------------|---------------|--------------|
-|6	|bie_dbafod	|Dış Borç Anapara ve Faiz Ödemeleri ile Diğer T...|
-|6	|bie_dbdborc	|Dış Borçlar-Brüt (Hazine ve Maliye Bakanlığı)|
-|6	|bie_kvdbs	|Kısa Vadeli Dış Borç Stoku (milyon ABD doları)|
-|6	|bie_yssk	|Özel Sektörün Yurt Dışından Sağladığı Uzun Vad...|
 
-Yukarıda yer alan örnekte 6'nolu kategori altında yer alan alt kategoriler listelenmiştir. Ayrıca `get_sub_categories` fonksiyonunda CATEGORY_ID yerine doğrudan ana kategori adı ile kullanabilirsiniz. Örneğin 
+| CATEGORY_ID | DATAGROUP_CODE | DATAGROUP_NAME                                    |
+| ----------- | -------------- | ------------------------------------------------- |
+| 6           | bie_dbafod     | Dış Borç Anapara ve Faiz Ödemeleri ile Diğer T... |
+| 6           | bie_dbdborc    | Dış Borçlar-Brüt (Hazine ve Maliye Bakanlığı)     |
+| 6           | bie_kvdbs      | Kısa Vadeli Dış Borç Stoku (milyon ABD doları)    |
+| 6           | bie_yssk       | Özel Sektörün Yurt Dışından Sağladığı Uzun Vad... |
+
+Yukarıda yer alan örnekte 6'nolu kategori altında yer alan alt kategoriler listelenmiştir. Ayrıca `get_sub_categories` fonksiyonunda CATEGORY_ID yerine doğrudan ana kategori adı ile kullanabilirsiniz. Örneğin
+
 ```python
 ...
 evds.get_sub_categories("KURLAR")
 ```
+
 ### Serileri listeleme
+
 Alt kategori altında yer alan veri serilerine aşağıdaki şekilde ulaşabilirsiniz. Ayrıca `raw=True` parametresi ile DataFrame yerine dictionary formatında serilere ulaşılabilir.
+
 ```python
 evds.get_series('Alt kategori adı')
 ```
+
 Örnek kulllanım;
+
 ```
 ...
 evds.get_series('bie_dbdborc')
 ```
-|SERIE_CODE|	SERIE_NAME|	START_DATE|
-|----------|------------|-----------|
-|TP.DB.B01|	1:TÜRKİYE BRÜT DIŞ BORÇ STOKU|	01-10-1989|
-|TP.DB.B02|	2:KISA VADELİ BORÇLAR (Borçluya Göre)|	01-10-1989|
-|TP.DB.B03|	2A:KAMU (Borçluya Göre)|	01-10-1989
-|TP.DB.B04|	2A1:GENEL YÖNETİM (Borçluya Göre)|	01-10-1989|
-|TP.DB.B05|	2A1a:Merkezi Yönetim|	01-10-1989|
+
+| SERIE_CODE | SERIE_NAME                            | START_DATE |
+| ---------- | ------------------------------------- | ---------- |
+| TP.DB.B01  | 1:TÜRKİYE BRÜT DIŞ BORÇ STOKU         | 01-10-1989 |
+| TP.DB.B02  | 2:KISA VADELİ BORÇLAR (Borçluya Göre) | 01-10-1989 |
+| TP.DB.B03  | 2A:KAMU (Borçluya Göre)               | 01-10-1989 |
+| TP.DB.B04  | 2A1:GENEL YÖNETİM (Borçluya Göre)     | 01-10-1989 |
+| TP.DB.B05  | 2A1a:Merkezi Yönetim                  | 01-10-1989 |
 
 `get_data()` fonksiyonu aracılığıyla SERIE_CODE'u kullanarak serilere ait verilere ulaşabilirsiniz.
+
 ## Proxy Tanımlama
+
 Proxy adresinizi aşağıdaki gibi `proxies` parametresi ile tanımlayabilirsiniz. Ayrıca `httpsVerify` parametresi ile https kontrolünü devre dışı bırakabilirsiniz.
+
 ```
 proxies = { "https" : "HTTPS_PROXY_URL"}
 evds = evdsAPI('EVDS_API_ANAHTARI', proxies=proxies, httpsVerify=False)
 ```
+
+## SSLError Hatası çözümü
+
+Sunucu sertifikası ve kullanılan python paketlerinden kaynaklı olarak SSL hatası alınabilmektedir. Bu hata durumunda legacySSL parametresi kullanılabilir:
+
+```
+evds = evdsAPI('EVDS_API_ANAHTARI', legacySSL=True)
+
+```
```

### Comparing `evds-0.2.0/evds/__init__.py` & `evds-0.3.0/evds/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,110 +1,139 @@
 import pandas as pd
 import requests
 import json
-import warnings
+import ssl
+import urllib3
+
+class CustomHttpAdapter (requests.adapters.HTTPAdapter):
+    # "Transport adapter" that allows us to use custom ssl_context.
+    def __init__(self, ssl_context=None, **kwargs):
+        self.ssl_context = ssl_context
+        super().__init__(**kwargs)
+
+    def init_poolmanager(self, connections, maxsize, block=False):
+        self.poolmanager = urllib3.poolmanager.PoolManager(
+            num_pools=connections, maxsize=maxsize,
+            block=block, ssl_context=self.ssl_context)
+
 
 class evdsAPI:
     """
     for more detail https://github.com/fatihmete/evds
     Example usage:
     from evds import evdsAPI
     evds = evdsAPI('EVDS_API_KEY')
     evds.get_data(['TP.DK.USD.A.YTL','TP.DK.EUR.A.YTL'], startdate="01-01-2019", enddate="01-01-2020")
     """
-    def __init__(self, key, lang = "TR", DEBUG=False, proxies = "", httpsVerify = True):
+
+    def __init__(self, key, lang="TR", DEBUG=False, proxies="", httpsVerify=True, legacySSL=False):
         self.key = key
         self.DEBUG = DEBUG
         self.proxies = proxies
-        self.httspVerify = httpsVerify
-        self.session = requests.Session()
-        self.data = ""
-        if self.proxies != "":
-            self.session.proxies = self.proxies
-            self.session.verify = self.httspVerify
-        
-        if lang in ["TR","ENG"]:
+        self.httpsVerify = httpsVerify
+        self.legacySSL = legacySSL
+
+        self.__create_session()
+
+        if lang in ["TR", "ENG"]:
             self.lang = lang
         else:
             self.lang = "TR"
         # API returns this main categories but they are not available
         self.not_available_categories = [17]
 
         self.main_categories = self.__get_main_categories()
-        
+
+    def __create_session(self):
+        self.session = requests.Session()
+        if self.legacySSL:
+            ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
+            ctx.options |= 0x4  # OP_LEGACY_SERVER_CONNECT
+            self.session.mount('https://', CustomHttpAdapter(ctx))
+
+        if self.proxies != "":
+            self.session.proxies = self.proxies
+            self.session.verify = self.httpsVerify
+
     def __get_main_categories(self):
         """
         Function returns main categories dataframe.
         """
-        main_categories = self.__make_request('https://evds2.tcmb.gov.tr/service/evds/categories/',\
-                            params={'key' : self.key, 'type' : 'json'})
+        main_categories = self.__make_request('https://evds2.tcmb.gov.tr/service/evds/categories/',
+                                              params={'key': self.key, 'type': 'json'})
         try:
             main_categories_raw = json.loads(main_categories)
-            main_categories_df = pd.DataFrame(main_categories_raw, dtype="int")[["CATEGORY_ID","TOPIC_TITLE_" + self.lang]]
+            main_categories_df = pd.DataFrame(main_categories_raw)[
+                ["CATEGORY_ID", "TOPIC_TITLE_" + self.lang]]
+            main_categories_df["CATEGORY_ID"] = main_categories_df["CATEGORY_ID"].astype(
+                "int")
             return main_categories_df[~main_categories_df.CATEGORY_ID.isin(self.not_available_categories)]
-            
+
         except:
-            raise EVDSConnectionError(f"Main categories couldn't load. Please check your API Key.")
+            raise EVDSConnectionError(
+                f"Main categories couldn't load. Please check your API Key.")
 
     def get_sub_categories(self, main_category="", detail=False, raw=False):
         """
         The function returns sub-categories as dataframe object.
         If main_category,
             - Not defined, returns all subcategories,
             - Defined as an integer, returns subcategories which main category id match this value,
             - Defined as a string, depending on self.lang value, search in main category name and 
               returns matched the main category' subcategories
         """
         if main_category == "":
-            params={ 'key' : self.key, 'mode' : 0, 'code' : '', 'type' : 'json'}
-            
-        elif isinstance(main_category, (int,float)):
+            params = {'key': self.key, 'mode': 0, 'code': '', 'type': 'json'}
+
+        elif isinstance(main_category, (int, float)):
             if main_category in self.main_categories["CATEGORY_ID"].to_list():
-                params={ 'key' : self.key, 'mode' : 2, 'code' : main_category, 'type' : 'json'}
+                params = {'key': self.key, 'mode': 2,
+                          'code': main_category, 'type': 'json'}
             else:
                 raise CategoryNotFoundError("Category not found.")
         else:
             try:
-                code = self.main_categories[self.main_categories["TOPIC_TITLE_"+self.lang].str.contains(main_category)]\
-                        ["CATEGORY_ID"].values[0]
-                params={ 'key' : self.key, 'mode' : 2, 'code' : code , 'type' : 'json'}
+                code = self.main_categories[self.main_categories["TOPIC_TITLE_" +
+                                                                 self.lang].str.contains(main_category)]["CATEGORY_ID"].values[0]
+                params = {'key': self.key, 'mode': 2,
+                          'code': code, 'type': 'json'}
             except:
                 raise CategoryNotFoundError("Category not found.")
 
-        sub_categories = self.__make_request('https://evds2.tcmb.gov.tr/service/evds/datagroups/',\
-                            params=params)
+        sub_categories = self.__make_request('https://evds2.tcmb.gov.tr/service/evds/datagroups/',
+                                             params=params)
         sub_categories = json.loads(sub_categories)
         if raw:
             return sub_categories
         df = pd.DataFrame(sub_categories)
-        if detail==False:
-            return df[["CATEGORY_ID",\
-                       "DATAGROUP_CODE",\
-                       "DATAGROUP_NAME" + ("_ENG" if self.lang=="ENG" else "")]]
-        else:
-            return df
+        if detail == False:
+            return df[["CATEGORY_ID",
+                       "DATAGROUP_CODE",
+                       "DATAGROUP_NAME" + ("_ENG" if self.lang == "ENG" else "")]]
+
+        return df
 
     def get_series(self, datagroup_code, detail=False, raw=False):
         """
         The function returns dataframe of series which belongs to given data group.
         Because of default detail parameter is False, only return "SERIE_CODE", "SERIE_NAME" and "START_DATE" value.
         """
-        series = self.__make_request('https://evds2.tcmb.gov.tr/service/evds/serieList/',\
-                                    params = {'key' : self.key, 'type' : 'json', 'code' : datagroup_code})
+        series = self.__make_request('https://evds2.tcmb.gov.tr/service/evds/serieList/',
+                                     params={'key': self.key, 'type': 'json', 'code': datagroup_code})
         series = json.loads(series)
         if raw:
             return series
         df = pd.DataFrame(series)
         if detail == False:
-            return df[["SERIE_CODE",\
-                        "SERIE_NAME" + ("_ENG" if self.lang=="ENG" else ""),\
-                        "START_DATE"]]
-        else:
-            return df
-        
+            return df[["SERIE_CODE",
+                       "SERIE_NAME" + ("_ENG" if self.lang == "ENG" else ""),
+                       "START_DATE"]]
+
+        return df
+
     def get_data(self, series, startdate, enddate="", aggregation_types="", formulas="", frequency="", raw=False):
         """
         The function returns data of the given series data. Series must be typed as list.
         Also, set parameter raw=False to return dictionary format.
         If end date not defined, end date set as equal to start date
         If aggregation_types and formulas,
             - not defined, API returns value aggregated and calculated default aggregations type and formula for the series.
@@ -125,82 +154,94 @@
             Workday: 2
             Weekly: 3
             Two times in a month: 4
             Monthly: 5
             Quarterly: 6
             Six month: 7
             Yearly: 8
-        """     
-        if isinstance(series, list)==False:
+        """
+        if isinstance(series, list) == False:
             return print("Series type must be list.")
-            
-        #For daily data set enddate to startdate, if blank
-        if enddate=="":
+
+        # For daily data set enddate to startdate, if blank
+        if enddate == "":
             enddate = startdate
-            
+
         series_count = len(series)
-        
-        #Set aggregation type
-        if aggregation_types=="":
-            #Default aggregation method
+
+        # Set aggregation type
+        if aggregation_types == "":
+            # Default aggregation method
             aggregation_type_param = ''
         elif isinstance(aggregation_types, list):
-            #User defined aggregation per series
-            aggregation_type_param = "-".join([str(i) for i in aggregation_types])
-        else:
-            #User defined aggregation same for all series
-            aggregation_type_param = "-".join([str(aggregation_types) for i in range(series_count)])
-
-        #Set formulas
-        if formulas=="":
-            #Default formula
+            # User defined aggregation per series
+            aggregation_type_param = "-".join([str(i)
+                                              for i in aggregation_types])
+        else:
+            # User defined aggregation same for all series
+            aggregation_type_param = "-".join([str(aggregation_types)
+                                              for i in range(series_count)])
+
+        # Set formulas
+        if formulas == "":
+            # Default formula
             formula_param = ''
         elif isinstance(formulas, list):
-            #User defined formula per series
+            # User defined formula per series
             formula_param = "-".join([str(i) for i in formulas])
         else:
-            #User defined formula same for all series
-            formula_param = "-".join([str(formulas) for i in range(series_count)])
-
-        data = self.__make_request('https://evds2.tcmb.gov.tr/service/evds/',\
-                           params = {
-                            'series' : "-".join(series),
-                            'startDate' : startdate,
-                            'endDate' : enddate,
-                            'type' : 'json',
-                            'key' : self.key,
-                            'formulas' : formula_param,
-                            'frequency' : str(frequency),
-                            'aggregationTypes' : aggregation_type_param,
-                            })
+            # User defined formula same for all series
+            formula_param = "-".join([str(formulas)
+                                     for i in range(series_count)])
+
+        data = self.__make_request('https://evds2.tcmb.gov.tr/service/evds/',
+                                   params={
+                                       'series': "-".join(series),
+                                       'startDate': startdate,
+                                       'endDate': enddate,
+                                       'type': 'json',
+                                       'key': self.key,
+                                       'formulas': formula_param,
+                                       'frequency': str(frequency),
+                                       'aggregationTypes': aggregation_type_param,
+                                   })
         data = json.loads(data)["items"]
-        #If raw is true return only json results.
+        # If raw is true return only json results.
         if raw:
             return data
-        #Numeric values in json data is defined as text. To fix this problem, set dtype="float"
-        df = pd.DataFrame(data, dtype="float")
+
+        df = pd.DataFrame(data)
+
+        # Numeric values in json data is defined as string. To fix this problem, we cast values to float.
+        for serie_col in [s.replace(".", "_") for s in series]:
+            if serie_col in df.columns:
+                df[serie_col] = df[serie_col].astype("float")
+
         if "UNIXTIME" in df.columns:
             df.drop(columns=["UNIXTIME"], inplace=True)
         return df
-       
-    def __make_request(self,url,params={}):
+
+    def __make_request(self, url, params={}):
         params = self.__param_generator(params)
-        
         request = self.session.get(url + params)
-        print(request.url) if self.DEBUG==True else None
-        if request.status_code==200:
+        self.session.close()
+        print(request.url) if self.DEBUG == True else None
+        if request.status_code == 200:
             return request.content
         else:
-            raise EVDSConnectionError("Connection error, please check your API Key or request. Url:{}".format(request.url))
+            raise EVDSConnectionError(
+                "Connection error, please check your API Key or request. Url:{}".format(request.url))
 
-    def __param_generator(self,param):
+    def __param_generator(self, param):
         param_text = ''
-        for key,value in param.items():
+        for key, value in param.items():
             param_text += str(key) + "=" + str(value)
             param_text += '&'
         return param_text[:-1]
 
+
 class CategoryNotFoundError(Exception):
     pass
 
+
 class EVDSConnectionError(Exception):
-    pass
+    pass
```

### Comparing `evds-0.2.0/evds.egg-info/PKG-INFO` & `evds-0.3.0/evds.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,194 +1,259 @@
 Metadata-Version: 2.1
 Name: evds
-Version: 0.2.0
+Version: 0.3.0
 Summary: EVDS python wrapper
 Home-page: https://github.com/fatihmete/evds
 Author: Fatih Mete
 Author-email: fatihmete@live.com
-License: UNKNOWN
-Description: # EVDS
-        
-        [English](https://github.com/fatihmete/evds/blob/master/README_EN.md)
-        
-        EVDS paketi EVDS-API üzerinden Türkiye Cumhuriyet Merkez Bankası (TCMB) tarafından Elektronik Veri Dağıtım Sistemi (EVDS) aracılığıyla yayımlanan tüm istatistiki verilere python aracılığıyla erişmenize imkan sağlar.
-        
-        ## Kurulum
-        evds paketini pip paket yöneticisi aracılığıyla kurabilirsiniz:
-        ```
-        pip install evds --upgrade
-        ```
-        ## Yenilikler
-        0.2 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
-        1. `get_data`, `get_sub_categories` ve `get_series` fonksiyonlarına, `raw` parametresi eklendi. Bu parametre `True` olarak tanımlandığında ilgili verilere dictionary formatında erişebilirsiniz.
-        2. Çeşitli hatalar giderildi.
-        
-        0.1.1 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
-        1. formulas parametresindeki hata giderildi.
-        
-        0.1.0 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
-        1. API üzerinden erişilemeyen serilere ilişkin EVDS'de yapılan güncellemeye paralel olarak tüm serilere erişim olanağı sağlanmıştır.
-        2. Proxy desteği eklenmiştir. 
-        3. Küçük hatalar giderildi
-        
-        ## Kullanım
-        Örnek kullanım, 01-01-2019 - 01-01-2020 arası USD ve EUR alış kurlarına aşağıdaki şekilde erişilebilir.
-        ```python
-        from evds import evdsAPI
-        evds = evdsAPI('EVDS_API_ANAHTARI')
-        evds.get_data(['TP.DK.USD.A.YTL','TP.DK.EUR.A.YTL'], startdate="01-01-2019", enddate="01-01-2020")
-        ```
-        get_data fonksiyonu DataFrame return edecektir. İstenmesi halinde  `raw=True` parametresi ile dictionary formatında ham veriye ulaşılabilir.
-        ### API Anahtarı Alma
-        evds paketini kullanmak için öncelikle EVDS sistemi üzerinden API Anahtarı almanız gerekmektedir. API Anahtarı almak için aşağıdaki adımları izleyiniz:
-        1. [EVDS](https://evds2.tcmb.gov.tr/) sayfasına giriş yaptıktan sonra Giriş Yap ve Kayıt Ol bağlantılarını izleyerek bir EVDS hesabı oluşturun.
-        2. Ardından kullanıcı adınızın altında yer alan profil bağlantısına tıklayınız.
-        
-        ![01](01.png)
-        
-        3. Profil sayfanızın alt kısmında yer alan "API Anahtarı" butonuna tıklayınız ve açılan kutucukta yer alan değeri kopyalayınız.
-        
-        ![02](02.png)
-        
-        ### Detaylı Sorgulama
-        `get_data` fonksiyonu aşağıdaki parametreleri alır:
-        #### series
-        Bu parametre liste olarak tanımlanmalıdır. Ayrıca birden fazla seri bu liste içerisinde tanımlanabilir. Tanımlanması zorunludur.
-        #### startdate
-        Seride yer alan verilerin hangi tarihten itibaren seçileceği bu parametre ile belirlenir. Tanımlanması zorunludur.
-        #### enddate
-        Eğer seri üzerinde bir aralık seçimi yapılmak isteniyorsa aralığın bitiş tarihi bu parametre ile belirtilir. Tanımlanması ihtiyaridir. Tanımlanmadığı durumda `startdate` değerine eşit olarak tanımlanır.
-        #### raw
-        `True` olması halinde fonksiyon talep edilen veriyi DataFrame yerine dictionary return eder. 
-        Örnek kullanım:
-        ```python
-        ...
-        evds.get_data(['TP.DK.USD.A.YTL','TP.DK.EUR.A.YTL'], startdate="01-01-2019", enddate="01-01-2020", raw=True)
-        ```
-        #### aggregation_types
-        Seri içindeki verilerin getirilmesi esnasında kullanılacak olan toplululaştırma yöntemini ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı yöntem kullanılır. Ayrıca değer olarak string veya liste alabilir. String alması durumunda tüm seriler için aynı yöntem uygulanır. Liste olarak tanımlanırsa `series` parametresinde tanımlanan serilere sırasıyla belirtilen yöntemler uygulanır.
-        Kullanılabilecek yöntemler aşağıdaki gibidir:
-        
-        |Yöntem|Parametre Değeri|
-        |------|----------------|
-        |Ortalama| avg|
-        |En düşük| min|
-        |En yüksek| max|
-        |Başlangıç| first|
-        |Bitiş| last|
-        |Kümülatif| sum|
-        
-        #### formulas
-        Seri içindeki verilerin getirilmesi esnasında uygulanacak formülü ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı formül kullanılır. Ayrıca değer olarak string veya liste alabilir. String alması durumunda tüm seriler için aynı formül uygulanır. Liste olarak tanımlanırsa `series` parametresinde tanımlanan serilere sırasıyla belirtilen formüller uygulanır.
-        Kullanılabilecek yöntemler aşağıdaki gibidir:
-        
-        |Formül|Değer|
-        |-------------|-|
-        |Düzey (Öntanımlı)|0|
-        |Yüzde Değişim|1|
-        |Fark|2|
-        |Yıllık Yüzde Değişim |3|
-        |Yıllık Fark|4|
-        |Bir Önceki Yılın Sonuna Göre Yüzde Değişim| 5|
-        |Bir Önceki Yılın Sonuna Göre Fark| 6|
-        |Hareketli Ortalama| 7|
-        |Hareketli Toplam| 8|
-        
-        API formula parametresi uygulandığında orijinal değerleri `None` olarak yanıtladığı için, formula parametresi tanımladığınız serinin orijinal değerlere ulaşmak için aynı seriyi tekrar ekleyiniz ve formula parametresini 0 olarak tanımlayınız. Örneğin
-        ```python
-        evds.get_data(['TP.DK.USD.A.YTL','TP.DK.USD.A.YTL'], 
-                      startdate="01-01-2019", 
-                      enddate="01-01-2020",
-                      formulas=[1,0],
-                        )
-        ```
-        USD için yüzde değişim ve orijinal değerlere aynı anda yukarıdaki gibi ulaşabilirsiniz.
-        
-        #### frequency
-        Seri içerisinde yer alan verilerin hangi sıklıkla getireceğini ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı yayımlanma sıklığı kullanılır.Aşağıdaki değerleri alabilir.
-        
-        |Sıklık|Değer|
-        |------|-----|
-        |Günlük| 1|
-        |İşgünü| 2|
-        |Haftalık| 3|
-        |Ayda 2 Kez| 4|
-        |Aylık| 5|
-        |3 Aylık| 6|
-        |6 Aylık| 7|
-        |Yıllık| 8|
-        
-        ## Mevcut Serileri Listeleme
-        EVDS üzerinde veri serileri sırasıyla Ana Kategori, Alt Kategori ve Seri hiyerarşisinde sunulmaktadır. 
-        > `get_data` fonksiyonun kullanılması için aşağıda yer alan işlemlerin gerçekleştirilmesine gerek yoktur. Veri serisine ait kodun bilinmesi durumunda doğrudan `get_data` fonksiyonu kullanılabilir.
-        
-        ### Ana kategorileri listeleme
-        `main_categories` değişkeni ile ana kategorileri listeleyebilirsiniz.
-        
-        ```python
-        ...
-        evds.main_categories
-        ```
-        komut ile ana kategorileri listeleyebilirsiniz. 
-        
-        |CATEGORY_ID | TOPIC_TITLE_TR|
-        |------------|---------------|
-        | 1	|PİYASA VERİLERİ|
-        |	2	|KURLAR|
-        |	3	|FAİZ İSTATİSTİKLERİ|
-        |	4	|PARA VE BANKA İSTATİSTİKLERİ|
-        |	...	|...|
-        
-        ### Alt kategorileri listeleme
-        Ana kategori altında yer alan alt kategorilere aşağıdaki şekilde ulaşabilirsiniz. Ayrıca `raw=True` parametresi ile DataFrame yerine dictionary formatında alt kategorileri ulaşılabilir.
-        ```python
-        evds.get_sub_categories('Ana kategori ID'si veya Adı')
-        ```
-        Örnek kulllanım;
-        ```python
-        ...
-        evds.get_sub_categories(6)
-        ```
-        |CATEGORY_ID	|DATAGROUP_CODE	|DATAGROUP_NAME|
-        |-------------|---------------|--------------|
-        |6	|bie_dbafod	|Dış Borç Anapara ve Faiz Ödemeleri ile Diğer T...|
-        |6	|bie_dbdborc	|Dış Borçlar-Brüt (Hazine ve Maliye Bakanlığı)|
-        |6	|bie_kvdbs	|Kısa Vadeli Dış Borç Stoku (milyon ABD doları)|
-        |6	|bie_yssk	|Özel Sektörün Yurt Dışından Sağladığı Uzun Vad...|
-        
-        Yukarıda yer alan örnekte 6'nolu kategori altında yer alan alt kategoriler listelenmiştir. Ayrıca `get_sub_categories` fonksiyonunda CATEGORY_ID yerine doğrudan ana kategori adı ile kullanabilirsiniz. Örneğin 
-        ```python
-        ...
-        evds.get_sub_categories("KURLAR")
-        ```
-        ### Serileri listeleme
-        Alt kategori altında yer alan veri serilerine aşağıdaki şekilde ulaşabilirsiniz. Ayrıca `raw=True` parametresi ile DataFrame yerine dictionary formatında serilere ulaşılabilir.
-        ```python
-        evds.get_series('Alt kategori adı')
-        ```
-        Örnek kulllanım;
-        ```
-        ...
-        evds.get_series('bie_dbdborc')
-        ```
-        |SERIE_CODE|	SERIE_NAME|	START_DATE|
-        |----------|------------|-----------|
-        |TP.DB.B01|	1:TÜRKİYE BRÜT DIŞ BORÇ STOKU|	01-10-1989|
-        |TP.DB.B02|	2:KISA VADELİ BORÇLAR (Borçluya Göre)|	01-10-1989|
-        |TP.DB.B03|	2A:KAMU (Borçluya Göre)|	01-10-1989
-        |TP.DB.B04|	2A1:GENEL YÖNETİM (Borçluya Göre)|	01-10-1989|
-        |TP.DB.B05|	2A1a:Merkezi Yönetim|	01-10-1989|
-        
-        `get_data()` fonksiyonu aracılığıyla SERIE_CODE'u kullanarak serilere ait verilere ulaşabilirsiniz.
-        ## Proxy Tanımlama
-        Proxy adresinizi aşağıdaki gibi `proxies` parametresi ile tanımlayabilirsiniz. Ayrıca `httpsVerify` parametresi ile https kontrolünü devre dışı bırakabilirsiniz.
-        ```
-        proxies = { "https" : "HTTPS_PROXY_URL"}
-        evds = evdsAPI('EVDS_API_ANAHTARI', proxies=proxies, httpsVerify=False)
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# EVDS
+
+[English](https://github.com/fatihmete/evds/blob/master/README_EN.md)
+
+EVDS paketi EVDS-API üzerinden Türkiye Cumhuriyet Merkez Bankası (TCMB) tarafından Elektronik Veri Dağıtım Sistemi (EVDS) aracılığıyla yayımlanan tüm istatistiki verilere python aracılığıyla erişmenize imkan sağlar.
+
+EVDS paketi resmi bir paket olmayıp açık kaynak kodlu olarak geliştirilmektedir.
+
+## Kurulum
+
+evds paketini pip paket yöneticisi aracılığıyla kurabilirsiniz:
+
+```
+pip install evds --upgrade
+```
+
+## Yenilikler
+
+0.3 sürümü ile aşağıdaki değişiklikler yapıldı:
+
+1. SSL hatalarının giderilmesi için legacySSL parametresi eklendi. [PR #8](https://github.com/fatihmete/evds/pull/8)
+2. Kod içerisinde düzeltmeler yapıldı. [PR #6](https://github.com/fatihmete/evds/pull/6) [PR #4](https://github.com/fatihmete/evds/pull/4)
+3. request session'un açık kalması nedeniyle ortaya çıkan ResourceWarning uyarısı giderildi. [PR #4](https://github.com/fatihmete/evds/pull/4)
+4. Pandas DataFrame numeric tiplere cast ederken ortaya çıkan FutureWarning uyarıları çıkıyordu. Bu sorun giderildi. [PR #9](https://github.com/fatihmete/evds/pull/9)
+
+0.2 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
+
+1. `get_data`, `get_sub_categories` ve `get_series` fonksiyonlarına, `raw` parametresi eklendi. Bu parametre `True` olarak tanımlandığında ilgili verilere dictionary formatında erişebilirsiniz.
+2. Çeşitli hatalar giderildi.
+
+0.1.1 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
+
+1. formulas parametresindeki hata giderildi.
+
+0.1.0 sürümü ile birlikte aşağıdaki özellikler eklenmiştir:
+
+1. API üzerinden erişilemeyen serilere ilişkin EVDS'de yapılan güncellemeye paralel olarak tüm serilere erişim olanağı sağlanmıştır.
+2. Proxy desteği eklenmiştir.
+3. Küçük hatalar giderildi
+
+## Kullanım
+
+Örnek kullanım, 01-01-2019 - 01-01-2020 arası USD ve EUR alış kurlarına aşağıdaki şekilde erişilebilir.
+
+```python
+from evds import evdsAPI
+evds = evdsAPI('EVDS_API_ANAHTARI')
+evds.get_data(['TP.DK.USD.A.YTL','TP.DK.EUR.A.YTL'], startdate="01-01-2019", enddate="01-01-2020")
+```
+
+get_data fonksiyonu DataFrame return edecektir. İstenmesi halinde `raw=True` parametresi ile dictionary formatında ham veriye ulaşılabilir.
+
+### API Anahtarı Alma
+
+evds paketini kullanmak için öncelikle EVDS sistemi üzerinden API Anahtarı almanız gerekmektedir. API Anahtarı almak için aşağıdaki adımları izleyiniz:
+
+1. [EVDS](https://evds2.tcmb.gov.tr/) sayfasına giriş yaptıktan sonra Giriş Yap ve Kayıt Ol bağlantılarını izleyerek bir EVDS hesabı oluşturun.
+2. Ardından kullanıcı adınızın altında yer alan profil bağlantısına tıklayınız.
+
+![01](01.png)
+
+3. Profil sayfanızın alt kısmında yer alan "API Anahtarı" butonuna tıklayınız ve açılan kutucukta yer alan değeri kopyalayınız.
+
+![02](02.png)
+
+### Detaylı Sorgulama
+
+`get_data` fonksiyonu aşağıdaki parametreleri alır:
+
+#### series
+
+Bu parametre liste olarak tanımlanmalıdır. Ayrıca birden fazla seri bu liste içerisinde tanımlanabilir. Tanımlanması zorunludur.
+
+#### startdate
+
+Seride yer alan verilerin hangi tarihten itibaren seçileceği bu parametre ile belirlenir. Tanımlanması zorunludur.
+
+#### enddate
+
+Eğer seri üzerinde bir aralık seçimi yapılmak isteniyorsa aralığın bitiş tarihi bu parametre ile belirtilir. Tanımlanması ihtiyaridir. Tanımlanmadığı durumda `startdate` değerine eşit olarak tanımlanır.
+
+#### raw
+
+`True` olması halinde fonksiyon talep edilen veriyi DataFrame yerine dictionary return eder.
+Örnek kullanım:
+
+```python
+...
+evds.get_data(['TP.DK.USD.A.YTL','TP.DK.EUR.A.YTL'], startdate="01-01-2019", enddate="01-01-2020", raw=True)
+```
+
+#### aggregation_types
+
+Seri içindeki verilerin getirilmesi esnasında kullanılacak olan toplululaştırma yöntemini ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı yöntem kullanılır. Ayrıca değer olarak string veya liste alabilir. String alması durumunda tüm seriler için aynı yöntem uygulanır. Liste olarak tanımlanırsa `series` parametresinde tanımlanan serilere sırasıyla belirtilen yöntemler uygulanır.
+Kullanılabilecek yöntemler aşağıdaki gibidir:
+
+| Yöntem    | Parametre Değeri |
+| --------- | ---------------- |
+| Ortalama  | avg              |
+| En düşük  | min              |
+| En yüksek | max              |
+| Başlangıç | first            |
+| Bitiş     | last             |
+| Kümülatif | sum              |
+
+#### formulas
+
+Seri içindeki verilerin getirilmesi esnasında uygulanacak formülü ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı formül kullanılır. Ayrıca değer olarak string veya liste alabilir. String alması durumunda tüm seriler için aynı formül uygulanır. Liste olarak tanımlanırsa `series` parametresinde tanımlanan serilere sırasıyla belirtilen formüller uygulanır.
+Kullanılabilecek yöntemler aşağıdaki gibidir:
+
+| Formül                                     | Değer |
+| ------------------------------------------ | ----- |
+| Düzey (Öntanımlı)                          | 0     |
+| Yüzde Değişim                              | 1     |
+| Fark                                       | 2     |
+| Yıllık Yüzde Değişim                       | 3     |
+| Yıllık Fark                                | 4     |
+| Bir Önceki Yılın Sonuna Göre Yüzde Değişim | 5     |
+| Bir Önceki Yılın Sonuna Göre Fark          | 6     |
+| Hareketli Ortalama                         | 7     |
+| Hareketli Toplam                           | 8     |
+
+API formula parametresi uygulandığında orijinal değerleri `None` olarak yanıtladığı için, formula parametresi tanımladığınız serinin orijinal değerlere ulaşmak için aynı seriyi tekrar ekleyiniz ve formula parametresini 0 olarak tanımlayınız. Örneğin
+
+```python
+evds.get_data(['TP.DK.USD.A.YTL','TP.DK.USD.A.YTL'],
+              startdate="01-01-2019",
+              enddate="01-01-2020",
+              formulas=[1,0],
+                )
+```
+
+USD için yüzde değişim ve orijinal değerlere aynı anda yukarıdaki gibi ulaşabilirsiniz.
+
+#### frequency
+
+Seri içerisinde yer alan verilerin hangi sıklıkla getireceğini ifade eder. Tanımlanması ihtiyaridir. Eğer tanımlanmamışsa seri için tanımlanan öntanımlı yayımlanma sıklığı kullanılır.Aşağıdaki değerleri alabilir.
+
+| Sıklık     | Değer |
+| ---------- | ----- |
+| Günlük     | 1     |
+| İşgünü     | 2     |
+| Haftalık   | 3     |
+| Ayda 2 Kez | 4     |
+| Aylık      | 5     |
+| 3 Aylık    | 6     |
+| 6 Aylık    | 7     |
+| Yıllık     | 8     |
+
+## Mevcut Serileri Listeleme
+
+EVDS üzerinde veri serileri sırasıyla Ana Kategori, Alt Kategori ve Seri hiyerarşisinde sunulmaktadır.
+
+> `get_data` fonksiyonun kullanılması için aşağıda yer alan işlemlerin gerçekleştirilmesine gerek yoktur. Veri serisine ait kodun bilinmesi durumunda doğrudan `get_data` fonksiyonu kullanılabilir.
+
+### Ana kategorileri listeleme
+
+`main_categories` değişkeni ile ana kategorileri listeleyebilirsiniz.
+
+```python
+...
+evds.main_categories
+```
+
+komut ile ana kategorileri listeleyebilirsiniz.
+
+| CATEGORY_ID | TOPIC_TITLE_TR               |
+| ----------- | ---------------------------- |
+| 1           | PİYASA VERİLERİ              |
+| 2           | KURLAR                       |
+| 3           | FAİZ İSTATİSTİKLERİ          |
+| 4           | PARA VE BANKA İSTATİSTİKLERİ |
+| ...         | ...                          |
+
+### Alt kategorileri listeleme
+
+Ana kategori altında yer alan alt kategorilere aşağıdaki şekilde ulaşabilirsiniz. Ayrıca `raw=True` parametresi ile DataFrame yerine dictionary formatında alt kategorileri ulaşılabilir.
+
+```python
+evds.get_sub_categories('Ana kategori ID'si veya Adı')
+```
+
+Örnek kulllanım;
+
+```python
+...
+evds.get_sub_categories(6)
+```
+
+| CATEGORY_ID | DATAGROUP_CODE | DATAGROUP_NAME                                    |
+| ----------- | -------------- | ------------------------------------------------- |
+| 6           | bie_dbafod     | Dış Borç Anapara ve Faiz Ödemeleri ile Diğer T... |
+| 6           | bie_dbdborc    | Dış Borçlar-Brüt (Hazine ve Maliye Bakanlığı)     |
+| 6           | bie_kvdbs      | Kısa Vadeli Dış Borç Stoku (milyon ABD doları)    |
+| 6           | bie_yssk       | Özel Sektörün Yurt Dışından Sağladığı Uzun Vad... |
+
+Yukarıda yer alan örnekte 6'nolu kategori altında yer alan alt kategoriler listelenmiştir. Ayrıca `get_sub_categories` fonksiyonunda CATEGORY_ID yerine doğrudan ana kategori adı ile kullanabilirsiniz. Örneğin
+
+```python
+...
+evds.get_sub_categories("KURLAR")
+```
+
+### Serileri listeleme
+
+Alt kategori altında yer alan veri serilerine aşağıdaki şekilde ulaşabilirsiniz. Ayrıca `raw=True` parametresi ile DataFrame yerine dictionary formatında serilere ulaşılabilir.
+
+```python
+evds.get_series('Alt kategori adı')
+```
+
+Örnek kulllanım;
+
+```
+...
+evds.get_series('bie_dbdborc')
+```
+
+| SERIE_CODE | SERIE_NAME                            | START_DATE |
+| ---------- | ------------------------------------- | ---------- |
+| TP.DB.B01  | 1:TÜRKİYE BRÜT DIŞ BORÇ STOKU         | 01-10-1989 |
+| TP.DB.B02  | 2:KISA VADELİ BORÇLAR (Borçluya Göre) | 01-10-1989 |
+| TP.DB.B03  | 2A:KAMU (Borçluya Göre)               | 01-10-1989 |
+| TP.DB.B04  | 2A1:GENEL YÖNETİM (Borçluya Göre)     | 01-10-1989 |
+| TP.DB.B05  | 2A1a:Merkezi Yönetim                  | 01-10-1989 |
+
+`get_data()` fonksiyonu aracılığıyla SERIE_CODE'u kullanarak serilere ait verilere ulaşabilirsiniz.
+
+## Proxy Tanımlama
+
+Proxy adresinizi aşağıdaki gibi `proxies` parametresi ile tanımlayabilirsiniz. Ayrıca `httpsVerify` parametresi ile https kontrolünü devre dışı bırakabilirsiniz.
+
+```
+proxies = { "https" : "HTTPS_PROXY_URL"}
+evds = evdsAPI('EVDS_API_ANAHTARI', proxies=proxies, httpsVerify=False)
+```
+
+## SSLError Hatası çözümü
+
+Sunucu sertifikası ve kullanılan python paketlerinden kaynaklı olarak SSL hatası alınabilmektedir. Bu hata durumunda legacySSL parametresi kullanılabilir:
+
+```
+evds = evdsAPI('EVDS_API_ANAHTARI', legacySSL=True)
+
+```
```

