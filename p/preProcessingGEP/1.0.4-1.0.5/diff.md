# Comparing `tmp/preProcessingGEP-1.0.4.tar.gz` & `tmp/preProcessingGEP-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preProcessingGEP-1.0.4.tar", last modified: Tue Jul  4 19:44:05 2023, max compression
+gzip compressed data, was "preProcessingGEP-1.0.5.tar", last modified: Sat Jul 22 09:46:56 2023, max compression
```

## Comparing `preProcessingGEP-1.0.4.tar` & `preProcessingGEP-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 19:44:05.242299 preProcessingGEP-1.0.4/
--rw-rw-rw-   0        0        0       11 2023-07-04 12:45:21.000000 preProcessingGEP-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     2332 2023-07-04 19:44:05.242299 preProcessingGEP-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-07-04 19:43:10.000000 preProcessingGEP-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 19:44:05.192194 preProcessingGEP-1.0.4/preProcessingGEP/
--rw-rw-rw-   0        0        0       46 2023-07-04 19:39:21.000000 preProcessingGEP-1.0.4/preProcessingGEP/__init__.py
--rw-rw-rw-   0        0        0    20126 2023-07-04 19:39:17.000000 preProcessingGEP-1.0.4/preProcessingGEP/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-07-04 19:44:05.232660 preProcessingGEP-1.0.4/preProcessingGEP.egg-info/
--rw-rw-rw-   0        0        0     2332 2023-07-04 19:44:04.000000 preProcessingGEP-1.0.4/preProcessingGEP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-07-04 19:44:05.000000 preProcessingGEP-1.0.4/preProcessingGEP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 19:44:04.000000 preProcessingGEP-1.0.4/preProcessingGEP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-04 19:44:04.000000 preProcessingGEP-1.0.4/preProcessingGEP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 19:44:05.242299 preProcessingGEP-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      689 2023-07-04 19:39:13.000000 preProcessingGEP-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:46:56.695117 preProcessingGEP-1.0.5/
+-rw-rw-rw-   0        0        0       11 2023-07-04 12:45:21.000000 preProcessingGEP-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2332 2023-07-22 09:46:56.694120 preProcessingGEP-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-07-04 19:43:10.000000 preProcessingGEP-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 09:46:56.648114 preProcessingGEP-1.0.5/preProcessingGEP/
+-rw-rw-rw-   0        0        0       46 2023-07-04 19:39:21.000000 preProcessingGEP-1.0.5/preProcessingGEP/__init__.py
+-rw-rw-rw-   0        0        0    14233 2023-07-06 07:43:33.000000 preProcessingGEP-1.0.5/preProcessingGEP/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:46:56.688664 preProcessingGEP-1.0.5/preProcessingGEP.egg-info/
+-rw-rw-rw-   0        0        0     2332 2023-07-22 09:46:56.000000 preProcessingGEP-1.0.5/preProcessingGEP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-07-22 09:46:56.000000 preProcessingGEP-1.0.5/preProcessingGEP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 09:46:56.000000 preProcessingGEP-1.0.5/preProcessingGEP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-22 09:46:56.000000 preProcessingGEP-1.0.5/preProcessingGEP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 09:46:56.696116 preProcessingGEP-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      689 2023-07-22 09:14:17.000000 preProcessingGEP-1.0.5/setup.py
```

### Comparing `preProcessingGEP-1.0.4/PKG-INFO` & `preProcessingGEP-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preProcessingGEP
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for preprocessing text
 Home-page: https://github.com/vanshajsingla03/preProcessingGEP
 Author: Vanshaj Singla
 Author-email: vanshaj.singla@gep.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `preProcessingGEP-1.0.4/README.md` & `preProcessingGEP-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `preProcessingGEP-1.0.4/preProcessingGEP/preprocess.py` & `preProcessingGEP-1.0.5/preProcessingGEP/preprocess.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,119 @@
 from nltk.tag       import StanfordPOSTagger
 from nltk.tag       import pos_tag
 
 
 warnings.filterwarnings("ignore")
 
 class PreProcessingService:
-    def _en_stopwords():
+    def __init__(self):
+        self.punctuation = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~ ' 
+        self.punc_split_regex = re_compile(r'[\s{}]+'.format(re.escape(self.punctuation)))
+
+        self.EN_STOPWORDS = self._en_stopwords()
+        # expr to find alphanumerics starting with alpha
+        self.RE_AL_NUM = re.compile(r"([a-z]+)([0-9]+)")
+        # expr to find alphanumerics starting with numerics
+        self.RE_NUM_AL = re.compile(r"([0-9]+)([a-z]+)")
+        # expr to find all combinations of alphanumerics
+        self.RE_ALPHA_NUM = re_compile(r'(\w*\d+\w*)+(?<!\\)')
+
+        self.RE_PUNCT = re.compile(r'([%s])+' % re.escape(r"""!"#$%&'()*+,-./:;<=>?@[]^_`{|}~"""), re.UNICODE)
+        # remove numbers and return alpha string
+        self.RE_NUMERIC = re.compile(r"[0-9]+")
+        self.RE_NONALPHA = re.compile(r"\W")
+        self.RE_WHITESPACE = re.compile(r"(\s)+")
+
+        self.wordnet_lemmatizer = WordNetLemmatizer()
+        self.synonyms = [
+            "aluminum,alum,aluminium=>al",
+                        "breaker=>brkr",
+                        "barrel=>bbl",
+                        "blowdown valve=>bdv",
+                        "cam lock=>camlock",
+                        "carbon steel,cstl=>cs",
+                        "comp,cmpr,compr=>compressor",
+                        "cpl,cplg=>coupling",
+                        "crtg=>cartridge",
+                        "csg=>casing",
+                        "distributed control system=>dcs",
+                        "electric=>elec",
+                        "equipement,equip,eqpt=>equipment",
+                        "ext=>external",
+                        "flg=>flange",
+                        "fltr=>filter",
+                        "grade=>gr",
+                        "gskt=>gasket",
+                        "htr=>heater",
+                        "hvac=>heating",
+                        "hvac=>ventilation",
+                        "hvac,air conditioning=>airconditioning",
+                        "inner diameter,internal diameter,inside diameter=>id",
+                        "inner ring,i.r.,i. r.=>ir",
+                        "internal,int=>internal",
+                        "left hand=>lh",
+                        "long radius=>lr",
+                        "min=>minimum",
+                        "moly,mo=>molybdenum",
+                        "n2=>nitrogen",
+                        "nippel,nip,npl=>nipple",
+                        "nomex,fire retardant clothing,fire resistant clothing=>frc",
+                        "o ring,o-ring=>oring",
+                        "ounce,oz=>ounce",
+                        "outside diameter,outer diameter=>od",
+                        "pmp=>pump",
+                        "polyvinylchloride,polyvinyl chloride=>pvc",
+                        "pounds per square inch guage=>psig",
+                        "pressure safety valve,prv=>psv",
+                        "raised face=>rf",
+                        "rd,rnd=>round",
+                        "reciprocating=>recip",
+                        "right hand=>rh",
+                        "safety relief valve,srv,safety valve=>sv",
+                        "schedule=>sch",
+                        "skt=>socket",
+                        "smls=>seamless",
+                        "socket weld=>sw",
+                        "sodium hydroxide=>caustic",
+                        "spiral wound,sprlw=>sw",
+                        "spl=>spool",
+                        "sprl=>spiral",
+                        "sq=>square",
+                        "standard cubic feet,ft3,cuft,cu ft,cu.ft.,cu. ft.=>scf",
+                        "stsl,stainless steel,stainless,ss,304=>304ss",
+                        "stsl,stainless steel,stainless,ss,309=>309ss",
+                        "stsl,stainless steel,stainless,ss,316=>316ss",
+                        "tbg=>tubing",
+                        "thread,thrd,thd=>threaded",
+                        "threads per inch=>tpi",
+                        "trans,xfmr=>transformer",
+                        "turbo=>turbocharger",
+                        "vac=>vacuum",
+                        "vlv=>valve",
+                        "welding neck,welded neck,weld neck=>wn",
+                        "wnd=>wound",
+                        "working pressure=>wp",
+                        "xmitter,trans=>transmitter",
+                        "ml=>milliliter",
+                        "mm,mil=>millimeter",
+                        "yd=>yard",
+                        "square foot,ft2,sq ft,sq. ft.=>sqft",
+                        "gallon=>gal",
+                        "w,w=>watt",
+                        "double=>2",
+                        "inches=>inch",
+                        "cms,centimeter=>cm",
+                        "foot,ft,feet=>feet",
+                        "pound,pounds,pounds per square inch,lbs/in2,psi=>lb",
+                        "diameter=>dia"
+        ]
+        
+        
+
+    def _en_stopwords(self):
         """
         list of stopwords
         :return: list of stopwords
         """
         custom_en_stopwords = []
         nltk_en_words = 'i me my myself we our ours ourselves you your yours yourself yourselves he him his himself she her ' \
                         'hers herself itself they them their theirs themselves what which who whom this that these ' \
@@ -35,18 +139,18 @@
                 'dec febr'
         addn_stopwords = 'a about above across after afterwards again against all almost alone along already also although always am among amongst ' \
                         'amoungst amount an and another any anyhow anyone anything anyway anywhere are around as at back be became because become ' \
                         'becomes becoming been before beforehand behind being below beside besides between beyond bill both bottom but by call can ' \
                         'cannot cant co computer con could couldnt cry de describe detail do done down due during each eg eight either eleven else ' \
                         'elsewhere empty enough etc even ever every everyone everything everywhere except few fifteen fify fill find fire first five ' \
                         'for former formerly forty found four from front full further get give go had has hasnt have he hence her here hereafter ' \
-                        'hereby herein hereupon hers herse" him himse" his how however hundred i ie if in inc indeed interest into is itse" keep last ' \
+                        'hereby herein hereupon hers herse" him himse" his how however hundred i it ie if in inc indeed interest into is itse" keep last ' \
                         'latter latterly least less ltd made many may me meanwhile might mill mine more moreover most mostly move much must my myse" ' \
                         'name namely neither never nevertheless next nine no nobody none noone nor not nothing now nowhere of off often on once one ' \
-                        'only onto or other others otherwise our ours ourselves out over own part per perhaps please put rather re same see seem ' \
+                        'only onto or other others otherwise our ours ourselves out over own part per perhaps pvt please put rather re same see seem ' \
                         'seemed seeming seems serious several she should show side since sincere six sixty so some somehow someone something sometime ' \
                         'sometimes somewhere still such system take ten than that the their them themselves then thence there thereafter thereby ' \
                         'therefore therein thereupon these they thick thin third this those though three through throughout thru thus to together too ' \
                         'top toward towards twelve twenty two un under until up upon us very via was we well were what whatever when whence whenever ' \
                         'where whereafter whereas whereby wherein whereupon wherever whether which while whither who whoever whole whom whose why ' \
                         'will with within without would yet you your yours yourself yourselves exclude unclassified exclude headquaters solutions'
         global_stopwords = 'sundry clearing deductible deduct refundable adjustment cogs payble payable ' \
@@ -58,375 +162,132 @@
         # removing words less than length 3
         custom_en_stopwords.extend(global_stopwords.split(" "))
         custom_en_stopwords.extend(months.split(" "))
         custom_en_stopwords.extend(addn_stopwords.split(" "))
         return list(set(custom_en_stopwords))
 
 
-    EN_STOPWORDS = _en_stopwords()
-
 
     # note the difference between strip_* from remove_* methods
-    def strip_numeric(s):
+    def strip_numeric(self,s):
         """
         Remove numbers from input string 's'.
         :param s: string
         :return: new string
         """
         s = re.sub(r'\d+((?!\w)|(?<!\w))', '', s)
         return s
 
 
-    def strip_punctuation(s):
+    def strip_punctuation(self,s):
         """
         Remove all punctuations from input string 's'.
         :param s: string
         :return: new string
         """
-        RE_PUNCT = re.compile(r'([%s])+' % re.escape(r"""!"#$%&'()*+,-./:;<=>?@[]^_`{|}~"""), re.UNICODE)
         s = re.sub(r'\\(?!\w*\d+\w*)', ' ', s)
-        return RE_PUNCT.sub(" ", s)
+        return self.RE_PUNCT.sub(" ", s)
 
 
-    def remove_stopwords(s):
+    def remove_stopwords(self,s):
         """
         Remove all stopwords from input string 's'.
         :param s: string
         :return: new string
         """
-        return " ".join(w for w in s.split() if w not in PreProcessingService.EN_STOPWORDS)
+        return " ".join(w for w in s.split() if w not in self.EN_STOPWORDS)
 
 
-    def strip_multiple_whitespaces(s):
+    def strip_multiple_whitespaces(self,s):
         """
         remove excess whitespace
         :param s: string
         :return: new string
         """
-        RE_WHITESPACE = re.compile(r"(\s)+")
-        return RE_WHITESPACE.sub(" ", s)
+        return self.RE_WHITESPACE.sub(" ", s)
 
 
-    def strip_short(s, minsize=2):
+    def strip_short(self,s, minsize=2):
         """
         remove words <=2
         :param s: string
         :param minsize: minimum size of string
         :return: new string
         """
         return " ".join(e for e in s.split(' ') if len(e) >= minsize)
 
 
-    def remove_alpha_num(s):
+    def remove_alpha_num(self,s):
         """
         Remove alphanumerics from input string 's'.
         :param s: string
         :return: new string
         """
         return re.sub(r'\s(\w*\d+\w*)+(?<!\\)', "", s)
 
 
-    def lemmatize(toks):
+    def lemmatize(self,toks):
         """
         lemmatize the tokens of the sentence
         :param toks: list of tokens
         :return: lemmatized word list
         """
-        wordnet_lemmatizer = WordNetLemmatizer()
         lemmatized_words = [
-            wordnet_lemmatizer.lemmatize(
+            self.wordnet_lemmatizer.lemmatize(
                 word, "n") for word in toks]
         return lemmatized_words
 
 
-    def nltk_pos(tokenslist):
-        """
-        pos tag of words
-        :param tokenslist: list of words
-        :return: pos tagged list of words
-        """
-        tok_pos_tags = pos_tag(list(tokenslist), tagset='universal')
-        return tok_pos_tags
-
-
-    def stanford_pos(tokenslist):
-        """
-        different kind of pos tagger
-        :param tokenslist: list of words
-        :return: list of pos tagged words
-        """
-        try:
-            if os_name == 'nt':
-                java_path = r"C:\Program Files (x86)\Java\jre1.8.0_60\bin\java.exe"
-                environ['JAVAHOME'] = java_path
-            _pos_modelpath = nltk_find(
-                path.join('stanford-postagger', 'models', 'english-bidirectional-distsim.tagger')).path
-            _pos_jarpath = nltk_find(path.join('stanford-postagger', 'stanford-postagger.jar')).path
-        except LookupError as e:
-            print("Stanford POS Tagger jar file and model file missing or Java path not set")
-            raise
-
-        modelpos = StanfordPOSTagger(model_filename=_pos_modelpath, path_to_jar=_pos_jarpath)
-        pos_tags = modelpos.tag(tokenslist)
-        return pos_tags
-
-
-    fpos_stanford = ('NN', 'NNS', 'NNP', 'NNPS', 'JJ', 'JJR', 'JJS', 'FW')
-    fpos_nltk = ("NOUN", "ADJ", "VERB")
-
-
-    def filter_pos(token_pos_list, fpos=fpos_nltk):
-        """
-        separate words and postags
-        :param token_pos_list: words and pos tag list
-        :param fpos: list of tags
-        :return: string with words
-        """
-        fil_toks = []
-        for tok, postag in token_pos_list:
-            if postag in fpos:
-                fil_toks.append(tok)
-        return " ".join(fil_toks)
-
-
-    def clean_text(text, stopwords=EN_STOPWORDS):
-        """
-        clean the text
-        :param text: string
-        :param stopwords: list of stopwords
-        :return:
-        """
-
-        # method to split multi word tags and clean
-        # tags_str format is defined as csv values.
-        #  from word tags and append to tags and explode the sparse vector of tags
-        text = PreProcessingService.remove_alpha_num(text.lower()).strip()
-
-        # after removing
-        punctuation = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~ '  # adding space at the end
-        punc_split_regex = re_compile(r'[\s{}]+'.format(re.escape(punctuation)))
-        text_arr = punc_split_regex.split(text)
-        text_arr = filter(lambda x: x not in stopwords, text_arr)
-        text_arr = filter(None, text_arr)
-        return text_arr
-
-
-    # Last filter must be word_tokenize which returns a list of tokens
     DEFAULT_FILTERS = [lambda x: x.lower(), strip_punctuation,
-                    strip_multiple_whitespaces, strip_numeric,
-                    remove_stopwords, strip_short, remove_alpha_num, word_tokenize]
-    DEFAULT_POS_FILTERS = [nltk_pos, filter_pos]
-
+                        strip_multiple_whitespaces,strip_numeric,
+                        remove_stopwords, strip_short, word_tokenize]
 
-    def preprocess_string(s, filters=DEFAULT_FILTERS):
+    def preprocess_string(self,s,filters=DEFAULT_FILTERS):
         """
         Presprocess the string by applying functions present in list filters
         :param s: string
         :param filters: list of filters (default DEFAULT_FILTERS)
         :return: modified string
         """
 
         for f in filters:
             s = f(s)
         return ' '.join(s.split())
 
-
-    def preprocess_postags(slist, filters=DEFAULT_POS_FILTERS):
-        """
-        Take list of strings and apply functions present in list 'filters'.
-        :param slist: input list of strings
-        :param filters: list of filter functions (default DEFAULT_POS_FILTERS)
-        :return: list of filtered strings
-        """
-        for f in filters:
-            slist = f(slist)
-        return slist
-
-
-    def guided_buy_preprocess(strlist):
-        """
-        Takes list of strings to return list of filtered entities after applying functions preprocess_string and preprocess_postags
-        :param strlist: input list of strings
-        :return: list of filtered entities
-        """
-        guidedbuy_filters = [lambda x: x.lower(), PreProcessingService.strip_punctuation,
-                            PreProcessingService.strip_numeric, PreProcessingService.strip_short,
-                            PreProcessingService.remove_alpha_num, PreProcessingService.strip_multiple_whitespaces,
-                            PreProcessingService.remove_stopwords]
-        processed_list = [PreProcessingService.preprocess_string(d, guidedbuy_filters) for d in strlist]
-
-        filtered_ents = [PreProcessingService.preprocess_postags(procstr) for procstr in processed_list]
-        return filtered_ents
-
-
-    def dump_interim_steps(strlist):
-        """
-        Takes list of strings to create list of list of filtered entities and return a DataFrame with strlist, entities and filtered entities.
-        :param strlist: list of strings
-        :return: DataFrame with strlist, entities and filtered entities
-        """
-
-        # takes list of strings to return list of list of filtered entities
-        from pandas import DataFrame
-
-        guidedbuy_filters = [lambda x: x.lower(), PreProcessingService.strip_punctuation, PreProcessingService.remove_alpha_num, PreProcessingService.strip_numeric, PreProcessingService.remove_stopwords,
-                            PreProcessingService.strip_short, PreProcessingService.strip_multiple_whitespaces]
-        processed_list = [PreProcessingService.preprocess_string(d, guidedbuy_filters) for d in strlist]
-
-        entities = [PreProcessingService.stanford_pos(procstr) for procstr in processed_list]
-        fpos_stanford = ('NN', 'NNS', 'NNP', 'NNPS', 'JJ', 'JJR', 'JJS', 'FW')
-        filtered_ents = [PreProcessingService.filter_pos(procstr, fpos=fpos_stanford) for procstr in entities]
-
-        df = DataFrame({'descriptions': strlist, 'entities': entities, 'filtered_entites': filtered_ents})
-        return df
-
-
-    wordnet_lemmatizer = WordNetLemmatizer()
-
-
-    def lemmatization(string):
+    def lemmatization(self,string):
         """
         default lemmatizer
         :param string:  string
         :return: modified string
         """
         wordnet_lemmatizer = WordNetLemmatizer()
         s = [wordnet_lemmatizer.lemmatize(i.lower(), "n") for i in string.split()]
         return ' '.join(s)
 
 
-    def cold_start_preprocess(strlist):
-        """
-        preprocessor used for cold start
-        :param strlist: list of words
-        :return: modified list
-        """
-        filters = [lambda x: str(x).lower(), PreProcessingService.strip_punctuation, PreProcessingService.remove_alpha_num, PreProcessingService.strip_numeric, PreProcessingService.strip_short,
-                PreProcessingService.remove_stopwords, PreProcessingService.lemmatization, PreProcessingService.strip_multiple_whitespaces, PreProcessingService.strip_short]
-        processed_list = [PreProcessingService.preprocess_string(d, filters) for d in strlist]
-        return processed_list
-
-
-    def unique_value_col(s):
-        """
-        split words based on '|'.
-        :param s: string
-        :return: modified string
-        """
-        return ' '.join(list(s.split('|')))
-
-
-    FILTERS = [lambda x: str(x).lower(), strip_punctuation, remove_alpha_num, strip_numeric, strip_short,
-            remove_stopwords, lemmatization, strip_multiple_whitespaces, strip_short]
-
-
-    
-    def convert_synonyms(synonyms):
+    def convert_synonyms(self,synonyms):
         converted_synonyms = {}
         for entry in synonyms:
             words, rhs = entry.split("=>")
             words = [word.strip() for word in words.split(",")]
             for word in words:
                 converted_synonyms[word] = rhs.strip()
         return converted_synonyms
 
 
-    def clean_description(cat_str):
+    def clean_description(self,cat_str):
         """
         Apply filer functions present in 'FILTERS' to the input string 'cat_str'
         :param cat_str: input string
         :return: preprocessed string 'preprocess_string'
         """
-        ########################### synonyms
-        synonyms = [
-            "aluminum,alum,aluminium=>al",
-                        "breaker=>brkr",
-                        "barrel=>bbl",
-                        "blowdown valve=>bdv",
-                        "cam lock=>camlock",
-                        "carbon steel,cstl=>cs",
-                        "comp,cmpr,compr=>compressor",
-                        "cpl,cplg=>coupling",
-                        "crtg=>cartridge",
-                        "csg=>casing",
-                        "distributed control system=>dcs",
-                        "electric=>elec",
-                        "equipement,equip,eqpt=>equipment",
-                        "ext=>external",
-                        "flg=>flange",
-                        "fltr=>filter",
-                        "grade=>gr",
-                        "gskt=>gasket",
-                        "htr=>heater",
-                        "hvac=>heating",
-                        "hvac=>ventilation",
-                        "hvac,air conditioning=>airconditioning",
-                        "inner diameter,internal diameter,inside diameter=>id",
-                        "inner ring,i.r.,i. r.=>ir",
-                        "internal,int=>internal",
-                        "left hand=>lh",
-                        "long radius=>lr",
-                        "min=>minimum",
-                        "moly,mo=>molybdenum",
-                        "n2=>nitrogen",
-                        "nippel,nip,npl=>nipple",
-                        "nomex,fire retardant clothing,fire resistant clothing=>frc",
-                        "o ring,o-ring=>oring",
-                        "ounce,oz=>ounce",
-                        "outside diameter,outer diameter=>od",
-                        "pmp=>pump",
-                        "polyvinylchloride,polyvinyl chloride=>pvc",
-                        "pounds per square inch guage=>psig",
-                        "pressure safety valve,prv=>psv",
-                        "raised face=>rf",
-                        "rd,rnd=>round",
-                        "reciprocating=>recip",
-                        "right hand=>rh",
-                        "safety relief valve,srv,safety valve=>sv",
-                        "schedule=>sch",
-                        "skt=>socket",
-                        "smls=>seamless",
-                        "socket weld=>sw",
-                        "sodium hydroxide=>caustic",
-                        "spiral wound,sprlw=>sw",
-                        "spl=>spool",
-                        "sprl=>spiral",
-                        "sq=>square",
-                        "standard cubic feet,ft3,cuft,cu ft,cu.ft.,cu. ft.=>scf",
-                        "stsl,stainless steel,stainless,ss,304=>304ss",
-                        "stsl,stainless steel,stainless,ss,309=>309ss",
-                        "stsl,stainless steel,stainless,ss,316=>316ss",
-                        "tbg=>tubing",
-                        "thread,thrd,thd=>threaded",
-                        "threads per inch=>tpi",
-                        "trans,xfmr=>transformer",
-                        "turbo=>turbocharger",
-                        "vac=>vacuum",
-                        "vlv=>valve",
-                        "welding neck,welded neck,weld neck=>wn",
-                        "wnd=>wound",
-                        "working pressure=>wp",
-                        "xmitter,trans=>transmitter",
-                        "ml=>milliliter",
-                        "mm,mil=>millimeter",
-                        "yd=>yard",
-                        "square foot,ft2,sq ft,sq. ft.=>sqft",
-                        "gallon=>gal",
-                        "w,w=>watt",
-                        "double=>2",
-                        "inches=>inch",
-                        "cms,centimeter=>cm",
-                        "foot,ft,feet=>feet",
-                        "pound,pounds,pounds per square inch,lbs/in2,psi=>lb",
-                        "diameter=>dia"
-        ]
-        FILTERS = [lambda x: str(x).lower(), PreProcessingService.strip_punctuation, PreProcessingService.remove_alpha_num, PreProcessingService.strip_numeric, PreProcessingService.strip_short,
-            PreProcessingService.remove_stopwords, PreProcessingService.lemmatization, PreProcessingService.strip_multiple_whitespaces, PreProcessingService.strip_short]
-        preprocessedString=PreProcessingService.preprocess_string(cat_str, FILTERS)
-        converted_synonyms = PreProcessingService.convert_synonyms(synonyms)
+        FILTERS = [lambda x: str(x).lower(), self.strip_punctuation, self.strip_numeric, self.strip_short,
+            self.remove_stopwords, self.lemmatization, self.strip_multiple_whitespaces, self.strip_short]
+        preprocessedString=self.preprocess_string(cat_str, FILTERS)
+        converted_synonyms = self.convert_synonyms(self.synonyms)
         converted_text = " ".join([converted_synonyms.get(word, word) for word in preprocessedString.split()])
         return converted_text
```

### Comparing `preProcessingGEP-1.0.4/preProcessingGEP.egg-info/PKG-INFO` & `preProcessingGEP-1.0.5/preProcessingGEP.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preProcessingGEP
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for preprocessing text
 Home-page: https://github.com/vanshajsingla03/preProcessingGEP
 Author: Vanshaj Singla
 Author-email: vanshaj.singla@gep.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `preProcessingGEP-1.0.4/setup.py` & `preProcessingGEP-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="preProcessingGEP",
-    version="1.0.4",
+    version="1.0.5",
     author="Vanshaj Singla",
     author_email="vanshaj.singla@gep.com",
     description="A package for preprocessing text",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vanshajsingla03/preProcessingGEP",
     packages=["preProcessingGEP"],
```

