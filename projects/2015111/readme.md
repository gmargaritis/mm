# Pacman

Ονοματεπώνυμο: Αλέξανδρος Δημήτριος Ζερβόπουλος

Αριθμός Μητρώου: Π2015111

Demo Pacman: https://p15zerv.github.io/pacman/

Αποθετήριο κώδικα Pacman: https://github.com/p15zerv/pacman

Το demo είναι η τρέχουσα έκδοση του παιχνιδιού, ανεξάρτητα του παραδοτέου. Ο κώδικας για κάθε παραδοτέο βρίσκεται σε ξεχωριστά branches στο αποθετήριο.

## Παραδοτέο 1

### Αποθετήριο κώδικα: https://github.com/p15zerv/pacman/tree/Deliverable1

## Παραδοτέο 2

### Αποθετήριο κώδικα: https://github.com/p15zerv/pacman/tree/Deliverable2

### Τελικό αποτέλεσμα

<img src="https://user-images.githubusercontent.com/22644005/32406041-71aa914c-c179-11e7-8b0f-a09429f0517e.PNG" alt="" width="450" height="500">

### Προσθήκες σε αυτό το παραδοτέο

#### Δημιουργία νέας πίστας μέσω Tiled

<img src="https://user-images.githubusercontent.com/22644005/32405734-964471cc-c173-11e7-91f0-3bf7b0f4e3b9.PNG" alt="" width="225" height="250">

* Αλλαγή χρωμάτων του αρχικού tileset
* Προσθήκη νέου tile στο αρχικό tileset (περαιτέρω εξήγηση παρακάτω)

#### Αλλαγή εμφάνισης του Pacman

![red2](https://user-images.githubusercontent.com/22644005/32405822-2a9a6eb6-c175-11e7-8130-5228221c597f.png)

#### Νέο αντικείμενο που μπορεί να συλλέξει ο παίκτης

<img src="https://user-images.githubusercontent.com/22644005/32405905-e5d61e2c-c176-11e7-9241-53c15a2aead4.png" alt="" width="30" height="30">

Το αντικείμενο προστίθεται στην πίστα με τη βοήθεια του νέου tile που αναφέρεται παραπάνω. Χρησιμοποιώντας την παρακάτω εντολή, αντικαθίστανται στην πίστα τα συγκεκριμένα tiles με το sprite του λουλουδιού, παίρνοντας όλα τα χαρακτηριστικά των dots.

```Javascript
this.map.createFromTiles(35, this.safetile, 'flower', this.layer, this.dots);
```

#### Προσθήκη score, χρόνου, bonus και ζωών
* Προσθήκη **χρόνου**, **score** και **high-score**, εμφανίζονται με κείμενο. 
* Προσθήκη νέου **αντικειμένου bonus**, το οποίο εμφανίζεται στην πίστα σε μία τυχαία χρονική στιγμή μεταξύ 10 και 20 seconds. Αν ο παίκτης το συλλέξει, προσθέτει 1000 στο score και καταστρέφεται. Εναλλακτικά, αν περάσουν 10 δευτερόλεπτα από τη δημιουργία του και δεν έχει συλλεχθεί, το αντικείμενο καταστρέφεται χωρίς να αυξηθεί το score του παίκτη.
* Προσθήκη **συστήματος ζωών**, εμφανίζονται με κείμενο. Μιας και σε αυτό το παραδοτέο δεν υπάρχουν ακόμα εχθροί, ο παίκτης χάνει μία ζωή όταν ο παίκτης μαζέψει όλα τα αντικείμενα στην πίστα (dots και flowers). Όταν ο παίκτης χάσει και τις 3 ζωές του, εμφανίζεται η οθόνη game over. Για να ξαναξεκινήσει το παιχνίδι, απαιτείται refresh της σελίδας.

**Υποσημείωση:** το κείμενο που χρησιμοποιείται για την εμφάνιση πληροφορίας στην οθόνη (π.χ. score και ζωές), πιθανότατα θα αντικατασταθεί στην πορεία με sprites, για να ταιριάζουν περισσότερο με την arcade αισθητική του παιχνιδιού.

#### Προσθήκη μουσικής και ηχητικών εφέ

* Προσθήκη μουσικής
* Προσθήκη ηχητικών εφέ όταν ο παίκτης συλλέγει ένα αντικείμενο ή το αντικείμενο bonus

#### Προσθήκη συστήματος αποθήκευσης

Το σύστημα αυτό επιτρέπει στον παίκτη να αποθηκεύσει την πρόοδό του. Μιας και αυτή τη στιγμή δεν υπάρχουν πολλά στοιχεία για αυτήν, το μόνο που αποθηκεύεται είναι το high-score, το οποίο γίνεται αυτόματα όταν τελειώσει η πίστα, δηλαδή όταν ο παίκτης έχει μαζέξει όλα τα αντικείμενα σε αυτήν.

Η λειτουργία αυτή δεν αναφέρεται στα παραδοτέα αλλά θεωρήθηκε χρήσιμη και επομένως υλοποιήθηκε.

__*Περισσότερες πληροφορίες υλοποίησής των παραπάνω, αλλά και links για όλα τα αρχεία που χρησιμοποιήθηκαν (sprites, sfx, κλπ), βρίσκονται σε σχόλια στα σχετικά τμήματα του κώδικα του παιχνιδιού.*__

## Παραδοτέο 3
...
## Παραδοτέο 4
...
