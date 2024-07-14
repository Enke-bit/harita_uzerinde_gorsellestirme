# Dünya Ülkelerinin Sıcaklık Verileri ile İnteraktif Harita

Bu proje, dünya ülkelerinin belirli tarihlerdeki sıcaklık verilerini interaktif bir harita üzerinde göstermeyi amaçlamaktadır. Kullanılan veri seti, her ülkenin çeşitli sıcaklık kategorilerindeki (örneğin, 'Aşırı Soğuk', 'Orta Soğuk', 'Orta Sıcak', 'Aşırı Sıcak') sıcaklık verilerini içermektedir.

## Kurulum

Projeyi çalıştırmak için aşağıdaki adımları izleyin:

 Gerekli Python kütüphanelerini yükleyin:
    ```bash
    pip install pandas geopy folium
    ```

## Kullanım

1. `main.py` dosyasını çalıştırın:
    ```bash
    python main.py
    ```

2. Oluşturulan harita dosyasını açın:
    - `world_temperature_map.html`

## Proje Detayları

Bu çalışma, dünya ülkelerinin belirli tarihlerdeki sıcaklık verilerini görselleştirmek için interaktif bir harita oluşturur. Projede kullanılan veri seti, ülkelerin sıcaklık kategorilerini içermektedir. Ülkelerin koordinat bilgileri, `geopy` kütüphanesi kullanılarak elde edilmiştir.

### Adımlar:

1. **Veri Setinin İncelenmesi:** Veri seti okunup sütun isimleri ve içeriği incelenmiştir.
2. **Koordinatların Elde Edilmesi:** `geopy` kütüphanesi kullanılarak, her ülkenin enlem ve boylam bilgileri elde edilmiştir.
3. **Haritanın Oluşturulması:** `folium` ve `MarkerCluster` kullanılarak interaktif bir dünya haritası oluşturulmuştur. Haritada her bir ülke, belirli bir sıcaklık değeri ile gösterilmektedir. Kullanıcı bir ülkeye tıkladığında, o ülkenin sıcaklık verileri pop-up olarak görüntülenmektedir.
4. **Haritanın Kaydedilmesi:** Oluşturulan harita, `world_temperature_map.html` dosyası olarak kaydedilmiş ve tarayıcıda görüntülenmek üzere hazırlanmıştır.

## Katkıda Bulunma

Katkıda bulunmak isterseniz lütfen bir pull request gönderin. Her türlü katkı değerlidir!

## Lisans

Bu proje MIT lisansı ile lisanslanmıştır. Daha fazla bilgi için `LICENSE` dosyasına bakın.
