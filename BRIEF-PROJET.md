# L'Odyssée de l'environnement — briefing du site

Fichier de contexte à lire avant toute modification du site.

## Structure

```
index.html     site complet — HTML, CSS et JS dans un seul fichier
images/        22 photos JPEG optimisées (issues du magazine officiel 2026)
```

Aucune dépendance, aucun build. Ressource externe unique : Google Fonts
(Fraunces pour les titres, Inter pour le texte). Site statique : il suffit
de déposer `index.html` et `images/` sur n'importe quel hébergeur.

## Qui est qui — à ne jamais confondre

| Nom | Ce que c'est |
|---|---|
| **L'Odyssée de l'environnement** | L'ASBL de droit belge. C'est elle le sujet de ce site. |
| **L'Odyssée Express** | Le nom de l'initiative fondatrice, antérieure à l'ASBL. Figure sur les certificats, les conventions et le nom de domaine. |
| **Yaoundé Propreté / Odyssée Smart City** | Projet d'une future société commerciale au Cameroun. **Ne doit pas apparaître sur ce site.** |

## Règles éditoriales non négociables

1. **L'ASBL ne s'attribue pas les réalisations antérieures à sa constitution.**
   Tout ce qui date d'avant 2026 a été mené par le fondateur à titre personnel ;
   l'édition de juillet 2026 l'a été sous le nom L'Odyssée Express. La section
   « Antériorité » et son encadré « Précision de méthode » disent exactement cela.
   Ne pas reformuler en « nous avons organisé » pour ce qui précède l'ASBL.

2. **Pas de plateforme, pas d'application, pas de produit.** L'ASBL organise,
   forme, accompagne et sensibilise. Ses trois domaines sont : mobilisation
   citoyenne, Green Hackathon, incubation des lauréats. Rien d'autre.

3. **Aucun chiffre inventé.** Pas de montant de cotisation, pas d'IBAN, pas de
   nombre de bénéficiaires, pas de budget, pas d'objectif de collecte tant que
   la donnée réelle n'est pas fournie. Les seuls chiffres autorisés sont ceux
   déjà présents : 9 équipes, 10 h de sprint, 4 partenaires, 3 conventions.

4. **Pas de contenu politique.** Le haut patronage scientifique du MINRESI est
   mentionné ; les références à la politique nationale camerounaise ont été
   volontairement écartées. Ne pas les réintroduire.

5. **Pas d'activité d'enseignement ou de soutien scolaire**, sous aucune forme.

## Repères de design

```
--forest      #0F3D2A   vert profond, structure
--forest-deep #071A13   fonds sombres, pied de page
--leaf        #1F9D55   vert d'action, boutons, libellés
--lime        #A8D64B   vert clair, accents sur fond sombre
--lime-soft   #E8F3D6   aplats clairs
--ochre       #E8871E   accent chaud : appels à l'action, lauréats
--ochre-soft  #FCEBD5   fond de la section « Nous soutenir »
--cream       #F4F8EF   fond de page
```

Titres : Fraunces 600. Texte : Inter 400/500/600.
Rayon des coins : 20 px pour les cartes, 999 px pour les boutons.
Alternance des fonds : `.b-cream`, `.b-white`, `.b-forest`, `.b-ochre` —
ne jamais placer deux bandes identiques côte à côte.

## Exigences techniques à préserver

- Responsive jusqu'à 380 px de large
- `prefers-reduced-motion` respecté (bloc `@media` en fin de CSS)
- Focus clavier visible sur tous les liens et boutons
- `loading="lazy"` sur toutes les images sauf celle du hero
- Attributs `alt` descriptifs — ils décrivent des photos réelles, ne pas les vider
- Ancres de navigation : `#association #domaines #edition #laureats #projet #anteriorite #partenaires #soutenir #contact`

## À compléter dès que les données existent

- [ ] Numéro d'entreprise BCE (actuellement « en cours d'attribution », en pied de page)
- [ ] Date exacte de constitution de l'ASBL (actuellement « 2026 » dans la frise)
- [ ] Montant de la cotisation de membre
- [ ] Numéro de compte bancaire de l'ASBL, pour rendre le soutien opérant
- [ ] Nom de domaine définitif — le site est encore rattaché à `odyssee-express.org`
- [ ] Accord des personnes reconnaissables sur les photos, pour publication web

## Pistes d'évolution

- Page dédiée au Green Hackathon Yaoundé #2 avec formulaire d'inscription
- Galerie complète de l'édition 2026 (27 photos disponibles dans le magazine)
- Version bilingue français / anglais
- Page « Actualités » pour le suivi des trois équipes incubées
- Mentions légales et politique de confidentialité (obligatoires en Belgique)
