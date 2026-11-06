# Leçons de Taaspi copte

Contenu téléchargé par l'app **Taaspi copte** pour mettre à jour ses leçons sans nouvelle APK.

- `content_manifest.json` : version (croissante), schéma et empreinte sha256 de chaque fichier.
- `letters.json`, `grammar_B.json`, `grammar_S.json`, `course_B.json`, `course_S.json`,
  `liturgy_B.json` : les leçons.

**Ne pas modifier ce dépôt à la main.** Il est alimenté depuis le dépôt de l'app par
`python tools/publish_content.py publish`, qui régénère le manifeste et pousse ici.
L'app vérifie chaque fichier (empreinte, lecture complète) avant de l'utiliser, et ignore un
contenu dont le schéma est plus récent que ce qu'elle comprend.

## Licences

- Cursus (`course_*.json`) : CC BY-SA 4.0, dérivé du *Comprehensive Coptic Lexicon* v1.2 (BBAW,
  KELLIA ; DOI 10.17169/refubium-27566) et des corpus de Coptic SCRIPTORIUM (licence par corpus,
  indiquée dans le champ `corpora`).
- Textes bibliques coptes : domaine public ; traductions Giguet, Crampon, Darby, World English
  Bible : domaine public.
- Textes liturgiques (`liturgy_B.json`) : textes traditionnels (domaine public), traductions du
  projet ; **à relire**.
- Alphabet et grammaire : d'après A. Mallon, *Grammaire copte*, et les sources citées dans chaque
  leçon.
