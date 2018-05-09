# Τεχνολογία Λογισμικού
## Οπτικοποίηση δεδομένων χορηγιών (UK)

#### Στοιχεία φοιτητή
##### Ονοματεπώνυμο: Μαρία-Νεφέλη Νικηφόρου
##### Αριθμός Μητρώου: Π2015054
##### Εξάμηνο φοίτησης: ΣΤ'
##### github username: nefelinikiforou
##### email: p15niki@ionio.gr

#### Σύνδεσμοι
##### Link ιστοσελίδας της εφαρμογής μου: [Link εκτελέσιμου](https://nefelinikiforou.github.io/D3js-uk-political-donations/)
##### Αποθετήριο του κώδικα της εφαρμογής (master branch) \*: [Link αποθετηρίου κώδικα](https://github.com/nefelinikiforou/D3js-uk-political-donations)
##### Link στο κλαδί του κώδικα που αντιστοιχεί στο Παραδοτέο 1 και στο Παραδοτέο 2 (gh-pages branch) \*: [Link branch κώδικα Παραδοτέων](https://github.com/nefelinikiforou/D3js-uk-political-donations/tree/gh-pages)
##### Link ιστοσελίδας της Τελικής Αναφοράς μου: [Link github-page Final Report](https://nefelinikiforou.github.io/SW-Final-Report/)
##### Αποθετήριο της Τελικής Αναφοράς μου: [Link repository Final Report](https://github.com/nefelinikiforou/SW-Final-Report)
***\*** **Σημείωση\:** Παραδοτέο 1 και Παραδοτέο 2: Οι αλλαγές στον κώδικα φαίνονται στο branch [gh-pages](https://github.com/nefelinikiforou/D3js-uk-political-donations/tree/gh-pages) του παραπάνω αποθετηρίου. Το master branch χρησιμοποιήθηκε αποκλειστικά για τα ζητούμενα που απαιτούσαν αλλαγές (pull request) στο κοινό αποθετήριο του κώδικα.*

### Πίνακας Περιεχομένων
  * Σύνοψη
  * Εισαγωγή
  * Aνάλυση σχετικών έργων και εργαλείων
  * Mέθοδος και τεχνικές ανάπτυξης
    * Παραδοτέο 1 - Ζητούμενα
    * Παραδοτέο 2 - Ζητούμενα
  * Aποτελέσματα
    * Παραδοτέο 1
    * Παραδοτέο 2
  * Συμπεράσματα
  * Bιβλιογραφία και σύνδεσμοι σε σχετικές εργασίες
    * Σχετικές εργασίες
    * Βιβλιοθήκες και πηγές κώδικα
    * Βοηθητικές ιστοσελίδες
    * Άλλα
  
## Σύνοψη
Το παρόν έγγραφο αποτελεί την τελική αναφορά της εξαμηνιαίας εργασίας με τίτλο "Οπτικοποίηση δεδομένων χορηγιών (UK)" της φοιτήτριας Μαρία-Νεφέλη Νικηφόρου (ΑΜ Π2015054), η οποία εντάσσεται στα πλαίσια του μαθήματος "Τεχνολογία Λογισμικού" του ΣΤ' Εαρινού Εξαμήνου 2018 με διδάσκων τον κ. Χωριανόπουλο.

Σκοπός της εργασίας είναι η εξοικείωση με τη χρήση της βιβλιοθήκης D3 της JavaScript για οπτικοποίηση δεδομένων, χρησιμοποιώντας παράλληλα τις σελίδες github pages. Επιπλέον, η εργασία στοχεύει στην προσαρμογή των πληροφοριών της ιστοσελίδας στις ανάγκες των χρηστών-αναγνωστών με προβλήματα όρασης, αξιοποιώντας τις δυνατότητες της γλώσσας JavaScript για λειτουργίες μεγέθυνσης κειμένου και text-to-speech.

Η εργασία υλοποιείται έχοντας ως βάση το σχετικό [αποθετήριο του github](https://github.com/ioniodi/D3js-uk-political-donations), το οποίο [οπτικοποιεί](https://ioniodi.github.io/D3js-uk-political-donations/full-viz.html) τα στατιστικά στοιχεία των δωρεών που έχουν γίνει σε πολιτικά κόμματα της Μεγάλης Βρετανίας.

## Εισαγωγή
Η οπτικοποίηση δεδομένων (data visualization) στοχεύει στην ακριβή και σαφή αναπαράσταση πληροφοριών μέσα από διαγράμματα και γραφήματα. Η αποτελεσματική οπτικοποίηση παρουσιάζει στους χρήστες πολύπλοκα δεδομένα με τέτοιο τρόπο, ώστε να είναι πιο προσιτά και κατανοητά, ενώ δίνει τη δυνατότητα στο χρήστη να εντοπίζει άμεσα μοτίβα ή/και σχέσεις και συσχετίσεις στα δεδομένα (για μία ή περισσότερες μεταβλητές). Συνεπώς, αυτός ο τρόπος οργάνωσης και αναπαράστασης των δεδομένων διευκολύνει σημαντικά το χρήστη στην εξαγωγή πληροφορίας από ένα σετ πολύπλοκων δεδομένων. Ακόμη, μεγάλο ενδιαφέρον παρουσιάζει η [ομιλία](https://www.ted.com/talks/david_mccandless_the_beauty_of_data_visualization?language=el#t-1076216) του David McCandless με τίτλο: "The beauty of data visualization" (TED talks 2010).

Στην παρούσα εργασία, η [εφαρμογή](https://nefelinikiforou.github.io/D3js-uk-political-donations/) που αναπτύσσεται αξιοποιεί τη βιβλιοθήκη D3 της JavaScript για οπτικοποίηση δεδομένων χορηγιών προς πολιτικά κόμματα της Μεγάλης Βρετανίας. Ο κώδικας βασίστηκε σε [αποθετήριο του github](https://github.com/ioniodi/D3js-uk-political-donations) (Βλ. [αποθετήριο κώδικα νέας εφαρμογής](https://github.com/nefelinikiforou/D3js-uk-political-donations/tree/gh-pages)). Διαθέτει διάφορες μορφές αναπαράστασης (κουμπιά) των δεδομένων ώστε να παρέχονται περισσότερες πληροφορίες στο χρήστη, ανάλογα με την επιλεγμένη συσχέτιση (All money, The public's purse, Split by party, Split by type of donor, Split by the amount of the donation), ενώ συνδέεται και με την υπηρεσία Google Search (κλικ σε μπάλα του γραφήματος) για την πρόσβαση σε περισσότερα στοιχεία για τον εκάστοτε δωρητή. Η χρήση χρωμάτων, ήχων, παραθύρων με πληροφορίες δωρητών (hover πάνω από μπάλα του γραφήματος) και σειράς εικόνων δωρητών (ιστορικό) κάνει την εφαρμογή πιο ελκυστική και χρήσιμη για το χρήστη. Επιπλέον, η υποστήριξη λειτουργιών όπως η μεγέθυνση κειμένου (λειτουργία ποντικιού ως μεγεθυντικός φακός με hover πάνω από το κείμενο) και η λειτουργία text-to-speech, η εφαρμογή-ιστοσελίδα προσαρμόζει τις πληροφορίες στις ανάγκες των χρηστών-αναγνωστών με προβλήματα όρασης. Η υλοποίηση όλων αυτών των στοιχείων και των λειτουργιών περιγράφεται αναλυτικά στην ενότητα "Mέθοδος και τεχνικές ανάπτυξης".


## Aνάλυση σχετικών έργων και εργαλείων
Η ιστοσελίδα μου βασίστηκε στο σχετικό [αποθετήριο του github](https://github.com/ioniodi/D3js-uk-political-donations), που [οπτικοποιεί](https://ioniodi.github.io/D3js-uk-political-donations/full-viz.html) τα στατιστικά στοιχεία των δωρεών που έχουν γίνει σε πολιτικά κόμματα της Μεγάλης Βρετανίας, και το οποίο έκανα fork ώστε να το τροποποιήσω κατάλληλα με βάση τις απαιτήσεις-ζητούμενα των παραδοτέων της εξαμηνιαίας εργασίας. Επίσης, μια παρόμοια εργασία είναι και αυτή: [Αποθετήριο](https://github.com/neilhawkins/d3-uk-political-donations) και [ιστοσελίδα](http://neilhawkins.github.io/d3-uk-political-donations/full-viz.html).

Αναφορικά με τα εργαλεία που χρησιμοποίησα, τα βασικότερα είναι η ιστοσελίδα του Github και το σύστημα Github Pages, καθώς μέσω αυτών επεξεργάστηκα τον κώδικα (αρχεία "[index.html](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/index.html)", "[chart.js](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/chart.js)" και "[style.css](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/style.css)"), επειδή μου δίνουν τη δυνατότητα να κάνω δοκιμές και να βλέπω άμεσα το αποτέλεσμα των ενεργειών μου (προσθήκες/αλλαγές/τροποποιήσεις) στην ιστοσελίδα της εφαρμογής μου. Επιπλέον, στο [API του Github](https://api.github.com/users/nefelinikiforou) βρήκα όλες τις πληροφορίες μου σαν χρήστης του Github για τα ζητούμενα που χρειάστηκε.

Για την επεξεργασία των 5 εικόνων των δωρητών που πρόσθεσα στο φάκελο [photos](https://github.com/ioniodi/D3js-uk-political-donations/tree/master/photos), χρησιμοποίησα ένα [online resizing tool](http://picresize.com/), ενώ οι εικόνες που φαίνονται στα παραδοτέα και στην τελική αναφορά είναι screenshots που έχουν δημιουργηθεί με το "Snipping Tool" των Windows.

Για τον εντοπισμό των pixels που χρειαζόμουν για να καθορίσω την ακριβή τοποθεσία διάφορων στοιχείων στην ιστοσελίδα της εφαρμογής μου, χρησιμοποίησα την επέκταση του Google Chrome, "Page Ruler". Τέλος, χρησιμοποίησα τα "Εργάλεια για Προγραμματιστές" του browser Google Chrome, προκειμένου να έχω τη δυνατότητα να ελέγχω την ορθότητα και να εντοπίζω τα σφάλματα του κώδικά μου.

Χρήσιμες βιβλιοθήκες αποτέλεσαν:
* η D3 της JavaScript.
* η [ResponsiveVoice](http://code.responsivevoice.org/responsivevoice.js) (JavaScript) για text-to-speech.
* η [βιβλιοθήκη](https://cdnjs.cloudflare.com/ajax/libs/animejs/2.0.2/anime.min.js) για το text animation (Βλ. [ιστοσελίδα participants](https://ioniodi.github.io/D3js-uk-political-donations/participants/)).


## Mέθοδος και τεχνικές ανάπτυξης
#### Παραδοτέο 1 - Ζητούμενα
* [Ιστοσελίδα εφαρμογής](https://nefelinikiforou.github.io/D3js-uk-political-donations/)

* Αλλαγή κατάληξης url της εφαρμογής μου από "full-viz.html", μετονομάζοντας το αντίστοιχο αρχείο σε "[index.html](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/index.html)":

  ![fullviz1](https://user-images.githubusercontent.com/22655733/36723280-7ea7b0fc-1bb8-11e8-9414-16dc95f95774.JPG)

  Από: https://nefelinikiforou.github.io/D3js-uk-political-donations/full-viz.html σε: https://nefelinikiforou.github.io/D3js-uk-political-donations/.

* Αλλαγή χρωμάτων στις μπάλες με τα δεδομένα:
  Χρειάστηκε να αλλάξω τους κωδικούς των χρωμάτων στο αρχείο "[chart.js](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/chart.js)"
  από: ![chart-js-code-colorballs-1](https://user-images.githubusercontent.com/22655733/36741172-1a9c1938-1bed-11e8-9526-4df6701d8d4e.JPG)
  
  σε: ![chart-js-code-colorballs-2](https://user-images.githubusercontent.com/22655733/36741327-78a919f4-1bed-11e8-9f2f-c8c84a9d3dbf.JPG)
  
  (Βλ. Εικ. 1.1., Ενότητα: "Αποτελέσματα").

* Αλλαγή χρωμάτων στα 3 πεδία της ομαδοποίησης *Split by party*:
  Χρειάστηκε να αλλάξω τους κωδικούς των χρωμάτων στο αρχείο "[style.css](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/style.css)":

  ![style-css-partycolor](https://user-images.githubusercontent.com/22655733/36935875-e8e46b86-1f05-11e8-9eb3-d2e91447b430.JPG)

  (Βλ. Εικ. 1.2., Ενότητα: "Αποτελέσματα").

* Ήχος στις επιλογές/κουμπιά ομαδοποίησης των δεδομένων (ενεργοποίηση με κλικ):
  1. Βρήκα ([εδώ](http://soundbible.com/)) και ανέβασα στο αποθετήριο της εφαρμογής μου ένα [mp3 αρχείο](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/Stapler-SoundBible.com-374581609.mp3).
  2. Στο αρχείο "[index.html](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/index.html)", έβαλα το script tag:

      ![sound1](https://user-images.githubusercontent.com/22655733/36936649-aeacefaa-1f10-11e8-9238-f31781456b76.JPG)
     και την ακόλουθη εντολή:

      ![sound2](https://user-images.githubusercontent.com/22655733/36936729-acbc9b90-1f11-11e8-9a4b-022613a8d783.JPG)
   
     στην ετικέτα <a></a> για κάθε λίστα των κουμπιών ομαδοποίησης των δεδομένων:
   
      ![sound3](https://user-images.githubusercontent.com/22655733/36936799-73156c0e-1f12-11e8-95e5-7b5429fdd520.JPG)

* Άνοιγμα νέου παραθύρου με αποτελέσματα αναζήτησης (google) για δωρητή (ενεργοποίηση με κλικ σε μπάλα):
  Στο αρχείο "[chart.js](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/chart.js)":
  1. Δημιούργησα τη συνάρτηση googleSearch(d), που έχει σαν όρισμα τα δεδομένα της εκάστοτε μπάλας (όνομα δωρητή) και με την εντολή window.open() ανοίγει ένα νέο παράθυρο με τα αποτελέσματα της αναζήτησης google για τον αντίστοιχο δωρητή:
   
      ![char-js-gsearch-funct](https://user-images.githubusercontent.com/22655733/37045497-c0958956-216e-11e8-9eed-ae070741eb7c.JPG)
  2. Συνδυάζοντας τη συνάρτηση on μαζί με τη συνάρτηση googleSearch(d), έβαλα την εξής εντολή μέσα στη συνάρτηση start():

      ![c2](https://user-images.githubusercontent.com/22655733/37046876-0d447e6c-2172-11e8-950a-6b5bebe4f353.JPG)
   
     έτσι ώστε να ενεργοποιείται η αναζήτηση όταν γίνεται κλικ σε κάποια μπάλα.
  3. Πρόσθεσα στη συνάρτηση mouseover(d, i) την εντολή:

      ![chart-js-cursor1](https://user-images.githubusercontent.com/22655733/37048053-6a7dadbc-2175-11e8-8f09-60aba3ab418d.JPG)
     
     και στη συνάρτηση mouseout() την εντολή:
      
      ![chart-js-cursor2](https://user-images.githubusercontent.com/22655733/37048165-ba8c7978-2175-11e8-81e6-38965b221d98.JPG)

   Η πρώτη εντολή μετατρέπει τον κέρσορα σε χεράκι που δείχνει (pointer) κάθε φορά που εκείνος μετακινείται πάνω από κάποια μπάλα, έτσι ώστε να φαίνεται ότι εκεί υπάρχει υπερσύνδεσμος. Η δεύτερη εντολή μετατρέπει τον κέρσορα στη default εμφάνισή του, όταν εκείνος δεν μετακινείται πάνω από κάποια μπάλα.

* Λειτουργία ποντικιού ως μεγεθυντικός φακός του κειμένου (αύξηση μεγέθους γραμματοσειράς):
  1. Στο αρχείο "[style.css](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/style.css)", έφτιαξα μια νέα κλάση zoom, η οποία αλλάζει το μέγεθος της γραμματοσειράς (font-size) σε *large* όταν το ποντίκι βρίσκεται πάνω από κείμενο (hover):

      ![zoom-style-css](https://user-images.githubusercontent.com/22655733/37148163-1c413cdc-22d2-11e8-8218-d85951c06dbc.JPG)
  2. Στο αρχείο "[index.html](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/index.html)", έβαλα το <script>:

      ![zoom-index-html](https://user-images.githubusercontent.com/22655733/37148864-97e63566-22d4-11e8-95d8-fedcfcad942c.JPG)

     Οι εντολές αυτές εντοπίζουν όλες τις ετικέτες (p, h4, h5, nav) στις οποίες θέλουμε να γίνεται η μεγέθυνση κειμένου και προσθέτουν σε αυτές την κλάση zoom. Η μεγέθυνση γίνεται ταυτόχρονα σε όλα τα κουμπιά, ανεξάρτητα από το πάνω σε ποιο ακριβώς από αυτά βρίσκεται το ποντίκι, καθώς θεώρησα ότι ο χρήστης θα θέλει να βλέπει καθαρά το σύνολο των δυνατών επιλογών (κουμπιά) που έχει, ώστε να βρίσκει άμεσα αυτό που θέλει. Επέλεξα να μη γίνεται zoom στις ετικέτες h1, h2 και h3, καθώς το κείμενό τους έχει ήδη αρκετά μεγάλο μέγεθος γραμματοσειράς και είναι bold.   
  3. Στο ίδιο αρχείο, πρόσθεσα ετικέτες < p > στα 25k, 50k, 100k, 500k, 1m (value scale), ώστε να μεγεθύνονται, καθώς έχουν αρκετά μικρό μέγεθος γραμματοσειράς και αχνό χρώμα:
      
      ![zoom2-index-html](https://user-images.githubusercontent.com/22655733/37149171-bb396df2-22d5-11e8-928f-17b447482836.JPG)

* Ήχος για την ονομασία του δωρητή και το ποσό της δωρεάς (ενεργοποίηση όταν το ποντίκι βρίσκεται μέσα σε κύκλο δωρητή):
  1. Στο τέλος του αρχείου "[index.html](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/index.html)", δήλωσα την εξωτερική βιβλιοθήκη [responsiveVoice](https://responsivevoice.org/api/):

      ![voice-link-index-html](https://user-images.githubusercontent.com/22655733/37205214-97be952e-239c-11e8-9633-cfa2e5dd4edf.JPG)
  2. Στο αρχείο "[chart.js](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/chart.js)", πρόσθεσα στη συνάρτηση mouseover(d,i) την εντολή:

      ![voice1-chart-js](https://user-images.githubusercontent.com/22655733/37206273-a843df7c-23a0-11e8-85dc-39ef3c7caf9a.JPG)
   
     Έτσι, ακούγονται οι πληροφορίες του δωρητή για όσο το ποντίκι βρίσκεται εντός του κύκλου του.
  3. Στο ίδιο αρχείο, πρόσθεσα στη συνάρτηση mouseout() την εντολή:

      ![voice2-chart-js](https://user-images.githubusercontent.com/22655733/37206301-c329bf64-23a0-11e8-8324-0d1bcd12df36.JPG)

     ώστε να σταματούν να ακούγονται οι πληροφορίες του δωρητή όταν το ποντίκι δε θα βρίσκεται πλέον μέσα στον κύκλο.

* Δημιουργία και προσθήκη νέας επιλογής ομαδοποίησης των δεδομένων (Split by the amount of the donation):
  1. Στο αρχείο "[index.html](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/index.html)": 
   * Δημιούργησα το νέο κουμπί κάτω από τα προηγούμενα της λίστας:
 
       ```
       <li><a href="#" onclick="sound.play()" role="button" class="pure-button switch" id="group-by-donation-amount">Split by the amount of the donation</a></li>
       ```
      

   * Πρόσθεσα το &lt;div id="view-donation-amount"&gt; κάτω από τα υπόλοιπα &lt;div&gt; ομαδοποίησης:
     
     ![new-div-index-html](https://user-images.githubusercontent.com/22655733/37247732-86326b82-24c8-11e8-957b-01a014dc99ba.JPG)
     
  2. Στο αρχείο "[chart.js](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/chart.js)":
   * Πρόσθεσα στη συνάρτηση transition() μία επιπλέον μετάβαση, η οποία (ενεργοποίηση με κλικ στο νέο κουμπί), φέρνει στο προσκήνιο (fadeIn) το #view-donation-amount, "κρύβει" (fadeOut) όλα τα υπόλοιπα # και επιστρέφει τη συνάρτηση amountsGroup():

       ![new-transition-chart-js](https://user-images.githubusercontent.com/22655733/37259189-d7ed4ee2-258b-11e8-8d62-d007e0942d97.JPG)
   
     Τέλος, έβαλα την εντολή:```$("#view-donation-amount").fadeOut(250);``` σε όλες τις υπόλοιπες μεταβάσεις της transition().
     
   * Έφτιαξα τη συνάρτηση amountsGroup() έχοντας ως πρότυπο τις υπόλοιπες συναρτήσεις (total(), partyGroup(), donorType(), fundsType()):

       ![func-amounts-group-chart-js](https://user-images.githubusercontent.com/22655733/37259371-f4862874-258d-11e8-8b32-4a4477ac2774.JPG)
   
      Με την εντολή: ```.on("tick", amounts)``` καλείται η συνάρτηση amounts().
      
   * Έφτιαξα τη συνάρτηση amounts() έχοντας ως πρότυπο τις υπόλοιπες συναρτήσεις (all(), parties(), entities(), types()):

       ![func-amounts-chart-js](https://user-images.githubusercontent.com/22655733/37259414-ab821d58-258e-11e8-9b9c-e7eff6161547.JPG)
       
   * Δημιούργησα τη συνάρτηση moveToAmounts(alpha), προκειμένου να μετακινηθούν οι κόμβοι στις κατάλληλες θέσεις. Ουσιαστικά, επιλέγεται ένα σταθερό κέντρο για τη θέση Y των κόμβων και, με βάση το value του κάθε κόμβου (το ποσό της δωρεάς), ορίζεται το X σε μία τιμή που αντιστοιχεί στις 6 επιλεγμένες τιμές (Donations over £1m, Donations over £500k, Donations over £100k, Donations over £50k, Donations over £25k, Donations under £25k):

       ![func-movetoamounts-chart-js](https://user-images.githubusercontent.com/22655733/37288197-4f23312e-260f-11e8-84b4-2850a0c94d0e.JPG)
       
  3. Στο αρχείο "[style.css](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/style.css)" :
   * Επέλεξα να μην εμφανίζονται αρχικά στη σελίδα τα στοιχεία της ```#view-donation-amount```:
  
       ![disappear-view-style-css](https://user-images.githubusercontent.com/22655733/37288507-26379da8-2610-11e8-8430-66c8deea4d6a.JPG)
  
   * Όρισα τις θέσεις εμφάνισης του τίτλου "Split by the amount of the donation" και των 6 τίτλων των ποσών (Donations over £1m, Donations over £500k, Donations over £100k, Donations over £50k, Donations over £25k, Donations under £25k):
   
       ![labels-style-css-1](https://user-images.githubusercontent.com/22655733/37288301-90a7795c-260f-11e8-9252-cd7175be46ef.JPG)
   
       ![labels-style-css-2](https://user-images.githubusercontent.com/22655733/37288330-aa8320a6-260f-11e8-9b38-e9925255bdb5.JPG)

     Για την εύρεση των κατάλληλων pixel, χρησιμοποίησα την επέκταση του Google Chrome, *Page Ruler*:

       ![pageruler](https://user-images.githubusercontent.com/22655733/37301526-77e6b776-2631-11e8-9680-2884296f53d8.JPG)
       
    (Βλ. Εικ. 1.3., Ενότητα: "Αποτελέσματα").

* Ζητούμενα που απαιτούν pull request
  1. Δημιούργησα το [αρχείο .csv](https://github.com/ioniodi/D3js-uk-political-donations/blob/master/participants/2015054.csv) με τα στοιχεία μου.
  2. Πρόσθεσα 5 εικόνες δωρητών στο φάκελο [photos](https://github.com/ioniodi/D3js-uk-political-donations/tree/master/photos): 
     * Bell Pottinger Group (685)
     * Betterworld (785)
     * HCA International (713)
     * Independent Print (808)
     * Seamark (705)

#### Παραδοτέο 2 - Ζητούμενα
* Εμφάνιση και δυναμική επέκταση σειράς εικόνων δωρητών (ενεργοποίηση όταν το ποντίκι βρίσκεται μέσα σε κύκλο δωρητή):

  1. Στο αρχείο "[index.html](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/index.html)", πρόσθεσα ένα νέο &lt;div&gt; tag για τη δημιουργία μιας περιοχής για τις εικόνες των δωρητών, πάνω από τους κύκλους των οποίων έχει περάσει ο δείκτης του ποντικιού του χρήστη:

      ![img_sidebar_html](https://user-images.githubusercontent.com/22655733/39702847-c625c900-520e-11e8-8de7-1d0c9c5b3cd7.JPG)
  2. Στο αρχείο "[style.css](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/style.css)", πρόσθεσα το πλαίσιο:

      ![img_sidebar_css](https://user-images.githubusercontent.com/22655733/39702982-4a2baba2-520f-11e8-8c0f-621786d98512.JPG)
   
     για να ορίσω το μέγεθος (ύψος: 42 pixels, καθώς οι εικόνες των δωρητών έχουν διαστάσεις 42x42) της περιοχής για τις εικόνες των δωρητών που έχουν προσπελαστεί, καθώς και την τοποθεσία της στην ιστοσελίδα. Με τη βοήθεια της επέκτασης του Google Chrome, *Page Ruler*, εντόπισα τα pixel για τη θέση του πλαισίου στην ιστοσελίδα:
   
      ![pixels_sidebar](https://user-images.githubusercontent.com/22655733/39742854-b438c1ae-52a7-11e8-90b0-5778f4cd379e.JPG)
   
     Χρωμάτισα το πλαίσιο προσωρινά (```background-color: light-blue;```), ώστε να ελέγχω ότι οι εικόνες τοποθετούνται σωστά:
   
      ![sidebar_1st_attempt](https://user-images.githubusercontent.com/22655733/39743105-9027a1da-52a8-11e8-8f98-ebd1602496bd.JPG)
  3. Στο αρχείο "[chart.js](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/chart.js)":
   * Όρισα μία νέα global μεταβλητή (κενό array) για να μετράω πόσες φορές έχει προσπελαστεί και εμφανιστεί η εικόνα κάθε δωρητή στο πλαίσιο, έτσι ώστε να αποφύγω την πολλαπλή εμφάνιση των ίδιων εικόνων (όταν το ποντίκι ξαναπερνάει πάνω από τον ίδιο κύκλο δωρητή):
  
      ![img_sidebar_js1](https://user-images.githubusercontent.com/22655733/39716346-c7901d84-5238-11e8-8728-79b07cc61c29.JPG)
   
   * Πρόσθεσα στη συνάρτηση mouseover(d,i):

      ![img_sidebar_js2](https://user-images.githubusercontent.com/22655733/39721439-4318e882-5248-11e8-8a2c-64f460b39af2.JPG)
      
       Με τον έλεγχο της επιστρεφόμενης τιμής της συνάρτησης dlist.indexOf(donor) να μην είναι μεγαλύτερη από -1, εξασφαλίζεται ότι θα εμφανιστούν στο πλαίσιο μόνο οι εικόνες των δωρητών που δεν έχουν ξαναεμφανιστεί. Επιπλέον, θέτω τις διαστάσεις όλων των εικόνων στα 42x42 pixels (```element.setAttribute("height", "42"); element.setAttribute("width", "42");```), προκειμένου να εμφανίζονται ομοιόμορφες. Με κάθε νέα εικόνα δωρητή, η σειρά των εικόνων επεκτείνεται δυναμικά (```document.getElementById("images-sidebar").appendChild(element); dlist.push(donor);```)
    
  4. Στο αρχείο "[style.css](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/style.css)", αφαιρώ το περιττό background color του πλαισίου:

   ![img_sidebar_css2](https://user-images.githubusercontent.com/22655733/39724828-820cd030-5252-11e8-94e0-e13b67d8af81.JPG)
   
(Βλ. Εικ. 2.1., Ενότητα: "Αποτελέσματα")
(Βλ. και [ιστοσελίδα](https://nefelinikiforou.github.io/D3js-uk-political-donations/))
      
* Ζητούμενα που απαιτούν pull request
  1. Εμφάνιση των στοιχείων μου (github username & picture) με κάποια κίνηση στην [ιστοσελίδα](https://ioniodi.github.io/D3js-uk-political-donations/participants/) με τους φοιτητές της άσκησης:

    * Δήλωσα στο [Issue του Παραδοτέου 2](https://github.com/ioniodi/D3js-uk-political-donations/issues/17) τη δέσμευση της θέσης "Position #014" στον [κώδικα](https://github.com/ioniodi/D3js-uk-political-donations/blob/master/participants/index.html) της ιστοσελίδας:

        ![issue](https://user-images.githubusercontent.com/22655733/39665515-5093f156-509e-11e8-9f47-85944c20c592.JPG)

    * Στο [API του Github](https://api.github.com/users/nefelinikiforou) βρήκα όλες τις πληροφορίες μου σαν χρήστης του Github και, συγκεκριμένα, το url για το avatar μου, το οποίο χρειάζεται ώστε να εμφανίζεται η εικόνα προφίλ μου:

        ![avatar](https://user-images.githubusercontent.com/22655733/39664939-77eeff5c-5094-11e8-8454-dd4436301b35.JPG)

        ![avatar_img](https://user-images.githubusercontent.com/22655733/39664956-c8123bac-5094-11e8-9b5c-7f3486862909.JPG)

    * Στο φάκελο [participants](https://github.com/ioniodi/D3js-uk-political-donations/tree/master/participants) μετέτρεψα το αρχείο "[index.html](https://github.com/ioniodi/D3js-uk-political-donations/blob/master/participants/index.html)" στη θέση που είχα δεσμεύσει (Position #014), αρχικά ορίζοντας το url για το avatar μου και το username μου και, έπειτα, xρησιμοποιώντας τη [βιβλιοθήκη](https://cdnjs.cloudflare.com/ajax/libs/animejs/2.0.2/anime.min.js) (την οποία εμπεριείχε ήδη το αρχείο) και μετατρέποντας κατάλληλα τον open source [κώδικα](http://tobiasahlin.com/moving-letters/#7) για text animation που βρήκα, ως εξής:

        ![avatar_index_hml_1](https://user-images.githubusercontent.com/22655733/39665012-641b37d8-5095-11e8-8d0e-de162231f886.JPG)

        ![avatar_index_html_2](https://user-images.githubusercontent.com/22655733/39665018-821f5606-5095-11e8-84b0-1143e6fb022e.JPG)

        ![avatar_index_html_3](https://user-images.githubusercontent.com/22655733/39665022-911b8d3c-5095-11e8-93ab-ef605e574eca.JPG)

   (Βλ. Εικ. 2.2., Ενότητα: "Αποτελέσματα")
   (Βλ. και [ιστοσελίδα](https://ioniodi.github.io/D3js-uk-political-donations/participants/))

  2. Ενημέρωσα το [αρχείο .csv](https://github.com/ioniodi/D3js-uk-political-donations/blob/master/participants/2015054.csv) με τα στοιχεία μου, προσθέτοντας το δεύτερο παραδοτέο.
## Aποτελέσματα
#### Παραδοτέο 1
![colorballs2](https://user-images.githubusercontent.com/22655733/36741492-ef804f0c-1bed-11e8-9fa9-08f6e26dc549.JPG)

*Εικ. 1.1. Αλλαγή χρωμάτων στις μπάλες με τα δεδομένα.*

![colorparty1](https://user-images.githubusercontent.com/22655733/36935907-79041ec8-1f06-11e8-8e61-451003c04f8f.JPG)
![colorparty2](https://user-images.githubusercontent.com/22655733/36935922-bcb6dbe2-1f06-11e8-9c1f-cbc67d4577f1.JPG)

*Εικ. 1.2. Αλλαγή χρωμάτων στα 3 πεδία της ομαδοποίησης **Split by party** (Αριστερά: Πριν την αλλαγή, Δεξιά: Μετά την αλλαγή).*

![amount-result](https://user-images.githubusercontent.com/22655733/39746245-755bdee8-52b2-11e8-9f6c-920cd02ab18b.JPG)

*Εικ. 1.3. Δημιουργία και προσθήκη νέας επιλογής ομαδοποίησης των δεδομένων (Split by the amount of the donation).*
#### Παραδοτέο 2
![final](https://user-images.githubusercontent.com/22655733/39743172-c33be73e-52a8-11e8-8273-f9c5c51c0976.JPG)

*Εικ. 2.1. Εμφάνιση και επέκταση σειράς εικόνων δωρητών.*

![anim-pict](https://user-images.githubusercontent.com/22655733/39665455-45b08e1c-509d-11e8-9620-18162508a4c8.JPG)

*Εικ. 2.2. Εμφάνιση των στοιχείων μου (github username & picture) με κάποια κίνηση στην [ιστοσελίδα](https://ioniodi.github.io/D3js-uk-political-donations/participants/) με τους φοιτητές της άσκησης.*
## Συμπεράσματα
Συνοψίζοντας, στα πλαίσια αυτής της εξαμηνιαίας εργασίας έχει υλοποιηθεί μία νέα, διαδραστική [ιστοσελίδα](https://nefelinikiforou.github.io/D3js-uk-political-donations/) σε HTML5, CSS και JavaScript (κυρίως με τη βοήθεια της βιβλιοθήκης D3 της JavaScript για οπτικοποίηση δεδομένων), βασισμένη σε μία προϋπάρχουσα [ιστοσελίδα](https://ioniodi.github.io/D3js-uk-political-donations/full-viz.html), πάνω στην οποία έγιναν όλες οι προσθήκες, οι αλλαγές και οι τροποποιήσεις. Παρέχονται οπτικοποιημένα τα στατιστικά στοιχεία των δωρεών που έχουν γίνει σε πολιτικά κόμματα της Μεγάλης Βρετανίας, καθώς και επιπλεόν λειτουργίες επί αυτών. Τέλος, στη νέα ιστοσελίδα επεκτείνονται οι δυνατότητες, η διάδραση και η λειτουργικότητα της αρχικής ιστοσελίδας και γίνεται πλέον κατάλληλη και για χρήστες-αναγνώστες με προβλήματα όρασης, μέσω των δυνατοτήτων της γλώσσας JavaScript για παροχή λειτουργιών μεγέθυνσης κειμένου και text-to-speech.

## Bιβλιογραφία και σύνδεσμοι σε σχετικές εργασίες
#### Σχετικές εργασίες
* [Αποθετήριο](https://github.com/ioniodi/D3js-uk-political-donations) και [ιστοσελίδα](https://ioniodi.github.io/D3js-uk-political-donations/full-viz.html) που βασίστηκε η δική μου εφαρμογή.
* [Αποθετήριο](https://github.com/neilhawkins/d3-uk-political-donations) και [ιστοσελίδα](http://neilhawkins.github.io/d3-uk-political-donations/full-viz.html) μιας σχετικής εργασίας.

#### Βιβλιοθήκες και πηγές κώδικα
* [D3.js](https://d3js.org/).
* [ResponsiveVoice](http://code.responsivevoice.org/responsivevoice.js) (JavaScript) και [API](https://responsivevoice.org/api/) για text-to-speech.
* [Bιβλιοθήκη](https://cdnjs.cloudflare.com/ajax/libs/animejs/2.0.2/anime.min.js) και [κώδικας](http://tobiasahlin.com/moving-letters/#7) για το text animation.
* [Πηγή ήχου κουμπιών](http://soundbible.com/) και [mp3 αρχείο](https://github.com/nefelinikiforou/D3js-uk-political-donations/blob/gh-pages/Stapler-SoundBible.com-374581609.mp3).

#### Βοηθητικές ιστοσελίδες
* Hex και RBG [κωδικοί χρωμάτων](https://htmlcolorcodes.com/).
* [Zoom on hover CSS](https://www.w3schools.com/howto/howto_css_zoom_hover.asp).
* [.addClass() documentation](https://api.jquery.com/addclass/).
* [Item in array search JavaScript](https://www.w3schools.com/jsref/jsref_indexof_array.asp).
* [Αrray push JavaScript](https://www.w3schools.com/jsref/jsref_push.asp).
* [Image object HTML](https://www.w3schools.com/jsref/dom_obj_image.asp) και [Image element JavaScript](http://www.java2s.com/Code/JavaScript/HTML/Imageelement.htm).
* [Access specific element HTML](https://www.w3schools.com/jsref/met_document_getelementbyid.asp).
* [Append node HTML](https://www.w3schools.com/jsref/met_node_appendchild.asp).

#### Άλλα
* Ενδιαφέρουσα [ομιλία](https://www.ted.com/talks/david_mccandless_the_beauty_of_data_visualization?language=el#t-1076216) του David McCandless για Data Visualization (TED talks 2010).
