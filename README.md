# Yuki Desktop 2D — documents et dépendances

Ce dépôt contient uniquement les documents publics de confidentialité et support, et les références des bibliothèques redistribuées. Il ne contient ni le code de Yuki, ni ses images, sprites, dialogues ou lettres.

- [Confidentialité](PRIVACY.md)
- [Assistance](SUPPORT.md)
- [Sources des bibliothèques](https://github.com/YouthSeiko/yuki-desktop-distribution/releases/tag/dependencies-6.10.2)
- [Provenance et empreintes](SOURCE-ORIGINS.json)

Les archives Qt 6.10.2, PySide/Shiboken 6.10.2, FFmpeg 7.1.2 et zlib 1.3.1 sont conservées dans la release ci-dessus. Leurs licences propres et notices sont incluses dans les archives. Ces composants ne sont pas modifiés par Yuki. Le runtime est construit sous Windows x64 avec Python 3.12.10, PySide6 6.10.2 et PyInstaller 6.19.0.

## Remplacer les bibliothèques

Le paquet MSIX est une archive ZIP. Une copie extraite permet de remplacer les DLL dynamiques et bindings ABI compatibles dans YukiDesktop2D/_internal/PySide6 et shiboken6 puis de lancer directement YukiDesktop2D.exe hors du Store. Gardez la même architecture x64 et les interfaces compatibles. Une copie modifiée n'a plus la signature du paquet Microsoft original ; aucun contrôle de signature interne de Yuki ne bloque le chargement de ces DLL. Le démarrage et la suppression de la copie extraite ne constituent pas une installation Store. Les modifications de bibliothèques LGPL et l'ingénierie inverse nécessaire à leur débogage restent autorisées.

Construisez les bibliothèques depuis leurs sources selon les instructions amont contenues dans les archives. Les conditions des bibliothèques demeurent applicables indépendamment des droits propres au personnage et à l'application Yuki.

Les documents propres à ce dépôt sont Copyright © 2026 YouthSeiko. Les licences des bibliothèques restent inchangées. Ce dépôt ne modifie pas les licences de versions de Yuki antérieurement distribuées.

## Mio Desktop 2D

Même environnement de bibliothèques dynamiques, sources et notices ci-dessus.
Les chemins de remplacement sont `MioDesktop2D/_internal/PySide6`, `shiboken6`
et `MioDesktop2D.exe`. Aucun code ni asset propre à Mio n’est publié ici.

- [Mio — confidentialité / privacy / プライバシー](mio/PRIVACY.md)
- [Mio — assistance / support / サポート](mio/SUPPORT.md)
