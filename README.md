# Besin Değerleri Dökümantasyon


# Besin Arama

POST URL: https://www.abctasarim.net/diyet/search.php

## Post Parametreleri

| Parametre  | Tip  | Gerekli | Açıklama |
| ---------- | ------ | --------- | --------- |
| keyword	| String	| Evet | Arama Kelimesi |



## Cevap Parametreleri

| Parametre  | Açıklama  |
| ---------- | ------ |
| img | Besin Resmi |
| name | Besin Adı |
| src | Detay Linki (Detay sayfasına post edilecek link)  |
| unit | Ölçü |
| cal | Kalori |

## Örnek

```
[
    {
        "img": "https://www.diyetkolik.com/site_media/media/nutrition_images/yulaf.jpg",
        "name": "Yulaf",
        "src": "https://www.diyetkolik.com/kac-kalori/yulaf/",
        "size": "1 Porsiyon (Orta) ",
        "cal": "351 kcal"
    },
    {
        "img": "https://www.diyetkolik.com/site_media/media/nutrition_images/yulaf-kepegi.jpg",
        "name": "Yulaf Kepeği",
        "src": "https://www.diyetkolik.com/kac-kalori/yulaf-kepegi/",
        "size": "1 Çorba Kaşığı ",
        "cal": "35 kcal"
    },
    {
        "img": "https://www.diyetkolik.com/site_media/media/nutrition_images/yulaf-unu.jpg",
        "name": "Yulaf Unu",
        "src": "https://www.diyetkolik.com/kac-kalori/yulaf-unu/",
        "size": "1 Paket ",
        "cal": "3530 kcal"
    },
    {
        "img": "https://www.diyetkolik.com/site_media/media/nutrition_images/yulaf-ezmesi.jpg",
        "name": "Yulaf Ezmesi",
        "src": "https://www.diyetkolik.com/kac-kalori/yulaf-ezmesi/",
        "size": "1 Çorba Kaşığı ",
        "cal": "39 kcal"
    },
    {
        "img": "https://www.diyetkolik.com/site_media/media/nutrition_images/yulaflapas.jpg",
        "name": "Yulaf Lapası",
        "src": "https://www.diyetkolik.com/kac-kalori/yulaf-lapasi/",
        "size": "1 Porsiyon (Orta) ",
        "cal": "100 kcal"
    }
]

```

# Detaylı Besin İçerikleri

POST URL: https://www.abctasarim.net/diyet/get.php

## Post Parametreleri

| Parametre  | Tip  | Gerekli | Açıklama |
| ---------- | ------ | --------- | --------- |
| link	| String	| Evet | search servisinden dönen link değeri |



## Cevap Parametreleri

| Parametre  | Tip  |  Açıklama  |
| ---------- | ------ | ------ |
| name | String | Besin Adı |
| img | String | Besin Resmi |
| units | Array | Ölçü Dizisi |

### Units Dizisi
| Değer  | Tip  |  Açıklama  |
| ---------- | ------ | ------ |
| name | String | Ölçü |
| values | Array | Ölçüye ait besin değerleri |

### Values Dizisi
| Değer  | Tip  |  Açıklama  |
| ---------- | ------ | ------ |
| amount | Float | Ağırlık (gr) |
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

## Örnek

```

{
    "name": "Elma",
    "img": "https://www.diyetkolik.com/site_media/media/nutrition_images/elma.jpg",
    "units": [
        {
            "unit": "Adet",
            "data": {
                "amount": "90.0000",
                "calcium": "5.4",
                "calory": "46.8",
                "carbohydrt": "12.429",
                "cholestrl": "0.0",
                "fiber_td": "2.16",
                "iron": "0.108",
                "lipid_tot": "0.153",
                "potassium": "96.3",
                "protein": "0.234",
                "sodium": "0.9",
                "units_id": "2",
                "vit_a_iu": "48.6",
                "vit_c": "4.14"
            }
        },
        {
            "unit": "Adet (Büyük)",
            "data": {
                "amount": "150.0000",
                "calcium": "9.0",
                "calory": "78.0",
                "carbohydrt": "20.715",
                "cholestrl": "0.0",
                "fiber_td": "3.6",
                "iron": "0.18",
                "lipid_tot": "0.255",
                "potassium": "160.5",
                "protein": "0.39",
                "sodium": "1.5",
                "units_id": "3",
                "vit_a_iu": "81.0",
                "vit_c": "6.9"
            }
        },
        {
            "unit": "Adet (Orta)",
            "data": {
                "amount": "100.0000",
                "calcium": "6.0",
                "calory": "52.0",
                "carbohydrt": "13.81",
                "cholestrl": "0.0",
                "fiber_td": "2.4",
                "iron": "0.12",
                "lipid_tot": "0.17",
                "potassium": "107.0",
                "protein": "0.26",
                "sodium": "1.0",
                "units_id": "6",
                "vit_a_iu": "54.0",
                "vit_c": "4.6"
            }
        },
        {
            "unit": "Adet (Küçük)",
            "data": {
                "amount": "90.0000",
                "calcium": "5.4",
                "calory": "46.8",
                "carbohydrt": "12.429",
                "cholestrl": "0.0",
                "fiber_td": "2.16",
                "iron": "0.108",
                "lipid_tot": "0.153",
                "potassium": "96.3",
                "protein": "0.234",
                "sodium": "0.9",
                "units_id": "5",
                "vit_a_iu": "48.6",
                "vit_c": "4.14"
            }
        },
        {
            "unit": "Porsiyon (Orta)",
            "data": {
                "amount": "120.0000",
                "calcium": "7.2",
                "calory": "62.4",
                "carbohydrt": "16.572",
                "cholestrl": "0.0",
                "fiber_td": "2.88",
                "iron": "0.144",
                "lipid_tot": "0.204",
                "potassium": "128.4",
                "protein": "0.312",
                "sodium": "1.2",
                "units_id": "121",
                "vit_a_iu": "64.8",
                "vit_c": "5.52"
            }
        },
        {
            "unit": "Yarım (Orta Boy)",
            "data": {
                "amount": "50.0000",
                "calcium": "3.0",
                "calory": "26.0",
                "carbohydrt": "6.905",
                "cholestrl": "0.0",
                "fiber_td": "1.2",
                "iron": "0.06",
                "lipid_tot": "0.085",
                "potassium": "53.5",
                "protein": "0.13",
                "sodium": "0.5",
                "units_id": "169",
                "vit_a_iu": "27.0",
                "vit_c": "2.3"
            }
        },
        {
            "unit": "Dilim (Büyük)",
            "data": {
                "amount": "30.0000",
                "calcium": "1.8",
                "calory": "15.6",
                "carbohydrt": "4.143",
                "cholestrl": "0.0",
                "fiber_td": "0.72",
                "iron": "0.036",
                "lipid_tot": "0.051",
                "potassium": "32.1",
                "protein": "0.078",
                "sodium": "0.3",
                "units_id": "57",
                "vit_a_iu": "16.2",
                "vit_c": "1.38"
            }
        },
        {
            "unit": "Dilim (Orta)",
            "data": {
                "amount": "20.0000",
                "calcium": "1.2",
                "calory": "10.4",
                "carbohydrt": "2.762",
                "cholestrl": "0.0",
                "fiber_td": "0.48",
                "iron": "0.024",
                "lipid_tot": "0.034",
                "potassium": "21.4",
                "protein": "0.052",
                "sodium": "0.2",
                "units_id": "61",
                "vit_a_iu": "10.8",
                "vit_c": "0.92"
            }
        },
        {
            "unit": "Adet (Rendelenmiş)",
            "data": {
                "amount": "130.0000",
                "calcium": "7.8",
                "calory": "67.6",
                "carbohydrt": "17.953",
                "cholestrl": "0.0",
                "fiber_td": "3.12",
                "iron": "0.156",
                "lipid_tot": "0.221",
                "potassium": "139.1",
                "protein": "0.338",
                "sodium": "1.3",
                "units_id": "243",
                "vit_a_iu": "70.2",
                "vit_c": "5.98"
            }
        },
        {
            "unit": "Dilim (İnce)",
            "data": {
                "amount": "15.0000",
                "calcium": "0.9",
                "calory": "7.8",
                "carbohydrt": "2.0715",
                "cholestrl": "0.0",
                "fiber_td": "0.36",
                "iron": "0.018",
                "lipid_tot": "0.0255",
                "potassium": "16.05",
                "protein": "0.039",
                "sodium": "0.15",
                "units_id": "59",
                "vit_a_iu": "8.1",
                "vit_c": "0.69"
            }
        },
        {
            "unit": "Gram",
            "data": {
                "amount": "1.0000",
                "calcium": "0.06",
                "calory": "0.52",
                "carbohydrt": "0.1381",
                "cholestrl": "0.0",
                "fiber_td": "0.024",
                "iron": "0.0012",
                "lipid_tot": "0.0017",
                "potassium": "1.07",
                "protein": "0.0026",
                "sodium": "0.01",
                "units_id": "187",
                "vit_a_iu": "0.54",
                "vit_c": "0.046"
            }
        }
    ]
}

```


