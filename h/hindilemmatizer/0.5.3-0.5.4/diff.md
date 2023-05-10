# Comparing `tmp/hindilemmatizer-0.5.3-py3-none-any.whl.zip` & `tmp/hindilemmatizer-0.5.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6835979 bytes, number of entries: 10
+Zip file size: 6836048 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      156 b- defN 23-May-06 13:08 hindilemmatizer/__init__.py
 -rw-r--r--  2.0 unx     3677 b- defN 23-May-10 01:19 hindilemmatizer/lemmatizer.py
 -rw-r--r--  2.0 unx   555099 b- defN 23-May-08 16:44 hindilemmatizer/data/data.csv
--rw-r--r--  2.0 unx   192237 b- defN 23-May-08 18:07 hindilemmatizer/data/direct.csv
+-rw-r--r--  2.0 unx   191509 b- defN 23-May-10 01:23 hindilemmatizer/data/direct.csv
 -rw-r--r--  2.0 unx 23623710 b- defN 23-May-08 16:44 hindilemmatizer/data/totalWords.txt
--rw-r--r--  2.0 unx     1071 b- defN 23-May-10 01:20 hindilemmatizer-0.5.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      186 b- defN 23-May-10 01:20 hindilemmatizer-0.5.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-10 01:20 hindilemmatizer-0.5.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-10 01:19 hindilemmatizer-0.5.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      868 b- defN 23-May-10 01:20 hindilemmatizer-0.5.3.dist-info/RECORD
-10 files, 24377112 bytes uncompressed, 6834497 bytes compressed:  72.0%
+-rw-r--r--  2.0 unx     1071 b- defN 23-May-10 01:24 hindilemmatizer-0.5.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      186 b- defN 23-May-10 01:24 hindilemmatizer-0.5.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 01:24 hindilemmatizer-0.5.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-10 01:23 hindilemmatizer-0.5.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      868 b- defN 23-May-10 01:24 hindilemmatizer-0.5.4.dist-info/RECORD
+10 files, 24376384 bytes uncompressed, 6834566 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: hindilemmatizer/data/direct.csv
 Comment: 
 
 Filename: hindilemmatizer/data/totalWords.txt
 Comment: 
 
-Filename: hindilemmatizer-0.5.3.dist-info/LICENSE
+Filename: hindilemmatizer-0.5.4.dist-info/LICENSE
 Comment: 
 
-Filename: hindilemmatizer-0.5.3.dist-info/METADATA
+Filename: hindilemmatizer-0.5.4.dist-info/METADATA
 Comment: 
 
-Filename: hindilemmatizer-0.5.3.dist-info/WHEEL
+Filename: hindilemmatizer-0.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: hindilemmatizer-0.5.3.dist-info/top_level.txt
+Filename: hindilemmatizer-0.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: hindilemmatizer-0.5.3.dist-info/RECORD
+Filename: hindilemmatizer-0.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hindilemmatizer/data/direct.csv

```diff
@@ -221,15 +221,15 @@
 बहुमुखी,बहुमुख
 रही,रह
 महिलाअाे,महिला
 असमर्थ्ा,असमर्थ
 बनाइर्,बना
 संसदीय,संसद
 अध्यक्ष्ा,अध्यक्ष
-कहा ,कह
+कहा,कह
 मानवाधिकारो,मानवाधिकार
 तथ्यो,तथ्य
 वासियो,वासी
 प्रौद्योगिकी,प्रौद्योगिक
 परियोजनाएं,परियोजना
 बांटा,बांट
 जातियो,जाति
@@ -287,15 +287,15 @@
 विवरण्ााे,विवरण
 वर्गों,वर्ग
 असामयिक,असमय
 भाइयो,भाइी
 ताकतो,ताकत
 अखबारो,अखबार
 नजरिये,नजर
-विद्यार्थियो ,विद्यार्थी
+विद्यार्थियो,विद्यार्थी
 कारण्ााे,कारण
 जातियो,जाति
 डाक्टरो,डाक्टर
 कालेजो,कालेज
 सेवाएं,सेवा
 प्राथमिकता,प्राथमिक
 हड़ताली,हड़ताल
@@ -623,15 +623,15 @@
 तत्‍कालीन,तत्कालीन
 विद्वानों,विद्वान
 सेनाओं,सेना
 वादों,वादा
 रचाई,रचा
 जाएगा,जा
 क्रॉप्स,क्रॉप
-"१०,०००",१००००
+"१०,०००",10000
 निकाली,निकाल
 करता,कर
 मार्गों,मार्ग
 घायलों,घायल
 मिलाकर,मिला
 सटी,सट
 मतों,मत
@@ -687,15 +687,15 @@
 सुलझाने,सुलझा
 मानते,मान
 लाई,ला
 अन्तर्राष्ट्रीय,अंतर्राष्ट्रीय
 उड़ाने,उड़ा
 खुले,खुल
 सुधारने,सुधार
-"४,०००",४०००
+"४,०००",4000
 जीने,जी
 ग़ैर,गैर
 उपायों,उपाय
 चुका,चुक
 बदलने,बदल
 कहलाएँगे,कहला
 आवाजें,आवाज
@@ -729,15 +729,15 @@
 परिव्राजकों,परिव्राजक
 जाएँगे,जा
 आया,आ
 जाया,जा
 सभी,सब
 खिड़कियां,खिड़की
 बनना,बन
-"१६,९०६",१६९०६
+"१६,९०६",16906
 नियमों,नियम
 मानवशास्त्रियों,मानवशास्त्री
 खेतों,खेत
 हटने,हट
 स्तंभों,स्तंभ
 लड़ने,लड़
 पैकेजों,पैकेज
@@ -896,15 +896,15 @@
 नागरिकों,नागरिक
 मरीज़,मरीज
 कूदने,कूद
 टिकी,टिक
 रची,रच
 लेने,ले
 देकर,दे
-"१२,८२५",१२८२५
+"१२,८२५",12825
 मिलती,मिल
 बीते,बीत
 हूं,है
 घंटियाँ,घंटी
 पहुंचा,पहुंच
 जरूरतों,जरूरत
 भव्‍य,भव्
@@ -924,15 +924,15 @@
 चीजों,चीज
 अंगों,अंग
 घटकर,घट
 अवरोधों,अवरोध
 विस्फोटों,विस्फोट
 मनाने,मना
 पुलों,पुल
-"६५,३००",६५३००
+"६५,३००",65300
 डालकर,डाल
 हसरतें,हसरत
 रखते,रख
 बचने,बच
 मारकर,मार
 कुचले,कुचल
 भारतवासियों,भारतवासी
@@ -942,15 +942,15 @@
 प्रतिनिधियों,प्रतिनिधि
 निर्यातकों,निर्यातक
 निकालने,निकाल
 पाएगा,पा
 लकड़ी,लकडी
 इकाइयों,इकाई
 मुलाक़ात,मुलाकात
-"६०,३००",६०३००
+"६०,३००",60300
 रहेंगे,रह
 सुनेंगे,सुन
 उर्वरकों,उर्वरक
 न्यायाधीशों,न्यायाधीश
 रोका,रोक
 दिल्‍ली,दिल्ली
 सदियों,सदी
@@ -971,15 +971,15 @@
 मिलेंगी,मिल
 गाँवों,गाँव
 लाना,ला
 हफ्तों,हफ्ता
 घिरे,घिर
 खोली,खोल
 पड़ेगी,पड़
-"४,९१०",४९१०
+"४,९१०",4910
 अठखेलियाँ,अठखेली
 मूर्तियों,मूर्ति
 लपटें,लपट
 उबारने,उबार
 खुलेंगे,खुल
 बदलेगी,बदल
 उपकरणों,उपकरण
@@ -1005,15 +1005,15 @@
 डॉक्टर्स,डॉक्टर
 मामलों,मामला
 उकसाया,उकसा
 समझा,समझ
 बिताने,बिता
 खाना,खा
 घटकों,घटक
-"६३,०००",६३०००
+"६३,०००",63000
 बिगड़,बिगड
 कहना,कह
 उठती,उठ
 पैरों,पैर
 वामदलों,वामदल
 लटके,लटक
 अपनाता,अपना
@@ -1022,15 +1022,15 @@
 लेकर,ले
 भग्‍नावशेष,भग्
 चले,चल
 खींचता,खींच
 तोड़ना,तोड़
 बढ़ना,बढ़
 बढ़ाया,बढ़ा
-"२७,८२८९९",२७८२८९९
+"२७,८२८९९",2782899
 पड़,पड
 अपनाया,अपना
 सुनाई,सुना
 रहने,रह
 स्मृतियों,स्मृति
 जाएंगे,जा
 फसलों,फसल
@@ -1088,15 +1088,15 @@
 हमारा,हम
 जवानों,जवान
 बचाई,बचा
 पार्टियों,पार्टी
 चूके,चूक
 मुद्दों,मुद्दा
 विशेषज्ञों,विशेषज्ञ
-"६,५२१",६५२१
+"६,५२१",6521
 सैलानियों,सैलानी
 लगेगा,लग
 नुक़सान,नुकसान
 सुविधाएं,सुविधा
 दिक्कतों,दिक्कत
 मिली,मिल
 खतरों,खतरा
@@ -1112,15 +1112,15 @@
 करोड़,करोड
 जीता,जीत
 पाई,पा
 जाएँगी,जा
 छुट्टियां,छुट्टी
 सौंपा,सौंप
 चुके,चुक
-"७७,०००",७७०००
+"७७,०००",77000
 "55,000",55000
 चोटियों,चोटी
 हत्याएं,हत्या
 लड़ाई,लडाई
 किए,कर
 थीं,था
 गरीबों,गरीब
@@ -1138,15 +1138,15 @@
 जुड़ा,जुड़
 बंटे,बंट
 करना,कर
 होती,हो
 होते,हो
 धर्मों,धर्म
 आरोपों,आरोप
-"२७,६००",२७६००
+"२७,६००",27600
 करें,कर
 स्‍थानों,स्थान
 यही,यह
 झेलने,झेल
 जिसका,जो
 भिक्षुओं,भिक्षु
 नियंत्रकों,नियंत्रक
@@ -1265,15 +1265,15 @@
 जाना,जान
 लाइनों,लाइन
 चाहेंगे,चाह
 माँगेगा,माँग
 सुविधाएँ,सुविधा
 जोड़कर,जोड
 कोसते,कोस
-"१४,५००",१४५००
+"१४,५००",14500
 मानना,मान
 सिफारिशों,सिफारिश
 जड़ें,जड़
 निकलने,निकल
 हुआ,हो
 मंत्रों,मंत्र
 बुलाकर,बुला
@@ -1317,15 +1317,15 @@
 लगाकर,लगा
 पक्षों,पक्ष
 विष्‍णु,विष्णु
 मिलाने,मिला
 हमें,हम
 खिलाड़ियों,खिलाडी
 भस्‍म,भस्म
-"२८,२७६",२८२७६
+"२८,२७६",28276
 बढ़ोतरी,बढोतरी
 लिखे,लिख
 आवश्यकताओं,आवश्यकता
 मानकों,मानक
 करेंगी,कर
 चाहते,चाह
 बढ़ने,बढ
@@ -1424,15 +1424,15 @@
 बनाते,बना
 ऑडिटरों,ऑडिटर
 सकूंगी,सक
 खिसकती,खिसक
 केंद्रों,केंद्र
 सुझाए,सुझा
 सदस्यों,सदस्य
-"५,२९३",५२९३
+"५,२९३",5293
 देखने,देख
 बने,बन
 कराते,करा
 ढूंढ़ने,ढूंढ़
 पीपुल्स,पीपुल
 गर्मियों,गर्मी
 होगा,हो
@@ -1501,15 +1501,15 @@
 गड़बड़ाए,गडबडा
 खंडों,खंड
 रखता,रख
 दुर्भावनाओं,दुर्भावना
 लगी,लग
 ठहरे,ठहर
 "70,000",70000
-"३३,४८२",३३४८२
+"३३,४८२",33482
 अत्‍यंत,अत्यंत
 सिक्‍के,सिक्
 निष्कर्षों,निष्कर्ष
 दिलाएगा,दिला
 लौटकर,लौट
 परंपराओं,परंपरा
 "5,000",5000
@@ -1536,15 +1536,15 @@
 रखेगी,रख
 नैय्या,नैया
 मंडराने,मंडरा
 निर्दलीयों,निर्दलीय
 चलती,चल
 हेलीकॉप्टर्स,हेलीकॉप्टर
 सोते,सो
-"७७,४५५",७७४५५
+"७७,४५५",77455
 उभरती,उभर
 मोटरसाइकिल्स,मोटरसाइकिल
 उठेंगे,उठ
 स्कीमों,स्कीम
 जलता,जल
 दबोचा,दबोच
 लड़की,लडकी
@@ -1597,15 +1597,15 @@
 बढ़े,बढ
 गुणों,गुण
 लगे,लग
 एग्ज़िबिशन,एग्जिबिशन
 बंटेगा,बंट
 स्‍पोर्टस,स्पोर्ट
 चलेगा,चल
-२५वीं,२५
+२५वीं,25
 दिखना,दिख
 तुम्हारे,तुम
 निकलता,निकल
 पकाया,पका
 गुज़रने,गुजर
 बनवाने,बनवा
 घटाने,घटा
@@ -1681,15 +1681,15 @@
 चोटें,चोट
 फेंके,फेंक
 माँगने,माँग
 कढ़ाई,कढाई
 सुधरी,सुधर
 उड़ाया,उडा
 पन्नों,पन्ना
-"८०,०००",८००००
+"८०,०००",80000
 गाँवों,गांव
 लुटाने,लुटा
 मनोवैज्ञानिकों,मनोवैज्ञानिक
 प्रतियां,प्रति
 भेजेगा,भेज
 तुले,तुल
 उलटपुलटकर,उलटपुलट
@@ -1809,15 +1809,15 @@
 फैलना,फैल
 आयवर्गवालों,आयवर्गवाला
 छुट्टियाँ,छुट्टी
 दबावों,दबाव
 संस्थाओं,संस्था
 गुज़ारा,गुजारा
 खिंचवाए,खिँच
-४.११,४.१
+4.11,4.1
 करनी,कर
 लाता,ला
 ब्रजवासियों,ब्रजवासी
 जुटेंगे,जुट
 धरे,धर
 मेरे,मैं
 बचती,बच
@@ -1856,15 +1856,15 @@
 कमांडरों,कमांडर
 मुलाजिमों,मुलाजिम
 क़दम,कदम
 मिलाए,मिला
 पट्टियां,पट्टी
 बहकर,बह
 लगानी,लगा
-"१८,५८७",१८५८७
+"१८,५८७",18587
 संपादकों,संपादक
 युवकों,युवक
 खोजी,खोज
 कथाओं,कथा
 जीतने,जीत
 बनें,बन
 सीज़न,सीजन
@@ -1889,15 +1889,15 @@
 मारने,मार
 रोज़,रोज
 एजेंसिंयों,एजेंसी
 पड़ोसी,पडोसी
 बचना,बच
 प्रश्नों,प्रश्न
 अफगानिस्तानियों,अफगानिस्तानी
-"७,४८०",७
+"७,४८०",7
 प्रायोजकों,प्रायोजक
 बोगियां,बोगी
 बदलता,बदल
 नावों,नाव
 रहे,रह
 रूका,रूक
 देखकर,देख
@@ -2016,15 +2016,15 @@
 "आईजी,",आईजी
 परियोजनाएं,परियोजना
 श्रेयस्‍कर,श्रेयस्
 इराकियों,इराकी
 तत्वों,तत्व
 मिलकर,मिल
 पत्थरों,पत्थर
-"२,०००",२०००
+"२,०००",2000
 कसने,कस
 खामियों,खामी
 बोर्डो,बोर्ड
 छूटे,छूट
 सौदों,सौदा
 बरती,बरत
 मोड़,मोड
@@ -2371,15 +2371,15 @@
 तोहफों,तोहफा
 हथियाने,हथिया
 दर्शाता,दर्शा
 समझते,समझ
 पहाड़,पहाड
 मेजबानों,मेजबान
 थामे,थाम
-"१४,६३६",१४६३६
+"१४,६३६",14636
 जुटाकर,जुटा
 कारसेवकों,कारसेवक
 जहाज़,जहाज
 उद्घधाटन,उद्घाटन
 महानगरों,महानगर
 चरणों,चरण
 परोसी,परोस
@@ -2411,15 +2411,15 @@
 नंबरों,नंबर
 मैचों,मैच
 चाहा,चाह
 उपजी,उपज
 रेलों,रेल
 खींचा,खींच
 जिताने,जिता
-"२,६००",२६००
+"२,६००",2600
 पड़ा,पड
 भरकर,भर
 घुसने,घुस
 दिलाते,दिला
 एतराज़,एतराज
 पड़ती,पड
 सम्बोधित,संबोधित
@@ -2487,15 +2487,15 @@
 फटने,फट
 ऊंचाइयों,ऊंचाई
 वादियाँ,वादी
 उड़ाने,उडान
 गोष्ठियों,गोष्ठी
 बाड़ी,बाडी
 स्तूपों,स्तूप
-"१४,०५३",१४०५३
+"१४,०५३",14053
 डराने,डरा
 शहरों,शहर
 पंचायतों,पंचायत
 सड़कों,सडक
 जमाकर,जमा
 कुबूलने,कुबूल
 तरफ़,तरफ
@@ -2552,15 +2552,15 @@
 बनाएगा,बना
 गुजरेंगे,गुजर
 लगने,लग
 सुनाते,सुना
 सर्किलों,सर्किल
 अपवादों,अपवाद
 तस्वीरों,तस्वीर
-"३२०,०००",३२००००
+"३२०,०००",320000
 धर्मस्थलों,धर्मस्थल
 जलाया,जला
 बढ़ाने,बढा
 बताईं,बता
 बचाओ,बचा
 घुसते,घुस
 खुली,खुल
@@ -2579,15 +2579,15 @@
 फैला,फैल
 बचें,बच
 धरोहरें,धरोहर
 ज़रूरतों,ज़रूरत
 सुरक्षागार्डों,सुरक्षागार्ड
 रखना,रख
 केन्द्र,केंद्र
-"९३,३६९",९३३६९
+"९३,३६९",93369
 प्रस्तावों,प्रस्ताव
 डिस्ट्रीब्यूटरों,डिस्ट्रीब्यूटर
 करोड़पति,करोडपति
 कार्यालयों,कार्यालय
 होता,हो
 विज्ञानियों,विज्ञानी
 सितम्बर,सितंबर
@@ -2622,15 +2622,15 @@
 क्लस्टरिंग,कलस्टरिंग
 दर्शनों,दर्शन
 जाएगा,जा
 दूंगी,दे
 डालेंगे,डाल
 खटखटाना,खटखटा
 चेतना,चेत
-"१०,०००",१००००
+"१०,०००",10000
 निकाली,निकाल
 मिलाएगा,मिला
 मंगवाया,मंगवा
 सड़कों,सड़क
 नम्बर,नंबर
 हिचकते,हिचक
 करता,कर
@@ -2639,25 +2639,25 @@
 स्कूलों,स्कूल
 खेलों,खेल
 घायलों,घायल
 मुस्लिम,मजबूत
 दागे,दाग
 फ़रार,फरार
 ढोने,ढो
-"२,१००",२१००
+"२,१००",2100
 मिलाकर,मिला
 मोहरों,मोहर
 कासलों,कासल
 कोशिकाओं,कोशिका
 मतों,मत
 ए.,ए
 जमने,जम
 बचके,बच
 अभियानों,अभियान
-"३०,०००",३००००
+"३०,०००",30000
 सकें,सक
 बरसानी,बरसा
 राजभवनों,राजभवन
 वार्डो,वार्ड
 फूलों,फूल
 बिना,बिन
 बर्तनों,बर्तन
@@ -2675,15 +2675,15 @@
 अंधड़,अंधड
 के.,का
 बची,बच
 ट्रस्टों,ट्रस्ट
 लगाई,लगा
 समर्थकों,समर्थक
 दबाने,दबा
-"१०,५६४",१०५६४
+"१०,५६४",10564
 कुचलकर,कुचल
 बदलते,बदल
 कुर्सियां,कुर्सी
 भाईयों,भाई
 बोलियां,बोली
 अंशधारकों,अंशधारक
 स्वीकारते,स्वीकार
@@ -2719,15 +2719,15 @@
 तलाशने,तलाश
 खदेड़,खदेड
 ट्रकों,ट्रक
 दलों,दल
 विश्वविद्यालय,विशवविद्यालय
 एयरलाइंस,एयरलाइन
 जोड़,जोड
-"३,१३,०००",३१३०००
+"३,१३,०००",313000
 धमाकों,धमाका
 नाक़ामयाब,नाकामयाब
 सैकड़ों,सैकड़ा
 मानेंगे,मान
 कराएगा,करा
 पतों,पता
 जेलें,जेल
@@ -2735,15 +2735,15 @@
 पड़ने,पड़
 पहुंचीं,पहुंच
 वालों,वाला
 गहनों,गहना
 लड़कियां,लड़की
 भीड़भाड़,भीडभाड
 गिनाए,गिना
-"२९,०००",२९०००
+"२९,०००",29000
 लगा,लग
 चढ़कर,चढ़
 तगड़ा,तगडा
 हटाने,हटा
 बताए,बता
 बिगड़ती,बिगड
 जगाई,जगा
@@ -2792,15 +2792,15 @@
 सोचिए,सोच
 घबराए,घबरा
 जाय,जा
 समस्याएं,समस्या
 कणों,कण
 पाकर,पा
 कारोबारियों,कारोबारी
-"१०,५७३",१०५७३
+"१०,५७३",10573
 जिनकी,जो
 जानतीं,जान
 द्वीपों,द्वीप
 गवाया,गवा
 उतारेगा,उतार
 जिसमें,जो
 कपड़े,कपडा
@@ -2936,15 +2936,15 @@
 नतिनियों,नतिनी
 पिलाती,पिला
 आवाजों,आवाज
 बसाया,बसा
 होगी,हो
 आख़िरकार,आखिरकार
 नहलाया,नहला
-"३,७०१",३७०१
+"३,७०१",3701
 करूँगा,कर
 आंतकियों,आंतकी
 घटनाक्रमों,घटनाक्रम
 साइकिल्स,साइकिल
 तोड़,तोड
 इमारतों,इमारत
 तरेरने,तरेर
@@ -3056,15 +3056,15 @@
 छोड़िए,छोड
 खोला,खोल
 पाए,पा
 बंदियों,बंदी
 लेती,ले
 मांगना,मांग
 समूहों,समूह
-"१,२७,३५७",१२७३५७
+"१,२७,३५७",127357
 उभरने,उभर
 पटरियां,पटरी
 मांगे,मांग
 सधी,सध
 जीवों,जीव
 सुधारनी,सुधार
 ढले,ढल
@@ -3337,15 +3337,15 @@
 पहुँचेगा,पहुँच
 कराई,करा
 सामग्रियों,सामग्री
 ड्राइवरों,ड्राइवर
 गुंबदों,गुंबद
 प्रतिबद्घताओं,प्रतिबद्घता
 पहनी,पहन
-"९,५००",९५००
+"९,५००",9500
 परियोजनाओं,परियोजना
 संगठनों,संगठन
 हराने,हरा
 कोर्सों,कोर्स
 उठाएंगे,उठा
 उड़ानों,उड़ान
 पत्नियों,पत्नी
@@ -3397,15 +3397,15 @@
 साधते,साध
 टुकड़ियाँ,टुकडी
 गवांनी,गवाँ
 प्राप्‍त,प्राप्त
 पकड़े,पकड
 रिपोर्टें,रिपोर्ट
 उड़ान,उडान
-"५०,०००",५००००
+"५०,०००",50000
 पार्टियां,पार्टी
 रहेंगी,रह
 पाती,पा
 उड़ाई,उड़ा
 बिताए,बिता
 उतरा,उतर
 आख्यानों,आख्यान
@@ -3480,15 +3480,15 @@
 गोलों,गोला
 निविदाओं,निविदा
 छोड़ने,छोड
 मोहल्लों,मोहल्ला
 मक़बरे,मकबरा
 दवाइयों,दवाई
 रखा,रख
-"२८,७३७",२८७३७
+"२८,७३७",28737
 तराशकर,तराश
 जाने,जा
 नज़र,नजर
 सिक्खी,सिक्ख
 पार्टनरों,पार्टनर
 अक़बर,अकबर
 विस्फ़ोट,विस्फोट
@@ -3681,15 +3681,15 @@
 मुर्गों,मुर्गा
 उछालने,उछाल
 बढ़ा,बढ़
 आईं,आ
 बदलेंगे,बदल
 बचने,बच
 मारकर,मार
-"४,००,९६६",४००९६६
+"४,००,९६६",400966
 उठते,उठ
 डी.,डी
 बरतनी,बरत
 परीक्षाएं,परीक्षा
 पूछा,पूछ
 ठहरने,ठहर
 प्रतिनिधियों,प्रतिनिधि
@@ -3752,15 +3752,15 @@
 समानताओं,समानता
 रगड़,रगड
 दामों,दाम
 विधाओं,विधा
 बनाकर,बना
 अभी,अब
 डूबने,डूब
-"३७,०००",३७०००
+"३७,०००",37000
 बताया,बता
 खबरों,खबर
 आश्रितों,आश्रित
 राज़ी,राजी
 लम्बी,लंबा
 स्रोतों,स्रोत
 जाएँगीं,जा
@@ -3836,15 +3836,15 @@
 चलता,चल
 बढ़ाये,बढा
 क़ानून,कानून
 विस्फोटकों,विस्फोटक
 मान्यताओं,मान्यता
 झलकता,झलक
 जिसको,जो
-"२०,०००",२०
+"२०,०००",20
 सुने,सुन
 घुसे,घुस
 खरीदना,खरीद
 बरतना,बरत
 औपचारिकताएँ,औपचारिकता
 दोहराई,दोहरा
 बचाने,बचा
@@ -3858,15 +3858,15 @@
 डाक्टरों,डाक्टर
 कर्ताओं,कर्ता
 हवाईअड्डों,हवाईअड्डा
 चिथड़े,चिथडा
 छोड़ूंगा,छोड़
 अधिकारों,अधिकार
 कानूनों,कानून
-"१३,७००",१३७००
+"१३,७००",13700
 कछुओं,कछुआ
 प्रतिभागियों,प्रतिभागी
 मतपेटियों,मतपेटी
 बातों,बात
 लानी,ला
 दिखता,दिख
 देता,दे
@@ -3878,15 +3878,15 @@
 बाढ़,बाढ
 मामलों,मामला
 प्लांटों,प्लांट
 बढ़ाएंगे,बढ़ा
 ठहरेंगे,ठहर
 ख़त्म,खत्म
 नारों,नारा
-"२२,०००",२२०००
+"२२,०००",22000
 छापामारों,छापामार
 उतरेंगे,उतर
 आएँ,आ
 होंगें,हो
 नागालैंडा,नागालैंड
 फ्लैटों,फ्लैट
 भाषाओं,भाषा
@@ -3894,15 +3894,15 @@
 चढ़ा,चढा
 गिरना,गिर
 समझा,समझ
 हक़ीकत,हकीकत
 घुसपैठियों,घुसपैठी
 बहना,बह
 मरा,मर
-"१,२७,५११",१२७५११
+"१,२७,५११",127511
 उतारा,उतार
 फ़र्जी,फर्जी
 बिताने,बिता
 खाना,खा
 आँकड़ों,आँकडा
 जुटाई,जुटा
 जरूरतमंदों,जरूरतमंद
@@ -3965,15 +3965,15 @@
 युवाओं,युवा
 छपने,छप
 उठाएँगे,उठा
 बिके,बिक
 सुधरे,सुधर
 छिपता,छिप
 अपनाया,अपना
-"४,८९८",४
+"४,८९८",4
 मुद्राएं,मुद्रा
 पलटी,पलट
 जिप्सियों,जिप्सी
 खरीदनी,खरीद
 उत्तराधिकारियों,उत्तराधिकारी
 भागीं,भाग
 सुनाई,सुना
@@ -3991,15 +3991,15 @@
 जाएंगे,जा
 दिवसों,दिवस
 फसलों,फसल
 पड़ना,पड
 सोचना,सोच
 इच्‍छानुसार,इच्छानुसार
 जोड़ने,जोड़
-"५४,०००",५४
+"५४,०००",54
 पढ़कर,पढ़
 खाता,खा
 बैठकों,बैठक
 सुविधाओं,सुविधा
 साज़िश,साजिश
 जनसभाएं,जनसभा
 पहलुओं,पहलू
@@ -4036,15 +4036,15 @@
 लड़ा,लड़
 शोलों,शोला
 हटी,हट
 विभूतियों,विभूति
 सुनना,सुन
 तपता,तप
 उगलवा,उगल
-"१०,०००",१०
+"१०,०००",10
 ए.डबल्यू.डबल्यू.ए.,ए.डबल्यू.डबल्यू.ए
 कर्तव्यों,कर्तव्य
 ग्रंथों,ग्रंथ
 डूबा,डूब
 उठाए,उठा
 पहुँचते,पहुँच
 छेड़,छेड
@@ -4253,15 +4253,15 @@
 हितैषियों,हितैषी
 परीक्षार्थियों,परीक्षार्थी
 पदों,पद
 देशवासियों,देशवासी
 सुरक्षाबलों,सुरक्षाबल
 जानें,जान
 हारने,हार
-"५०,६४१",५०६४१
+"५०,६४१",50641
 पहुंची,पहुंच
 सेंटरों,सेंटर
 युवतियों,युवती
 कराये,करा
 ब्रोकरों,ब्रोकर
 दर्शकों,दर्शक
 सीखते,सीख
@@ -4292,20 +4292,20 @@
 सौंपा,सौंप
 खामियां,खामी
 बनाई,बना
 वजहों,वजह
 प्रगाढ़,प्रगाढ
 कहता,कह
 बदली,बदल
-"२०,०००",२००००
+"२०,०००",20000
 चुके,चुक
 दिखाना,दिखा
 केमिकल्स,केमिकल
 लौटता,लौट
-३२९३२९,३२९
+329329,329
 चिल्लाना,चिल्ला
 धरना,धर
 फंसने,फँस
 चोटियों,चोटी
 राजनेताओं,राजनेता
 हत्याएं,हत्या
 लड़ाई,लडाई
@@ -4426,15 +4426,15 @@
 नमाजियों,नमाजी
 क़ाफिले,काफिला
 पीना,पी
 मिलें,मिल
 ढोलों,ढोल
 पहाड़ियां,पहाड़ी
 लड़कों,लडका
-"४०,०००",४००००
+"४०,०००",40000
 जमकर,जम
 चट्टानें,चट्टान
 खेलती,खेल
 बीतने,बीत
 पहचाना,पहचान
 कीजिए,कर
 पहुंचने,पहुंच
@@ -4447,15 +4447,15 @@
 रदों,रदा
 कैरक्टरों,कैरक्टर
 दिखाएगा,दिखा
 साहबों,साहब
 किसी,कोई
 शक्तियों,शक्ति
 निभाने,निभा
-"४,८२४",४८२४
+"४,८२४",4824
 खुशियां,खुशी
 अजनबियों,अजनबी
 चप्पुओं,चप्पू
 नोएडावासियों,नोएडावासी
 तुक़,तुक
 उठाएं,उठा
 पाले,पाल
@@ -4569,15 +4569,15 @@
 नुमाइंदें,नुमाइंदा
 डरने,डर
 पीड़ितों,पीड़ित
 जाएगी,जा
 कसमसाते,कसमसा
 जनश्रुतियाँ,जनश्रुति
 बताने,बता
-"२६,०००",२६
+"२६,०००",26
 क़िला,किला
 हिन्दुत्व,हिंदुत्व
 दबी,दब
 संतों,संत
 टेके,टेक
 फेंकते,फेंक
 चौंका,चौंक
@@ -4604,16 +4604,16 @@
 सबकी,सब
 ख़ान,खान
 पगडंडियां,पगडंडी
 छीनी,छीन
 समझाने,समझा
 दोहराए,दोहरा
 पहनना,पहन
-"८५,०००",८५०००
-"९,०००",९०००
+"८५,०००",85000
+"९,०००",9000
 तुमने,तुम
 बनवाई,बन
 मालाएं,माला
 सुनकर,सुन
 लिखा,लिख
 अपराधों,अपराध
 जाएंगी,जा
@@ -4640,15 +4640,15 @@
 घड़े,घडा
 आंकें,आंक
 झुकाना,झुका
 जतायी,जता
 कांग्रेसियों,कांग्रेसी
 सबको,सब
 इलाकों,इलाका
-"११,१२०",१११२०
+"११,१२०",11120
 एअरलाइंस,एअरलाइन
 रहती,रह
 बोलती,बोल
 क़वायद,कवायद
 फंसा,फँस
 दिखाता,दिखा
 दवाइयां,दवाई
@@ -4657,15 +4657,15 @@
 दिखाते,दिखा
 माननी,मान
 स्थितियां,स्थिति
 दीर्घाओं,दीर्घा
 घिरने,घिर
 करे,कर
 फिल्‍माया,फिल्‍मा
-"१,५००",१५००
+"१,५००",1500
 घटाकर,घटा
 रैलियाँ,रैली
 पाते,पा
 संभाला,संभाल
 सटे,सट
 आएंगे,आ
 उग्रवादियों,उग्रवादी
@@ -4755,15 +4755,15 @@
 सीढ़ियों,सीढ़ी
 जेड्स,जेड
 सुनाया,सुना
 नदियां,नदी
 बोलता,बोल
 याचिकाएँ,याचिका
 झुकी,झुक
-"१५,०००",१५०००
+"१५,०००",15000
 भूलतीं,भूल
 मांगों,मांग
 जिस,जो
 तहसीलों,तहसील
 संसाधनों,संसाधन
 खिड़कियों,खिडकी
 आकांक्षाओं,आकांक्षा
@@ -4892,15 +4892,15 @@
 अड़चनों,अड़चन
 किये,कर
 साहित्यकारों,साहित्यकार
 अंकों,अंक
 फरेबियों,फरेबी
 सौंपेगी,सौंप
 साइंसेस,साइंस
-"७०,१०१",७०१०१
+"७०,१०१",70101
 लेते,ले
 डेलिगेट्स,डेलिगेट
 जिनको,जो
 पड़ा,पड़
 प्रतिष्ठानों,प्रतिष्ठान
 गिरफ़्तारी,गिरफ्तारी
 टूटने,टूट
@@ -4933,24 +4933,24 @@
 वस्तुएँ,वस्तु
 प्रचारकों,प्रचारक
 पेसरों,पेसर
 साधने,साध
 बढ़ाने,बढ़ा
 सूचनाएँ,सूचना
 प्रियजनों,प्रियजन
-"१५०,०००",१५००००
+"१५०,०००",150000
 लगाकर,लगा
 उगाई,उगा
 बचा,बच
 पक्षों,पक्ष
 विष्‍णु,विष्णु
 मिलाने,मिला
 निर्देशकों,निर्देशक
 लकड़ियां,लकड़ी
-३३३६०२३३३६०२,३३३६०२
+333602333602,333602
 सकेंगे,सक
 गाडियां,गाडी
 हमें,हम
 समुद्रों,समुद्र
 दृश्यों,दृश्य
 उमड़ा,उमड
 खेलना,खेल
@@ -5073,15 +5073,15 @@
 बड़ी,बडा
 बंधी,बँध
 खटखटाया,खटखटा
 न्यौता,न्यौत
 पुजारियों,पुजारी
 उखाड़,उखाड
 स्थितियाँ,स्थिति
-"१,६००",१६००
+"१,६००",1600
 बुलाना,बुला
 ढाला,ढाल
 डीज़ल,डीजल
 चौड़े,चौडा
 भारतीयों,भारतीय
 जिनसे,जो
 देशों,देश
@@ -5091,15 +5091,15 @@
 बांग्लादेशियों,बांग्लादेशी
 लिए,ले
 लगता,लग
 पहनाया,पहना
 गुरुद्वारों,गुरुद्वारा
 पाया,पा
 सेनाएं,सेना
-"२,५००",२५००
+"२,५००",2500
 सूत्रों,सूत्र
 पाँचों,पाँच
 कल्पनाओँ,कल्पना
 फोड़े,फोड़
 ठहरी,ठहर
 वाहनों,वाहन
 समझना,समझ
@@ -5128,15 +5128,15 @@
 पाऊंगी,पा
 अलगावादियों,अलगावादी
 बेचने,बेच
 गड़बड़,गडबड
 नदियों,नदी
 के.,के
 निपटाया,निपटा
-"१००,०००",१०००००
+"१००,०००",100000
 हटेगा,हट
 झुकें,झुक
 बोई,बो
 तबकों,तबका
 देखा,देख
 भरी,भर
 करूंगी,कर
@@ -5196,15 +5196,15 @@
 खड़कने,खड़क
 रिकार्डों,रिकार्ड
 बनी,बन
 व्यापारियों,व्यापारी
 समुदायों,समुदाय
 खाने,खा
 गढ़,गढ
-"६५,०००",६५०००
+"६५,०००",65000
 हैं,है
 तगड़े,तगडा
 जहाजों,जहाज
 उछाला,उछाल
 क्षेत्राधिकारियों,क्षेत्राधिकारी
 लड़कर,लड
 रुकवाने,रुकवा
@@ -5238,15 +5238,15 @@
 पांचवीं,पांचवा
 जानने,जा
 सहूलियतें,सहूलियत
 मार्शलों,मार्शल
 उगाने,उगा
 ऑपरेशंस,ऑपरेशन
 पंचकेदारों,पंचकेदार
-"३५,०००",३५०००
+"३५,०००",35000
 विस्फ़ोटों,विस्फोट
 सकूं,सक
 परिजनों,परिजन
 कटी,कट
 बखेड़ा,बखेडा
 उपलब्धियां,उपलब्धि
 उड़ाने,उडा
@@ -5385,36 +5385,36 @@
 लेंगे,ले
 आएं,आ
 चुकीं,चुक
 उघाड़,उघाड
 पुरातत्वविदों,पुरातत्वविद
 लगवाती,लग
 टेका,टेक
-"११,४५८",११४५८
+"११,४५८",11458
 पौने,पौन
 चुनावों,चुनाव
 आते,आ
 बग़ैर,बगैर
 खानी,खा
 भगाए,भगा
-"७०,०००",७००००
+"७०,०००",70000
 दीवारें,दीवार
 सिक्कों,सिक्का
 कदमों,कदम
 बांटा,बांट
 दुकानदारों,दुकानदार
 द्रव्यों,द्रव्य
 आंतकवादियों,आंतकवादी
 मुस्लिमों,मुस्लिम
 रक़म,रकम
 लाइन्स,लाइन
 मुझसे,मैं
 पूछे,पूछ
 बैठकें,बैठक
-"४,२९,०००",४२९०००
+"४,२९,०००",429000
 निपटाएंगे,निपटा
 जातियों,जाति
 क़रीब,करीब
 बैठे,बैठ
 वेश्याओं,वेश्या
 जोरों,जोर
 खींचना,खींच
@@ -5445,27 +5445,27 @@
 इतिहासविदों,इतिहासविद
 मंत्रालयों,मंत्रालय
 बदलकर,बदल
 होनेवाली,हो
 झटकों,झटका
 मिल्स,मिल
 रिफाइनरियों,रिफाइनरी
-"१,०००",१०००
+"१,०००",1000
 जुड़ने,जुड़
 पशुओं,पशु
 दीं,दे
 बचते,बच
 वेत्ताओं,वेत्ता
 मंडलों,मंडल
 धरी,धर
 कड़ियों,कडी
 "80,000",80000
-"३२,०००",३२
+"३२,०००",32
 महलों,महल
-"३,२३,५६३",३२३५६३
+"३,२३,५६३",323563
 टलने,टल
 गेंदबाजों,गेंदबाज
 स्कैनरों,स्कैनर
 भटकाने,भटका
 जाए,जा
 बढ़कर,बढ़
 गुजरती,गुजर
@@ -5507,15 +5507,15 @@
 आतंकवादियों,आतंकवादी
 विजेताओं,विजेता
 मौकों,मौका
 कमजोरियों,कमजोरी
 गुजारी,गुजार
 लिखित,लिख
 ट्रेनें,ट्रेन
-"३५,०१८",३५०१८
+"३५,०१८",35018
 क़तर,कतर
 होंगे,हो
 ढूंढने,ढूंढ
 गाते,गा
 उड़,उड
 उड़ती,उड़
 ठहराया,ठहरा
@@ -5546,17 +5546,17 @@
 ख़ाली,खाली
 भिड़ना,भिड़
 दफनाया,दफना
 गड़ी,गड
 लाएंगे,ला
 बैठना,बैठ
 अटकाने,अटका
-"१,४००",१४००
+"१,४००",1400
 ढूँढ़े,ढूँढ
-"६,१६,४००",६१६४००
+"६,१६,४००",616400
 बढ़ेंगे,बढ़
 समझिए,समझ
 मज़बूत,मजबूत
 विनियमों,विनियम
 पहचानी,पहचान
 रखता,रख
 घुसकर,घुस
@@ -5580,14 +5580,16 @@
 अधीनस्थों,अधीनस्थ
 उखाड़कर,उखाड
 लौटकर,लौट
 परंपराओं,परंपरा
 मृतकों,मृतक
 परिस्थितियाँ,परिस्थिति
 खेला,खेल
-"१८,७४०",१८७४०
+"१८,७४०",18740
 प्रतिक्रियाएँ,प्रतिक्रिया
 लेगा,ले
 मानकर,मान
 बांधों,बांध
 जमाकर्ताओं,जमाकर्ता
 खेमों,खेमा
+की,का
+के,का
```

## Comparing `hindilemmatizer-0.5.3.dist-info/LICENSE` & `hindilemmatizer-0.5.4.dist-info/LICENSE`

 * *Files identical despite different names*
