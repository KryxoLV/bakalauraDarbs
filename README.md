# Bakalaura darbs - Kristers Rutkis 3ITB
## Botānisko vārdnīcu digitalizācija un datu integrācija IMDS sistēmā, izmantojot attēlu apstrādes algoritmus un mašīnmacīšanās algoritmus - Digitization of botanical dictionaries and data integration in IMDS system using image processing algorithms and machine learning algorithms

  Bakalaura darba laikā izstrādātas programmas kods pieejams gan .rar , gan .zip formātos - tādējādi izvairoties no maksimālā atļauto failu skaita limita GitHub vidē.  
  Lai atarhivēt programmas kodu, nepieciešams to lejuplādēt no GitHub repozitorija. Atvērt to ar WinRar vai 7zip piedāvāto risinājumu. Atarhivēt Jums ērtā vietā.  
  Pēc arhīva izvlikšanas nepieciešams izvilkt arī to saturošo images arhīvu. Ērtības nolūkos to būtu labi atarhivēt iekš Bakalaurs_V1 mapes.  
  Pēc abu arhīvu atarhivēšanas tos drīkst izdzēst.  
  Pēc arhīva izdzēšanas nepieciešams iegūto images folderi dublēt arī OCR/KerasOCR , OCR/TesseractOCR un OCR/EasyOCR folderos  

#### **Izmantotā vide **
Python
Anaconda Command Prompt

  #### **Nepieciešamās bilbiotēkas **
    tesserocr (conda install -c simonflueckiger tesserocr)
    langdetect(pip install langdetect)
    csv(ietverts automātiski)
    spacy.language(ietverts spacy.langdetect)
    spacy.langdetect(pip install spacy_langdetect un  python -m spacy download en_core_web_sm)
    spacy (pip install spacy)
    lingua (pip install linuga-language-detector)
    easyocr (pip install easyocr)
    glob (automātiski ietverts)
    keras_ocr(pip install keras_ocr)
    keras (pip install keras)
    tensorflow (pip install tensorflow)
    matplotlib.pyplot (automātiski ietverts)
    PIL (automātiski ietverts)
    numpy (automātiski ietverts)
    matplotlib (pip install matplotlib)
    matplotlib.font_manager
    re (automātiski ietverts)
    os (automātiski ietverts)
    requests (pip install requests)
    urllib.parse (automātiski ietverts)
    bs4 (pip install bs4)
    fitz (pip install pymupdf)
    ntpath (automātiski ietverts)
    pathlib (automātiski ietverts)
    xlwings (pip install xlwings)
    openpyxl (pip install openpyxl)
    pandas (automātiski ietverts)
    itertools (automātiski ietverts)
  
  #### **Anaconda vides uzstādīšana :**
    *https://www.anaconda.com/products/distribution#windows*
    Izmantojot Anaconda tīmekļa vietni lejuplādēt Anaconda Python 3.9 versiju
    Veikt instalāciju pēc sniegtajām norādēm instalācijas failā
    Pēc instalācijas veikšanas atvērt Anaconda command prompt un izveidot jaunu vidi pamatojoties uz tālāk esošās tīmekļavientes pamācību
    *https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html*
    Pēc vides izveidošanas, aktivizēt vidi ar komandu "activate videsNosaukums"
    Lai pārliecinātos par vides aktivizēšanu - vides nosaukumam jārādas komandrindas pašā sākumā - iekavās
    Tālāk jāuzstāda nepieciešamās bibliotēkas programmas izpildei - to iespējams izdarīt rakstot komandrindu ailēs komandas, kuras norādītas aiz bilbiotēkām iekavās.
    Kopējais bilbiotēku apjoms : apmēram 2.5 - 3.0 GB

  Dažreiz lajuplādējot un uzstādot bibliotēkas tās savstarpēji nesadarbojas un izdzēš viena otru, tad nepieciešams vēlreiz palaist attiecīgās bilbiotēkas lejuplādi un uzstādīšanu
  
  #### **Bakalaura darba nodevuma struktūra :** 
      Katrs no atsevišķiem posmiem ir sadalīts daļās  - apakšdirektorijās. Piemēram, OCR daļa ir zem OCR direktorijas u.t.t.
      Ir iespējams palaist, apskatīt kodu katram no posmiem atsevišķi, vai darbināt kopējo programmas versiju (v1-3folder.py)
      
  #### **Kopējas programmas versijas palaišana** :
      Atverot Anaconda command prompt, nepieciešams pārliecināties vai aktīva iepirekšējos soļos uzstādītā vide
      Pēc vides aktivizēšanas izmantojot cd komandu nepieciešams "aizstaigāt" līdz faila direktorijai
      Izmantojot komandu "Python V1-3folder.py" jāpalaiž programma
      Pirmā programmas izvade pieprasīs ievadīt JPG failu saturošu dirketoriju - mūsu gadījumā tā ir images direktorija. Piemērs - C:\Users\BigBoy\Downloads\Bakalura_V1\images
      Nākamā programmas izvade pieprasīs ievadīt faila izvades direktoriju - ērtības nolūkos šo atstājam tukšu , lai faili taisās turpat Bakalaurs_V1 direktorijā
      Pēc programmas izpildes zem direktorijas "UnSorted" redzams sadalījums pa valodām un pa lappusēm
      Zem direktorijas "Sorted" redzami jau sasaistīti termini Excel izklājlapu veidā, gan atsevišķās lapās, gan visi kopā
      Pēc terminu izgūšanas, iespējams palaist terminu pagarinātāju "pagarinatajs.py"
      Pēc šīs programmas izpildes rezultāti redzami "Sorted\Test2.xlsx" izklājlapā
      Par terminu precizitāti iespējams pārliecināties palaižot programmu "salidzinatajs.py", kas salīdzina temrinus ar manuāli digitalizētiem pirms pagarināšanas
      Pēc terminu saīsinājuma pagarināšanas iespējams vēlreiz pārliecināties par precizitāti izmantojot "salidzinajums2.py" programmu
      
      
  
