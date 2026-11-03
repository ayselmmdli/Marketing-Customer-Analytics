# Business Insights Report

**Layihə:** Marketing & Customer Analytics  
**Mənbə:** Tableau dashboardlarında müşahidə olunan yekun rəqəmlər  
**Status:** İlkin biznes şərhi; Python–Tableau yekun reconciliation hələ təsdiqlənməyib.

## 1. Executive Summary

Məlumat dəsti **2,240 müştərini** əhatə edir. Müştərilərin cəmi xərcləməsi **1,356,988**, kanal ölçüləri üzrə alış sayı **28,083**, ümumi orta müştəri xərcləməsi isə **605.8**-dir. Son kampaniyaya **334 müştəri** müsbət cavab verib (**14.9%**). Məhsul xərcləməsi bir neçə kateqoriyada cəmlənir; müştəri seqmentləri və gəlir qrupları arasında kampaniya cavab faizi nəzərəçarpacaq fərqlənir.

**Əsas biznes fürsəti:** RFM və gəlir seqmentlərinə görə kiçik, ölçülə bilən kampaniya testləri aparmaq; nəticəni ümumi cavab sayı ilə deyil, kampaniya çatdırılma və gəlir məlumatları əlavə ediləndən sonra dəqiq performans ölçüləri ilə qiymətləndirmək.

## 2. Ümumi göstəricilər

| KPI | Dəyər | Şərh |
|---|---:|---|
| Total Customers | 2,240 | Təhlil edilən baza |
| Total Spending | 1,356,988 | Müştərilərin ümumi xərcləməsi |
| Total Purchases | 28,083 | Üç kanal üzrə alış saylarının cəmi |
| Average Spending | 605.8 | Müştəri üzrə orta xərcləmə |
| Campaign Responders | 334 | Son kampaniyaya müsbət cavab verənlər |
| Campaign Response Rate | 14.9% | 334 / 2,240 |
| Previous Campaign Acceptances | 667 | Beş əvvəlki kampaniyanın qəbul hadisələri cəmi |
| Average Spending — Responders | 987.4 | Cavab verən müştərilərin orta xərcləməsi |
| Complaint Rate | 0.9% | Şikayət göstəricisi |
| Flagged Customers | 7 | Data keyfiyyəti baxımından yoxlanmalı qeydlər |

## 3. Məhsul kateqoriyaları

| Kateqoriya | Xərcləmə | Ümumi xərcləmədə pay |
|---|---:|---:|
| Wines | 680,816 | 50.2% |
| Meat Products | 373,968 | 27.6% |
| Gold Products | 98,609 | 7.3% |
| Fish Products | 84,057 | 6.2% |
| Sweet Products | 60,621 | 4.5% |
| Fruits | 58,917 | 4.3% |

**Insight:** Wines və Meat Products birlikdə ümumi xərcləmənin təxminən **77.7%-ni** yaradır. Kateqoriya konsentrasiyası yüksəkdir.

**Tövsiyə:**

1. Ən çox xərcləmə olan kateqoriyalar üçün stok mövcudluğu və təkrar alış davranışını izləyin.
2. Digər kateqoriyaların satış potensialını səbət analizi və kontrollu cross-sell testləri ilə yoxlayın.
3. Xərcləmə payını mənfəət payı ilə eyniləşdirməyin; qiymət və maya dəyəri daxil edilmədən rentabellik bilinmir.

## 4. Alış kanalları

| Kanal | Alış sayı | Pay |
|---|---:|---:|
| Store | 12,970 | 46.2% |
| Web | 9,150 | 32.6% |
| Catalog | 5,963 | 21.2% |

**Insight:** Fiziki mağaza say etibarilə liderdir; veb alışlar da əhəmiyyətli həcmdədir.

**Tövsiyə:** Hər kanal üçün ayrıca alış tezliyi, orta sifariş dəyəri, geri dönüş və müştəri saxlama göstəricilərini hesablayın. Yalnız alış sayına əsasən hansı kanalın daha gəlirli olduğu müəyyən edilə bilməz.

## 5. RFM müştəri seqmentləri

| Seqment | Müştəri sayı | Baza payı | Kampaniyaya cavab faizi |
|---|---:|---:|---:|
| Low Engagement | 755 | 33.7% | 13.4% |
| Potential Loyalists | 517 | 23.1% | 4.4% |
| At Risk | 402 | 17.9% | 30.1% |
| Champions | 329 | 14.7% | 15.5% |
| Loyal Customers | 230 | 10.3% | 16.5% |
| Needs Review / No Record | 7 | 0.3% | 0.0% |

**Insight 1:** **At Risk** qrupunda cavab faizi (**30.1%**) ən yüksəkdir. Bu qrup üçün geri-qazanma (win-back) kampaniyası test edilməyə dəyər.

**Insight 2:** **Potential Loyalists** böyük qrupdur (**517 nəfər**), lakin cavab faizi **4.4%**-dir. Mesaj, kanal və təklif uyğunluğunun yoxlanması üçün prioritet namizəddir.

**Tövsiyə:**

- At Risk: A/B test ilə fərdiləşdirilmiş geri-qazanma təklifləri.
- Champions / Loyal Customers: loyallıq və təkrar alış ssenariləri.
- Potential Loyalists: auditoriya tərifi, təklif və əlaqə vaxtını test edin.

**Vacib:** Qruplararası fərq səbəb-nəticə sübutu deyil. Auditoriyanın kampaniyaya məruz qalma sayı məlum olmadığı üçün nəticələr müşahidə olunan müsbət cavab paylarıdır.

## 6. Demoqrafik profil

| Göstərici | Nəticə |
|---|---:|
| Orta müştəri yaşı | 45.2 |
| Orta household income | 52,247 |
| Uşağı olan müştərilər | 71.5% |
| Ən böyük yaş qrupu | 35–44 (740 müştəri) |
| Ən böyük təhsil qrupu | Graduate (1,127 müştəri) |
| Yaş qrupu `Null` | 3 |
| Gəlir qrupu `Null` | 24 |

**Insight:** Müştəri profilinin əsas hissəsi orta yaş qruplarında cəmlənir. Müştərilərin böyük hissəsində uşaqların olması ailə yönümlü təkliflərin sınağı üçün hipotez yaradır.

**Tövsiyə:** Yaş və ailə strukturu üzrə fərqli kreativ və təklifləri ayrıca test edin; nəticəni təsadüfi seçilmiş kontrol qrupu ilə müqayisə edin.

## 7. Kampaniya analizi

### Əvvəlki kampaniyaların qəbul sayı

| Kampaniya | Qəbul sayı |
|---|---:|
| AcceptedCmp1 | 144 |
| AcceptedCmp2 | 30 |
| AcceptedCmp3 | 163 |
| AcceptedCmp4 | 167 |
| AcceptedCmp5 | 163 |
| **Cəmi qəbul hadisəsi** | **667** |
| Son kampaniya — Response | 334 |

**Qeyd:** 667 qəbul hadisəsi eyni müştərini bir neçə dəfə əhatə edə bilər. Kampaniyaların göndərilmə həcmi, dövrü və büdcəsi olmadan birini digəri ilə səmərəlilik baxımından müqayisə etmək düzgün deyil.

### Gəlir qrupuna görə kampaniya cavab faizi

| Gəlir qrupu | Cavab faizi |
|---|---:|
| High Income | 26.9% |
| Lower-Middle Income | 12.5% |
| Low Income | 10.5% |
| Upper-Middle Income | 10.3% |
| Null | 4.2% |

**Insight:** High Income qrupunun müşahidə olunan cavab faizi **26.9%** olub və ümumi bazadakı **14.9%** səviyyəsindən yüksəkdir. Bu, hədəfləmə hipotezidir; mütləq ROI üstünlüyü demək deyil.

**Responders spending:** Cavab verən müştərilərin orta xərcləməsi **987.4**, ümumi baza üzrə **605.8**-dir — təxminən **63.0%** daha yüksək. Yüksək xərcləyənlərin kampaniyaya daha meyilli olması mümkündür; kampaniyanın xərcləməni artırdığını bu göstərici ilə sübut etmək olmaz.

## 8. Prioritetləşdirilmiş fəaliyyət planı

| Prioritet | Təklif | Necə ölçmək olar? |
|---|---|---|
| P1 | At Risk qrupu üçün kontrollu win-back pilotu | Çatdırılmış mesajlar, müsbət cavab, incremental purchases |
| P1 | Kampaniya exposure, xərc və tarix məlumatlarını birləşdirmək | Conversion rate, CPA, ROAS, uplift |
| P1 | 7 işarələnmiş müştəri qeydini ayrıca yoxlamaq | Açıq data keyfiyyəti problemləri sayı |
| P2 | High Income qrupunda təklif/kreativ testi | Qrupdaxili test-control fərqi |
| P2 | Potential Loyalists üçün mesaj və kanal testi | Cavab faizi və təkrar alış |
| P2 | Kanal və kateqoriya üzrə gəlirlilik ölçməsini qurmaq | Marja və mənfəət (əlavə data ilə) |

## 9. Data keyfiyyəti və məhdudiyyətlər

1. Dashboardda **7 flagged customer** göstərilir. Mənbə qeydlərinə görə `NumDealsPurchases > Total Purchases` qaydasını pozan **3**, `Total Purchases = 0` olduğu halda `Total Spending > 0` olan **6** qeyd var; **2** qeyd kəsişdiyi üçün unikal flag sayı **7**-dir. Bu qaydalar yekun kodla yenidən təsdiqlənməlidir.
2. Yaş qrupunda **3**, gəlir qrupunda **24** boş/qrupa düşməyən qeyd mövcuddur.
3. Dörd gəlir qrupunun hərəsində **554 müştəri** görünür. Qrupların bərabərliyi kvantil bölgüsünə uyğun ola bilər, lakin təsdiq üçün preprocessing koduna baxılmalıdır.
4. Kampaniya göndərilmə/çatdırılma məlumatları yoxdur; **334/2,240** həqiqi göndərilmə əsaslı dönüşüm faizi kimi göstərilməməlidir.
5. Məbləğlərin valyutası, müşahidə dövrü, məhsul maya dəyəri və reklam xərcləri təsdiqlənməyib.
6. Python notebook-un CSV fayl yolunda `FileNotFoundError` yaşandığı üçün Python–Tableau yekun rəqəm tutuşdurması **hələ təsdiq edilməyib**.

## 10. Nəticə

Ən aydın imkanlar: **risk altındakı müştərilərin aktivləşdirilməsi**, **yüksək gəlir seqmentində hədəfli testlər** və **məhsul/kanal konsentrasiyasının dərinləşdirilmiş analizi**. Növbəti mərhələdə məqsəd bu müşahidələri test edilə bilən hipotezlərə çevirmək və kampaniyaların real əlavə təsirini hesablamaqdır.
