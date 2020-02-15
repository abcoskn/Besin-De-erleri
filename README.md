# Besin-De-erleri Documentation


# Besin Arama

POST URL: https://www.abctasarim.net/diyet/search.php

# Post Parametreleri

| Parametre  | Tip  | Gerekli | Açıklama |
| ---------- | ------ | --------- | --------- |
| keyword	| String	| Evet | Arama Kelimesi |



# Cevap Parametreleri

| Parametre  | Açıklama  |
| ---------- | ------ |
| img | Besin Resmi |
| name | Besin Adı |
| src | Detay Linki (Detay sayfasına post edilecek link)  |
| unit | Ölçü |
| cal | Kalori |



# Detaylı Besin İçerikleri

POST URL: https://www.abctasarim.net/diyet/get.php

# Post Parametreleri

| Parametre  | Tip  | Gerekli | Açıklama |
| ---------- | ------ | --------- | --------- |
| link	| String	| Evet | search servisinden dönen link değeri |



# Cevap Parametreleri

| Parametre  | Tip  |  Açıklama  |
| ---------- | ------ |
| name | String | Besin Adı |
| img | String | Besin Resmi |
| units | Array[] | Ölçü Dizisi |

| Değer  | Tip  |  Açıklama  |
| ---------- | ------ |
| name | String | Ölçü |
| values | Array[] | Ölçüye ait besin değerleri |

| Değer  | Tip  |  Açıklama  |
| ---------- | ------ |
| amount | Float | Ağırlık |
| calcium | Float | Kalsiyum |
| calory | Float | Kalori |
| carbohydrt | Float | Karbonhidrat |
| cholestrl | Float | Kolestrol |
| fiber_td | Float | Lif |
| iron | Float | Demir |
| lipid_tot | Float | Food |
| potassium | Float | Potasyum |
| protein | Float | Protein |
| sodium | Float | Sodyum |
| units_id | int | Ölçü ID |
| vit_a_iu | Float | Vitamin A |
| vit_c | Float | Vitamin C |


