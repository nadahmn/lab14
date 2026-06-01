# lab14
SecureStorageLabJava
https://img.shields.io/badge/Android-24%252B-brightgreen
https://img.shields.io/badge/Java-8%252B-orange
https://img.shields.io/badge/License-MIT-yellow.svg

📱 Description
Application Android démontrant toutes les méthodes de persistance locale avec bonnes pratiques de sécurité.

🎯 Fonctionnalités
SharedPreferences - Stockage non sensible (thème, langue, nom)

EncryptedSharedPreferences - Stockage chiffré des tokens/secrets

Stockage interne - Fichiers texte UTF-8 + JSON

Cache - Données temporaires purgeables

Stockage externe app-specific - Export contrôlé sans permission

🏗️ Structure
text
app/src/main/java/com/example/securestoragejava/
├── ui/MainActivity.java
├── prefs/AppPrefs.java + SecurePrefs.java
├── files/InternalTextStore.java + StudentsJsonStore.java
├── cache/CacheStore.java
├── external/ExternalAppFilesStore.java
└── model/Student.java
🚀 Installation
bash
git clone https://github.com/votreusername/SecureStorageLabJava.git
Ajouter la dépendance (déjà présente) :

gradle
implementation "androidx.security:security-crypto:1.1.0-alpha06"
🔒 Sécurité (10 points)
Point	Statut
Aucun token dans Logcat	✅
EncryptedSharedPreferences pour secrets	✅
MODE_PRIVATE partout	✅
Champ token en textPassword	✅
Nettoyage complet disponible	✅
Cache réservé au temporaire	✅
Externe limité à app-specific	✅
Exceptions gérées sans fuite	✅
UTF-8 pour tous les fichiers	✅
Affichage longueur token uniquement	✅
📱 Interface
Action	Description
Sauvegarder prefs	Nom + langue + thème + token chiffré
Charger prefs	Restauration des préférences
Sauvegarder JSON	Crée students.json et note.txt
Charger JSON	Lit et affiche les données
Effacer	Purge complète (prefs + fichiers + cache)
🐛 Dépannage rapide
Problème	Solution
Crypto non trouvé	Sync Gradle
Crash encryption	API 24+ requis
Fichiers invisibles	Vérifier /data/data/<package>/files/
JSON vide	Sauvegarder d'abord
📄 Licence
MIT

👩‍🏫 Crédits
MLIAEdu - Cours Programmation Mobile Android Java

