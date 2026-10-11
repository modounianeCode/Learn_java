# Apprendre Java — ton guide complet 📌

📌 **Ce projet = ta salle d'entraînement Java (Java 25, sans Maven, compilation `javac`).**
111 exercices corrigés dans `src/`, 24 énoncés pour pratiquer (`EXERCICES.md`), 12 inédits pour te tester (`INTERRO.md`).

## 🚀 1. Démarrage rapide (à faire en 5 minutes)

```bash
# 1. Vérifie Java (il faut 25+) :
java -version && javac -version

# 2. Compile TOUT le projet (depuis la racine) :
javac -d out $(find src -name "*.java")

# 3. Lance un premier programme :
java -cp out src.instructionsDeControles.FizzBuzz

# 4. Lance un test (le -ea est OBLIGATOIRE pour les assert) :
java -ea -cp out src.verification.VerifRectangle
```

✅ Si tu vois `FizzBuzz` défiler et `✅ Tous les tests Rectangle sont verts !`, ton poste est prêt.
⚠️ `out/` est ignoré par git (voir `.gitignore`) : recompile après chaque modification, c'est normal.

## 🗺️ 2. Carte du projet

| Dossier | Ce que tu y apprends |
|---|---|
| `src/generalites` | Premier programme, variables, conversions |
| `src/instructionsDeControles` | `if/else`, `switch`, boucles `for/while/do`, jeux |
| `src/tableaux` | Tableaux 1D/2D, moyennes |
| `src/chaines` | `String`, `split`, `StringBuilder`, text blocks |
| `src/classes_objets` | Classes, constructeurs, `this`, `static`, encapsulation |
| `src/heritage` | `extends`, `super`, `abstract`, polymorphisme |
| `src/interfaces` | `interface`, `implements` |
| `src/enums` | `enum`, `switch` moderne |
| `src/records` | `record` (données immuables) |
| `src/generiques` | `Boite<T>`, méthodes génériques, wildcards |
| `src/collections` | `ArrayList`, `HashMap`, `HashSet` |
| `src/tri` | `Comparator`, `TreeSet` |
| `src/queue` | `ArrayDeque`, `PriorityQueue` |
| `src/streams` | `filter/map/sorted`, `groupingBy`, lambdas |
| `src/fonctionnel` | `Predicate/Function/Consumer/Supplier` |
| `src/optionnel` | `Optional` (adieu les `NullPointerException`) |
| `src/exceptions` | `try/catch/finally`, exceptions perso |
| `src/fichiers` | `Files`, `BufferedReader/Writer`, sérialisation |
| `src/dates` | `LocalDate`, `Period`, formatage français |
| `src/threads` | `Thread` + `ExecutorService` |
| `src/regex` | `Pattern` (téléphone SN, email, mot de passe) |
| `src/patterns` | Strategy, Singleton |
| `src/inner` | Classes internes (4 sortes) |
| `src/verification` | Tests `assert` (lancer avec `-ea`) |

📌 Chaque fichier = 1 exercice autonome, style `package src.xxx;` + `static void main()` + `Scanner` pour la saisie.

## 📌 3. Ta méthode de travail (à suivre pour CHAQUE exercice)

1. 📌 **Lis l'énoncé** dans `EXERCICES.md` (ne regarde JAMAIS le corrigé avant).
2. 🚀 **Code** ton fichier au bon endroit (`src/tonpackage/TonExercice.java`) avec le bon `package`.
3. ✅ **Compile** : `javac -d out $(find src -name "*.java")` — zéro erreur exigée.
4. ✅ **Exécute** avec l'exemple de l'énoncé + UN cas limite (vide, zéro, négatif, invalide).
5. 📌 **Compare** : ouvre SEULEMENT maintenant le corrigé voisin, note les différences.
6. ❓ **Bloqué +30 min ?** Regarde UN SEUL corrigé du même thème, puis refais l'exercice SANS le recopier.

## 🗓️ 4. Parcours ordonné (ne saute pas d'étape !)

### Étape 1 — Bases 📌 (vise 6/8 dans `EXERCICES.md` niveau 1)
1. `src/generalites` : PremierProgramme → Parite → Racines → Conver → Decalage
2. `src/instructionsDeControles` : Tva → Switch1 → Factorielle → TableMultiplication → FizzBuzz → DevineNombre
3. `src/tableaux` : Moyenne → TabPoint → tab2indl
4. `src/chaines` : Palindrome → CompteVoyelles
5. `src/classes_objets` : Point → TstCerc → CompteBancaire → Rectangle
6. `src/heritage` : Pointcol → Poly → Forme/CercleF/RectangleF/TstForme
7. `src/exceptions` : DivisionSecurisee
8. `src/collections` : GestionNotes → Annuaire
9. `src/fichiers` : SauvegardePrenoms
10. 📌 Fais ensuite les **n°1 à 8 de `EXERCICES.md`**.

### Étape 2 — Maîtrise 🚀 (vise 6/8 niveau 2)
`interfaces` → `enums` → `generiques/Boite` → `streams/FiltrageNotes` → `threads/CourseThreads` → `verification` (`-ea`) → `records/Etudiant` → `regex téléphone` → `collections/PointsUniques` → `threads/CourseExecutor`.
📌 Fais ensuite les **n°9 à 16 de `EXERCICES.md`**.

### Étape 3 — Tout Java 🏆 (vise 6/8 niveau 3)
`dates` → `fonctionnel` → `optionnel` → `tri` → `queue` → exception perso → `try-with-resources` → sérialisation → méthodes génériques → classes internes → Strategy → Singleton → regex email → `StringBuilder` → `groupingBy`.
📌 Fais ensuite les **n°17 à 24 de `EXERCICES.md`**.

### Étape 4 — Examen 🏆
`INTERRO.md` en conditions réelles : 3h, `src/` INTERDIT, barème /12. `>= 10` = Java validé ✅.

## 📝 5. Suivi de progression (coche au fur et à mesure)

- 📌 Étape 1 : corrigés lus `[ ]` / exos 1-8 réussis `[ ]` (note : __/8)
- 🚀 Étape 2 : corrigés lus `[ ]` / exos 9-16 réussis `[ ]` (note : __/8)
- 🏆 Étape 3 : corrigés lus `[ ]` / exos 17-24 réussis `[ ]` (note : __/8)
- 🏆 Interro : note __/12, mention : __________

📌 Recopie ce tableau dans un carnet et mets la date à chaque case cochée.

## 🔧 6. Dépannage (erreurs fréquentes)

| Erreur | Cause | Solution |
|---|---|---|
| `javac: file not found` | Pas à la racine du projet | `cd` dans le dossier qui contient `src/`, recommence |
| `NoSuchMethodError: main` | Mauvais `main` | Vérifie `static void main()` (sans `String[]` ici, style Java 25 du projet) |
| `ClassNotFoundException` | Mauvais `-cp` ou nom | `java -cp out src.monpackage.MaClasse` (nom complet avec package) |
| Tests `assert` silencieux | `-ea` oublié | Toujours `java -ea -cp out ...` pour `src/verification` |
| `InputMismatchException` | Texte au lieu de nombre | Relance et entre un nombre ; pense à `entre.nextLine()` après `nextInt()` |
| `DateTimeParseException` | Mauvais format de date | Respecte `JJ/MM/AAAA` (ex `15/03/2005`) |
| Fichier `.txt`/`.ser` introuvable | Lancé depuis un autre dossier | Les fichiers se créent là où tu lances `java` ; reste à la racine |

## 🏆 7. Règles d'or

- 📌 Un exercice = un fichier, compilé et testé AVEC un cas limite.
- 🚀 Jamais de copier-coller de corrigé : recopie à la main en comprenant.
- ⚠️ `Scanner` : après `nextInt()`/`nextDouble()`, ajoute `nextLine()` pour vider le buffer.
- ✅ Nommage : classes en `Majuscule`, packages existants, pas d'accents dans le code.
- ❓ Demande-moi « corrige + ton code » quand tu veux une notation copie par copie.

## 📚 8. Référence des corrigés (à consulter APRÈS l'effort)

### Niveau 2

| Fichier | Notion | Sortie attendue |
|---|---|---|
| `src.interfaces.TstPayable` | `interface`, `implements` | `Awa -> 350000.0 FCFA` / `Moussa (freelance) -> 250000.0 FCFA` / `Masse salariale : 1000000.0 FCFA` |
| `src.enums.TstSaison` (entrée `7`) | `enum` + `switch` | `Saison : ETE (chaude)` + liste des 4 saisons |
| `src.generiques.TstBoite` | `Boite<T>` sans cast | `Boite de String : Bonjour Dakar` / `Boite de Integer : 42` |
| `src.streams.FiltrageNotes` | `stream/filter/sorted/map` | `Admises : [11.0, 12.0, 16.5, 19.0]` / `Moyenne : 11.21...` |
| `src.threads.CourseThreads` | `Thread`, `join` | Étapes entrelacées (ordre variable ⚠️) puis `Course terminée.` |
| `src.verification.VerifRectangle` (`-ea`) | `assert` | `✅ Tous les tests Rectangle sont verts !` |
| `src.records.TstEtudiant` | `record`, tri, `HashSet` | `Major : Etudiant[nom=Awa, moyenne=16.5]` |
| `src.verification.VerifPoint` (`-ea`) | `toString/equals/hashCode` | `✅ Tous les tests Point sont verts ! Point(x=3, y=5)` |
| `src.verification.VerifAnnuaire` (`-ea`) | regex `Pattern` | `✅ Tous les tests Annuaire (regex) sont verts !` |
| `src.threads.CourseExecutor` | `ExecutorService`, `Future` | `ARRIVÉ !` + `Course terminée (ExecutorService).` |
| `src.collections.PointsUniques` | `HashSet` | `Liste (6)` → `Set (4 uniques)` |

### Niveau 3

| Fichier | Notion | Sortie attendue |
|---|---|---|
| `src.dates.AgeExact` (`15/03/2005`) | `LocalDate`, `Period` | `Âge : 21 ans, 6 mois, 25 jours` + `mardi` |
| `src.fonctionnel.LambdasDemo` | `Predicate/...`, `->`, `::` | `[Moussa, Fatou, Ibra]` → triés `[Ibra, Fatou, Moussa]` |
| `src.optionnel.PrixOptionnel` | `Optional` | `Riz 5kg : 3500.0` / `Lait 1L : 0.0` |
| `src.tri.TriEtudiants` | `Comparator`, `TreeSet` | `Podium (4)`, premier Awa 16.5 |
| `src.queue.FileAttente` | `ArrayDeque`, `PriorityQueue` | Soin `Awa(1) → Fatou(2) → Moussa(3)` |
| `src.exceptions.CompteSecurise` | exception checked | `❌ Refusé : Solde 35000.0 FCFA insuffisant...` |
| `src.fichiers.JournalBord` | `try-with-resources` | `✅ Noté dans .../journal.txt` |
| `src.fichiers.SauvegardeObjet` | `Serializable` | `✅ Sauvegardé` + `✅ Relu : Personne(nom=Awa, age=25)` |
| `src.generiques.MethodesGeneriques` | `<T>`, wildcards | `max(3,7)=7`, `somme=42.5` |
| `src.inner.ClassesInternes` | 4 classes internes | `🔔 DRING ! Fin des cours.` |
| `src.patterns.StrategieRemise` | Strategy | `15000` → `13500` (étudiant) / `13000` (gros) |
| `src.patterns.ConfigSingleton` | Singleton | `Même instance ? true` |
| `src.regex.ValidationEmail` | regex email | `✅ awa@ecole.sn`, `❌ pas-un-email` |
| `src.chaines.StringBuilderDemo` | `StringBuilder`, text block | `Bonjour Modou, Bienvenue au club...` |
| `src.streams.CompteMots` | `groupingBy/counting` | `{bonjour=3, ...}`, top `bonjour x3` |

### Niveau 1 (extraits)

- `Factorielle` (`5`) : `5! = 120` (for + while) | `Palindrome` (`radar`) : palindrome ✅
- `CompteBancaire` : `50000` → refus `100000` → `55000` | `Rectangle` : aire `20.0`, `2` créés
- `TstForme` : totale `42.77...` | `DivisionSecurisee` (`10/0`) : erreur gérée + `finally`
- `TableMultiplication` (`7`) : `7 x 10 = 70`, somme pairs `210`

## ❓ 9. Et après ?

- 📌 Java validé (`>= 10` à l'interro) ? Passe aux projets : mini-banque console, gestion d'école avec fichiers, jeu complet.
- 🚀 Reviens me voir avec « corrige + ton code » pour la notation, ou « nouveau défi : <thème> » pour aller plus loin (JDBC, réseau, tests JUnit).
- 🏆 Bon courage — on s'arrête ici pour aujourd'hui, à toi de jouer ! 🎉
