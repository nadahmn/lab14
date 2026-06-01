# SecureStorageLabJava

[![Android](https://img.shields.io/badge/Android-24%2B-brightgreen)](https://developer.android.com)
[![Java](https://img.shields.io/badge/Java-8%2B-orange)](https://www.java.com)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## 📖 Description

Application éducative Android démontrant toutes les méthodes de persistance locale avec des bonnes pratiques de sécurité strictes. Projet réalisé dans le cadre du cours **Programmation Mobile : Android avec Java** de **MLIAEdu**.

## 🎯 Objectifs pédagogiques

- Écrire/lire des préférences avec SharedPreferences (apply vs commit)
- Stocker des secrets chiffrés avec EncryptedSharedPreferences + MasterKey
- Manipuler des fichiers internes (UTF-8 et JSON)
- Utiliser le cache temporaire (cacheDir)
- Exporter vers le stockage externe app-specific
- Appliquer une checklist de sécurité complète

## 🛠️ Technologies

| Technologie | Version |
|-------------|---------|
| Android SDK | 24+ (Nougat) |
| Langage | Java 8+ |
| Sécurité | AndroidX Security Crypto 1.1.0-alpha06 |
| JSON | org.json (intégré) |

## 📁 Architecture

com.example.securestoragejava/
│
├── ui/
│ └── MainActivity.java # Interface principale
│
├── prefs/
│ ├── AppPrefs.java # SharedPreferences classiques
│ └── SecurePrefs.java # EncryptedSharedPreferences
│
├── files/
│ ├── InternalTextStore.java # Fichiers texte UTF-8
│ └── StudentsJsonStore.java # Stockage JSON
│
├── cache/
│ └── CacheStore.java # Gestion du cache
│
├── external/
│ └── ExternalAppFilesStore.java # Stockage externe
│
└── model/
└── Student.java # Modèle de données


## 🚀 Installation

### 1. Cloner le projet

<img width="1207" height="734" alt="image" src="https://github.com/user-attachments/assets/58c33126-5740-41bd-b341-cc00c565fc3a" />
