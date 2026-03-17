

\## `flutter/apk.md`



La documentació oficial de Flutter indica que per generar una APK es pot fer servir `flutter build apk`, i per generar binaris separats per arquitectura es pot usar `--split-per-abi`; per a Play Store, també és habitual generar un Android App Bundle amb `flutter build appbundle`.\[5]



```md

\# Generar APK i AAB a Flutter



\## Comprovar l'entorn



```bash

flutter doctor



\##Obtenir depenències

flutter pub get





\##Generar APK reléase

flutter build apk



\## Generar APK separada per arquitectura

flutter build apk --split-per-abi





\## 1. Compila projecte



npm run build



\## 2. Instal·la Capacitor



\# Instal·la el nucli de Capacitor

npm i @capacitor/core @capacitor/cli



\# Inicialitza Capacitor (posa-li el nom que vulguis a l'app)

npx cap init



\## 3. Afegeix la plataforma Android

npm i @capacitor/android

npx cap add android



\## 4. Sincronitza el codi

npm run build

npx cap copy



\## 5. Genera l'APK amb Android Studio

npx cap open Android



\##===========================

\##RECOMPILAR PROJECTE ANDROID

\##===========================

\# Desde Visual Studio

\# Netejar i tornar a construir

npm run build

npx cap sync android



\# Si això no funciona, prova amb:

npx cap copy android









