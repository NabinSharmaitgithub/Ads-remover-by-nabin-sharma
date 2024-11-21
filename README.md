# Ads-remover-by-nabin-sharma-
Best android patch with several patches including regex for ads, analytics, etc
# ☣️ Ads remover ☣️
file that helps to remove ads from almost all the apps 


<img src="https://www.google.com/search?client=ms-android-xiaomi-terr1-rso2&sca_esv=41abccaec8fca31d&q=logo+for+ads+removing+app&udm=2&fbs=AEQNm0Aa4sjWe7Rqy32pFwRj0UkWd8nbOJfsBGGB5IQQO6L3JyJJclJuzBPl12qJyPx7ESJehObpS5jg6J88CCM-RK72qUv4GOvBp3LxAsC-35pUAVd1mVJIz_kJEl7OpW0Y42qduZyCIUQvYXF-Rlml4RoqFbNWi5tYNUImDyWlZNODzhRu2wrxbBepXslH0S2cg_2ElVWx&sa=X&ved=2ahUKEwjg17Ls-O2JAxU4dmwGHRlaO6oQtKgLegQIExAB&biw=360&bih=663&dpr=2#vhid=of323WmqUrptMM&vssid=mosaic&ip=1"/>






# Regex 1

search 🔍 

```bash
(\.method\s(public|private|static)\s\b(?!\babstract|native\b)(.*)?loadAd\(.*\)V)
```
replace 

```bash
$1

    return-void
```



# Regex 2

search 🔍 

```bash
(\.method\s(public|private|static)\s\b(?!\babstract|native\b)(.*)?loadAd\(.*\)Z)
```
replace 

```bash
$1

    const/4 v0, 0x0

    return v0
```




# Regex 3

search 🔍 

```bash
(invoke.*loadAd\(.*\)[VZ])
```
replace 

```bash
#$1
```





# Regex 4

search 🔍 

```bash
(invoke.*gms.*\>(loadUrl|loadDataWithBaseURL|requestInterstitialAd|showInterstitial|showVideo|showAd|loadData|onAdClicked|onAdLoaded|isLoading|loadAds|AdLoader|AdRequest|AdListener|AdView).*V)
```
replace 

```bash
#$1
```





# Regex 5

search 🔍 

```bash
\"(http.*|//.*)(61\.145\.124\.238|\-ads\.|\.ad\.|\.ads\.|\.analytics\.localytics\.com|\.mobfox\.com|\.mp\.mydas\.mobi|\.plus1\.wapstart\.ru|\.scorecardresearch\.com|\.startappservice\.com|\/ad\.|\/ads|ad\-mail|ad\.*\_logging|ad\.api\.kaffnet\.com|adc3\-launch|adcolony|adinformation|adkmob|admax|admob|admost|adsafeprotected|adservice|adtag|advert|adwhirl|adz\.wattpad\.com|alta\.eqmob\.com|amazon\-*ads|amazon\.*ads|amobee|analytics|applovin|applvn|appnext|appodeal|appsdt|appsflyer|burstly|cauly|cloudfront|com\.google\.android\.gms\.ads\.identifier\.service\.START|crashlytics|crispwireless|doubleclick|dsp\.batmobil\.net|duapps|dummy|flurry|gad|getads|google\.com\/dfp|googleAds|googleads|googleapis\.*\.ad\-*|googlesyndication|googletagmanager|greystripe|gstatic|inmobi|inneractive|jumptag|live\.chartboost\.com|madnet|millennialmedia|moatads|mopub|native\_ads|pagead|pubnative|smaato|supersonicads|tapas|tapjoy|unityads|vungle|zucks).*\"
```
replace 

```bash
"="
```






# Regex 6

search 🔍 

```bash
ca-app-pub-\d{16}/\d{10}
```
replace 

```bash
ca-app-pub-0000000000000000/0000000000
```






# Regex 7

search 🔍 

```bash
invoke-.*\{.*\}, L.*;->(loadAd|requestNativeAd|showInterstitial|fetchad|fetchads|onadloaded|requestInterstitialAd|showAd|loadAds|AdRequest|requestBannerAd|loadNextAd|createInterstitialAd|setNativeAd|loadBannerAd|loadNativeAd|loadRewardedAd|loadRewardedInterstitialAd|loadAds|loadAdViewAd|showInterstitialAd|shownativead|showbannerad|showvideoad|onAdFailedToLoad)\(.*\)V
```
replace 

```bash
nop
```






# Regex 8

search 🔍 

```bash
invoke-*.* \{*.*\}, Lcom*.*;->requestInterstitialAd\(*.*\)V|invoke-*.* \{*.*\}, Lcom*.*;->loadAds\(*.*\)V|invoke-*.* \{*.*\}, Lcom*.*;->loadAd\(*.*\)V|invoke-*.* \{*.*\}, Lcom*.*;->requestBannerAd\(*.*\)V|invoke-*.*\s\{[v|p]\d\},\sLcom/facebook*.*\;\-\>show\(*.*\)V|invoke-*.*\s\{[v|p]\d\},\sLcom/google*.*\;\-\>show\(*.*\)V
```
replace 

```bash
nop
```







# Regex 9

search 🔍 

```bash
(\.method.*(loadAd|requestNativeAd|showInterstitial|fetchad|fetchads|onadloaded|requestInterstitialAd|showAd|loadAds|AdRequest|requestBannerAd|loadNextAd|createInterstitialAd|setNativeAd|loadBannerAd|loadNativeAd|loadRewardedAd|loadRewardedInterstitialAd|loadAds|loadAdViewAd|showInterstitialAd|shownativead|showbannerad|showvideoad|onAdFailedToLoad)\(.*\)V
    \.registers \d+)[\s\S]*?\.end method
```
replace 

```bash
#
```



### Features:
* Simple and intuitive interface
* No root access required
* Completely free with no in-app purchases
* Awesome library of pre-defined regex patterns
* Block various types of ads with the regex patterns
* Added several other patches to make the app more interesting
* Smali To Regex Converter inbuilt

### Instructions:
- Download the latest files 
- open the file and 
- enjoy.

### Notes:
- All devices are compatible.
- Turn off Play Protect so you can install without issues.

Ads Regex files built by [Nabin sharma](https://github.com/NabinSharmaitgithub).Contact Us [here](https://www.facebook.com/profile.php?id=100068552625787&mibextid=ZbWKwL) for more information or suggestions.





