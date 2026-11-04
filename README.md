# Marketing & Customer Analytics | Tableau Portfolio Project

> **EN:** An end-to-end customer analytics portfolio project covering data preparation, RFM customer segmentation, demographics, campaign response analysis, and interactive Tableau dashboards.

Bu layihənin məqsədi müştəri davranışlarını, alış kanallarını, məhsul kateqoriyalarını və marketinq kampaniyalarına reaksiyaları analiz edərək məlumatlara əsaslanan biznes qərarları üçün praktik nəticələr təqdim etməkdir.

### Canlı interaktiv dashboard

**[▶ Tableau Public-də Marketing & Customer Analytics dashboardunu aç](https://public.tableau.com/app/profile/aysel.m.mm.dli/viz/MarketingCustomerAnalytics_17937073779890/01_Executive_Overview)**

GitHub mənbə faylları: [Marketing-Customer-Analytics repository](https://github.com/ayselmmldi/Marketing-Customer-Analytics).

## Layihəyə ümumi baxış

| Göstərici | Nəticə |
|---|---:|
| Müştəri sayı | 2,240 |
| Ümumi müştəri xərcləməsi | 1,356,988 |
| Ümumi alış sayı (kanallar üzrə) | 28,083 |
| Bir müştəriyə orta xərcləmə | 605.8 |
| Son kampaniyaya müsbət reaksiya verənlər | 334 |
| Kampaniya cavab faizi | 14.9% |
| Data keyfiyyəti yoxlamasında işarələnən müştərilər | 7 |

**Qeyd:** Məbləğlərin valyutası mənbə məlumatında təsdiqlənməyib; buna görə pul vahidi əlavə edilmir. Xərcləmə göstəriciləri mənfəət və ya kampaniya gəliri kimi şərh edilməməlidir.

## Məqsədlər və biznes sualları

1. Müştərilər hansı RFM (Recency, Frequency, Monetary) seqmentlərində cəmlənir?
2. Hansı məhsul kateqoriyaları və alış kanalları daha böyük paya malikdir?
3. Yaş, gəlir və təhsil qruplarına görə müştəri profili necə dəyişir?
4. Hansı müştəri seqmentlərində kampaniyaya cavab faizi daha yüksəkdir?
5. Məlumat keyfiyyəti ilə bağlı hansı qeydlər analitik nəticələrə təsir edə bilər?

## Texnologiyalar

- **Python / Pandas** — məlumatların hazırlanması, xüsusiyyətlərin yaradılması və yoxlama.
- **CSV** — Tableau üçün təmizlənmiş məlumat mənbəyi (`marketing_data_rfm.csv`).
- **Tableau** — interaktiv dashboard, filtrlər və səhifələrarası keçid.
- **GitHub** — layihənin sənədləşdirilməsi və portfolio təqdimatı.

## Dashboard səhifələri

| Səhifə | Məzmun |
|---|---|
| **01 — Executive Overview** | Müştəri sayı, ümumi xərcləmə, alış sayı, məhsul kateqoriyaları və alış kanalları |
| **02 — Customer Segmentation** | RFM seqmentlərinin bölgüsü, yüksək dəyərli və risk altındakı müştərilər |
| **03 — Customer Demographics** | Yaş, gəlir, təhsil, uşaqlı müştərilər və orta gəlir |
| **04 — Marketing Campaign Analysis** | Kampaniya cavab faizi, əvvəlki kampaniya qəbulları, RFM və gəlir qrupu üzrə reaksiya |

Dashboardlarda **Age Group**, **Income Group** və **Country** filtrləri, həmçinin **Overview / Segmentation / Demographics / Campaigns** naviqasiya düymələri nəzərdə tutulub.

## Əsas tapıntılar

- **Wines** kateqoriyası ümumi xərcləmənin təxminən **50.2%-ni** təşkil edir.
- **Wines + Meat Products** birlikdə ümumi xərcləmənin təxminən **77.7%-ni** əhatə edir.
- **Store** kanalı alışların təxminən **46.2%-ni**, **Web** isə **32.6%-ni** təşkil edir.
- **At Risk** RFM seqmentində kampaniya cavab faizi **30.1%** göstərilir; bu, hədəflənmiş geri-qazanma testi üçün potensial siqnaldır.
- **High Income** qrupunun kampaniya cavab faizi **26.9%**-dir.
- Kampaniyaya cavab verənlərin orta xərcləməsi **987.4**, ümumi müştəri orta göstəricisi isə **605.8**-dir. Bu fərq səbəb-nəticə əlaqəsini sübut etmir.

Ətraflı şərh, prioritetləşdirilmiş təkliflər və məhdudiyyətlər: [Business Insights](reports/BUSINESS_INSIGHTS.md).

## Repository strukturu

```text
Marketing-Customer-Analytics/
├── README.md
├── 02_Data_Understanding/
│   └── 01_Data_Profiling.ipynb
├── 03_Data_Cleaning/
│   └── 01–06_*.ipynb
├── 04_EDA/
│   └── 01–09_*.ipynb
├── data/
│   ├── marketing_data_clean.csv
│   ├── marketing_data_rfm.csv
│   └── data_quality_report.xlsx
├── tableau/
│   └── Marketing_Customer_Analytics.twbx
├── images/
│   └── 4 dashboard ekran görüntüsü
└── reports/
    └── BUSINESS_INSIGHTS.md
```

Notebook qovluqları GitHub-da layihənin kökündə, orijinal nömrələnmə ilə saxlanılır. Digər fayl və qovluqların yerləşməsi yükləmə tamamlandıqdan sonra yoxlanmalıdır. `.twb` faylı təkbaşına məlumat mənbəyini ehtiva etməyə bilər; paylaşarkən `.twbx` paketini yoxlayın.

## Reproduksiya və yoxlama

1. Lokal layihədə `marketing_data_rfm.csv` faylının yerləşdiyi qovluğu dəqiqləşdirin.
2. Python notebook-un istifadə etdiyi yolu yoxlayın: `Path.cwd()` və `file_path.resolve()`.
3. Məlumatın sətir sayı (**2,240**), əsas sütunları, boş dəyərləri və təkrarlanan müştəri ID-lərini yoxlayın.
4. Python nəticələrini Tableau KPI-ları ilə **eyni filtr şərtlərində** tutuşdurun.
5. Tableau workbook-u açın, dörd dashboardu, filtrləri və naviqasiya keçidlərini test edin.
6. Şəxsi məlumatları silin və ya anonimləşdirin; yalnız paylaşım icazəsi olan məlumat və vizualları yayımlayın.

**Validasiya statusu:** Lokal Python yoxlamasında CSV üçün `FileNotFoundError` müşahidə olunub. Fayl yolu düzəldilib yekun reconciliation nəticələri təsdiqlənənədək bu layihənin tam texniki validasiyası **tamamlanmış hesab edilmir**.

## Məlumat keyfiyyəti və metodoloji məhdudiyyətlər

- **7 müştəri** bir və ya bir neçə data-keyfiyyət qaydasına görə işarələnib; bu qeydlər avtomatik silinməməlidir.
- Yaş qrupunda **3**, gəlir qrupunda **24** `Null` müşahidə olunur.
- **Previous Campaign Acceptances = 667** beş kampaniya üzrə müsbət cavabların **cəmi**dir; 667 unikal müştəri demək deyil.
- Kampaniyaların göndərildiyi/çatdığı auditoriya ayrıca məlum olmadığı üçün `Campaign Response Rate` bu datasetdə **334 / 2,240** əsasında verilir; həqiqi exposure-based conversion rate deyil.
- `Income Group` ölçüsündə qeydə alınan dörd qrupun hərəsində 554 müştəri var; qruplaşdırma qaydasını koddan təsdiqləmədən təbii bazar bölgüsü kimi yozmaq olmaz.
- Tarix intervalı, məbləğ valyutası və kampaniya xərcləri təsdiqlənmədiyindən ROI/ROAS barədə nəticə çıxarılmır.

## Portfolio təqdimatı

- **Tableau Public:** [Marketing & Customer Analytics — Executive Overview](https://public.tableau.com/app/profile/aysel.m.mm.dli/viz/MarketingCustomerAnalytics_17937073779890/01_Executive_Overview)
- **GitHub:** [ayselmmldi/Marketing-Customer-Analytics](https://github.com/ayselmmldi/Marketing-Customer-Analytics)

## İstifadə qeydi

Məlumat mənbəyinin lisenziyası və paylaşım hüquqları ayrıca təsdiqlənməlidir. Bu repository-yə real şəxsi məlumatlar və məxfi məlumatlar yüklənməməlidir.
