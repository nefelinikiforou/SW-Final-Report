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
***\*** **Σημείωση\:** Παραδοτέο 1 και Παραδοτέο 2: Οι αλλαγές στον κώδικα φαίνονται στο branch [gh-pages](https://github.com/nefelinikiforou/D3js-uk-political-donations/tree/gh-pages) του παραπάνω αποθετηρίου. Το master branch χρησιμοποιήθηκε αποκλειστικά για τα ζητούμενα που απαιτούσαν αλλαγές (pull request) στο κοινό αποθετήριο του κώδικα.*

### Πίνακας Περιεχομένων
  * [Σύνοψη](https://github.com/nefelinikiforou/SW-Final-Report/blob/master/README.md#%CE%A3%CF%8D%CE%BD%CE%BF%CF%88%CE%B7)
  * [Εισαγωγή](https://github.com/nefelinikiforou/SW-Final-Report/blob/master/README.md#%CE%95%CE%B9%CF%83%CE%B1%CE%B3%CF%89%CE%B3%CE%AE)
  * [Aνάλυση σχετικών έργων και εργαλείων](https://github.com/nefelinikiforou/SW-Final-Report/blob/master/README.md#a%CE%BD%CE%AC%CE%BB%CF%85%CF%83%CE%B7-%CF%83%CF%87%CE%B5%CF%84%CE%B9%CE%BA%CF%8E%CE%BD-%CE%AD%CF%81%CE%B3%CF%89%CE%BD-%CE%BA%CE%B1%CE%B9-%CE%B5%CF%81%CE%B3%CE%B1%CE%BB%CE%B5%CE%AF%CF%89%CE%BD)
  * [Mέθοδος και τεχνικές ανάπτυξης](https://github.com/nefelinikiforou/SW-Final-Report/blob/master/README.md#m%CE%AD%CE%B8%CE%BF%CE%B4%CE%BF%CF%82-%CE%BA%CE%B1%CE%B9-%CF%84%CE%B5%CF%87%CE%BD%CE%B9%CE%BA%CE%AD%CF%82-%CE%B1%CE%BD%CE%AC%CF%80%CF%84%CF%85%CE%BE%CE%B7%CF%82)
  * [Aποτελέσματα](https://github.com/nefelinikiforou/SW-Final-Report/blob/master/README.md#a%CF%80%CE%BF%CF%84%CE%B5%CE%BB%CE%AD%CF%83%CE%BC%CE%B1%CF%84%CE%B1)
  * [Bιβλιογραφία και σύνδεσμοι σε σχετικές εργασίες](https://github.com/nefelinikiforou/SW-Final-Report/blob/master/README.md#b%CE%B9%CE%B2%CE%BB%CE%B9%CE%BF%CE%B3%CF%81%CE%B1%CF%86%CE%AF%CE%B1-%CE%BA%CE%B1%CE%B9-%CF%83%CF%8D%CE%BD%CE%B4%CE%B5%CF%83%CE%BC%CE%BF%CE%B9-%CF%83%CE%B5-%CF%83%CF%87%CE%B5%CF%84%CE%B9%CE%BA%CE%AD%CF%82-%CE%B5%CF%81%CE%B3%CE%B1%CF%83%CE%AF%CE%B5%CF%82)
  
## Σύνοψη
Το παρόν έγγραφο αποτελεί την τελική αναφορά της εξαμηνιαίας εργασίας με τίτλο "Οπτικοποίηση δεδομένων χορηγιών (UK)" της φοιτήτριας Μαρία-Νεφέλη Νικηφόρου (ΑΜ Π2015054), η οποία εντάσσεται στα πλαίσια του μαθήματος "Τεχνολογία Λογισμικού" του ΣΤ' Εαρινού Εξαμήνου 2018 με διδάσκων τον κ. Χωριανόπουλο.

Σκοπός της εργασίας είναι η εξοικείωση με τη χρήση της βιβλιοθήκης D3 της javascript για οπτικοποίηση δεδομένων, χρησιμοποιώντας παράλληλα τις σελίδες github pages. Επιπλέον, η εργασία στοχεύει στην προσαρμογή των πληροφοριών της ιστοσελίδας στις ανάγκες των χρηστών-αναγνωστών με προβλήματα όρασης, αξιοποιώντας τις δυνατότητες της γλώσσας javascript για λειτουργίες μεγέθυνσης κειμένου και text-to-speech.

Η εργασία υλοποιείται, έχοντας ως βάση το σχετικό [αποθετήριο του github](https://github.com/ioniodi/D3js-uk-political-donations), το οποίο [οπτικοποιεί](https://ioniodi.github.io/D3js-uk-political-donations/full-viz.html) τα στατιστικά στοιχεία των δωρεών που έχουν γίνει σε πολιτικά κόμματα της Μεγάλης Βρετανίας.

## Εισαγωγή

## Aνάλυση σχετικών έργων και εργαλείων
## Mέθοδος και τεχνικές ανάπτυξης
## Aποτελέσματα
## Bιβλιογραφία και σύνδεσμοι σε σχετικές εργασίες
* [Αποθετήριο](https://github.com/neilhawkins/d3-uk-political-donations) και [ιστοσελίδα](http://neilhawkins.github.io/d3-uk-political-donations/full-viz.html)
