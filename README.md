# 📚 LA THÉORIE ULTIME DES NOMBRES : De ℕ à ℂ et au-delà

> **Auteur** : `HACKERS_TCHAD`  
> **Version** : 1.0.0 — Édition Approfondie  
> **Langue** : Français  
> **Licence** : MIT / Éducation Libre  
> **Objectif** : Comprendre en profondeur les ensembles de nombres, leurs définitions, leurs architectures, leurs créateurs, leurs applications et maîtriser leur utilisation grâce à des centaines d'exemples et d'exercices.

---

## 📖 Table des matières

1. [Introduction générale](#introduction-générale)
2. [Histoire et pionniers des nombres](#histoire-et-pionniers-des-nombres)
3. [Architecture des ensembles numériques](#architecture-des-ensembles-numériques)
4. [Les nombres naturels — ℕ](#les-nombres-naturels--n)
5. [Les nombres entiers relatifs — ℤ](#les-nombres-entiers-relatifs--z)
6. [Les nombres rationnels — ℚ](#les-nombres-rationnels--q)
7. [Les nombres réels — ℝ](#les-nombres-réels--r)
8. [Les nombres complexes — ℂ](#les-nombres-complexes--c)
9. [Systèmes numériques avancés](#systèmes-numériques-avancés)
10. [Relations et hiérarchie](#relations-et-hiérarchie)
11. [Où et comment sont utilisés ces nombres ?](#où-et-comment-sont-utilisés-ces-nombres-)
12. [Exercices complets et progressifs](#exercices-complets-et-progressifs)
13. [Ressources, livres et liens](#ressources-livres-et-liens)
14. [Annexes techniques](#annexes-techniques)

---

## Introduction générale

La notion de nombre est l'une des inventions intellectuelles les plus fondamentales de l'humanité. Depuis les premiers comptages de troupeaux jusqu'aux équations les plus sophistiquées de la physique quantique, les nombres structurent notre compréhension du monde, modélisent le réel et permettent de résoudre des problèmes concrets aussi bien qu'abstraits.

Ce document propose une exploration complète, progressive et très approfondie des principaux ensembles numériques :

- Les **nombres naturels** : `ℕ = {0, 1, 2, 3, ...}`
- Les **nombres entiers relatifs** : `ℤ = {..., -3, -2, -1, 0, 1, 2, 3, ...}`
- Les **nombres rationnels** : `ℚ = {p/q | p ∈ ℤ, q ∈ ℤ*, q ≠ 0}`
- Les **nombres réels** : `ℝ`, incluant les irrationnels comme `π`, `e`, `√2`
- Les **nombres complexes** : `ℂ = {a + bi | a, b ∈ ℝ, i² = -1}`

Chaque section présente la définition formelle, une description intuitive, des exemples variés, des propriétés algébriques et analytiques, des applications concrètes, une discussion historique et technique, ainsi que de nombreux exercices corrigés ou non corrigés pour s'entraîner.

L'objectif final est de fournir une ressource de référence de plus de 1000 lignes, utilisable par les étudiants, les développeurs, les autodidactes et tous ceux qui souhaitent maîtriser la théorie des nombres dans sa globalité.

---

## Histoire et pionniers des nombres

### Les premiers comptages

Les premières traces de comptage remontent à environ **35 000 ans avant notre ère**, avec l'os d'Ishango découvert en République démocratique du Congo, présentant des encoches groupées par trois, peut-être liées à un système de comptage préhistorique.

Les civilisations mésopotamiennes, égyptiennes, chinoises, indiennes et mayas ont développé des systèmes numériques sophistiqués pour gérer le commerce, l'astronomie, la taxation et l'architecture.

### L'invention du zéro

Le **zéro** fut conceptualisé en Inde aux alentours du **Vᵉ siècle** par les mathématiciens indiens, notamment **Brahmagupta** (598–668). Avant cela, les Grecs et les Romains n'avaient pas de symbole pour représenter le néant numérique.

Le zéro est fondamental car il permet de distinguer `10` et `1`, de poser des additions et des soustractions sans ambiguïté, et de construire l'arithmétique moderne.

### Les nombres négatifs

Les nombres négatifs furent longtemps considérés comme absurdes. En Chine, vers le **Iᵉʳ siècle**, le *Jiuzhang Suanshu* utilisait déjà des baguettes rouges pour les positifs et noires pour les négatifs. En Inde, Brahmagupta énonça des règles de calcul sur les nombres négatifs.

En Europe, ce n'est qu'au **XVIᵉ siècle**, avec des mathématiciens comme **Stifel** et plus tard **Descartes**, que les nombres négatifs furent pleinement acceptés.

### Les nombres rationnels

Les fractions étaient connues des Égyptiens sous forme de fractions unitaires. Les Grecs, notamment les Pythagoriciens, découvrirent que certaines grandeurs n'étaient pas commensurables, ce qui conduisit à l'idée de nombres irrationnels.

### Les nombres irrationnels

La découverte de l'irrationalité de `√2` est attribuée à **Hipparque** ou à un pythagoricien anonyme. Cette découverte bouleversa la conception grecque selon laquelle tout nombre pouvait s'exprimer comme rapport de deux entiers.

### Les nombres complexes

Les nombres complexes émergèrent au **XVIᵉ siècle** avec la résolution des équations cubiques par **Cardan** et **Tartaglia**. **Bombelli** (1526–1572) fut le premier à manipuler systématiquement des expressions contenant des racines carrées de nombres négatifs.

Le terme "imaginaire" fut popularisé par **Descartes**, tandis que **Gauss** (1777–1855) et **Argand** donnèrent la représentation géométrique des complexes dans le plan.

### Les constructeurs de l'analyse moderne

- **Augustin-Louis Cauchy** (1789–1857) : formalisation des limites et des suites.
- **Karl Weierstrass** (1815–1897) : construction rigoureuse des réels par les suites de Cauchy.
- **Georg Cantor** (1845–1918) : théorie des ensembles, ensembles infinis, cardinaux.
- **Richard Dedekind** (1831–1916) : construction des réels par les coupures.

---

## Architecture des ensembles numériques

### Hiérarchie ensembliste

```
ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ ⊂ ℂ
```

Cette inclusion signifie que chaque nombre naturel est aussi un entier relatif, chaque entier relatif est aussi un rationnel, chaque rationnel est aussi un réel, et chaque réel est aussi un complexe.

### Vue schématique

```
                    ℂ : nombres complexes
                   / \
                  /   \
                 /     \
                ℝ       nombres complexes non réels
               / \
              /   \
             /     \
            ℚ       nombres irrationnels
           / \
          /   \
         /     \
        ℤ       nombres rationnels non entiers
       / \
      /   \
     /     \
    ℕ       nombres entiers négatifs
```

### Propriétés structurantes

| Ensemble | Opérations internes | Ordre total | Corps | Anneau |
|----------|---------------------|-------------|-------|--------|
| ℕ        | +, ×                | Oui         | Non   | Non    |
| ℤ        | +, −, ×             | Oui         | Non   | Oui    |
| ℚ        | +, −, ×, ÷ (≠0)     | Oui         | Oui   | Oui    |
| ℝ        | +, −, ×, ÷ (≠0)     | Oui         | Oui   | Oui    |
| ℂ        | +, −, ×, ÷ (≠0)     | Non         | Oui   | Oui    |

### Construction axiomatique

- **ℕ** est construit à partir des axiomes de **Peano**.
- **ℤ** est construit comme complétion de ℕ pour la soustraction.
- **ℚ** est construit comme corps des fractions de ℤ.
- **ℝ** est construit par complétion métrique de ℚ ou par coupures de Dedekind.
- **ℂ** est construit comme extension algébrique de ℝ par adjonction de `i` tel que `i² = -1`.

---

## Les nombres naturels — ℕ

### Définition formelle

L'ensemble des **nombres naturels**, noté `ℕ`, est l'ensemble des entiers positifs ou nuls utilisés pour compter :

```
ℕ = {0, 1, 2, 3, 4, 5, 6, ...}
```

Certains auteurs notent `ℕ*` ou `ℕ⁺` pour l'ensemble des naturels strictement positifs :

```
ℕ* = {1, 2, 3, 4, 5, ...}
```

### Axiomes de Peano

Giuseppe Peano (1858–1932) a formalisé l'arithmétique naturelle par cinq axiomes :

1. **Zéro est un naturel** : `0 ∈ ℕ`.
2. **Tout naturel a un successeur** : si `n ∈ ℕ`, alors `S(n) ∈ ℕ`.
3. **Zéro n'est le successeur d'aucun naturel** : il n'existe pas `n ∈ ℕ` tel que `S(n) = 0`.
4. **Les successeurs distincts proviennent d'antécédents distincts** : si `S(n) = S(m)`, alors `n = m`.
5. **Principe de récurrence** : si une propriété est vraie pour `0` et si sa vérité pour `n` entraîne sa vérité pour `S(n)`, alors elle est vraie pour tout `n ∈ ℕ`.

### Description intuitive

Les nombres naturels sont les nombres du comptage. Ils servent à répondre à la question "combien ?". On les utilise pour dénombrer des objets, itérer des processus, indexer des suites et structurer le raisonnement par récurrence.

### Exemples

- `0` : le nombre de pommes dans un panier vide.
- `3` : le nombre de côtés d'un triangle.
- `7` : le nombre de jours dans une semaine.
- `1000` : le nombre de mètres dans un kilomètre.

### Propriétés algébriques

- **Addition** : commutative, associative, élément neutre `0`.
- **Multiplication** : commutative, associative, élément neutre `1`.
- **Distributivité** : `a × (b + c) = a×b + a×c`.
- **Ordre** : relation d'ordre total `≤` compatible avec `+` et `×`.

### Limitations

Dans ℕ, la soustraction `a − b` n'est définie que si `a ≥ b`. Ainsi, `5 − 3 = 2` est valide, mais `3 − 5` n'est pas un naturel. Cette limitation motive l'extension vers ℤ.

### Arithmétique modulaire

Sur ℕ, on peut définir la division euclidienne :

```
Pour tout a ∈ ℕ et b ∈ ℕ*, il existe un unique couple (q, r) tel que :
a = bq + r, avec 0 ≤ r < b
```

Exemple : `17 = 5 × 3 + 2`, donc `q = 3` et `r = 2`.

### Nombres premiers

Un naturel `p > 1` est **premier** s'il n'est divisible que par `1` et lui-même.

Exemples : `2, 3, 5, 7, 11, 13, 17, 19, 23, 29`.

Le **théorème fondamental de l'arithmétique** affirme que tout naturel supérieur ou égal à `2` se décompose de manière unique en produit de facteurs premiers.

Exemple : `60 = 2² × 3 × 5`.

### Où utilise-t-on les nombres naturels ?

- Informatique : indices de tableaux, boucles `for`, compteurs.
- Biologie : dénombrement de populations.
- Commerce : quantités de produits.
- Logique : preuves par récurrence.
- Cryptographie : arithmétique modulaire, nombres premiers.

---

## Les nombres entiers relatifs — ℤ

### Définition formelle

L'ensemble des **nombres entiers relatifs**, noté `ℤ`, est l'ensemble des entiers positifs, nuls et négatifs :

```
ℤ = {..., -3, -2, -1, 0, 1, 2, 3, ...}
```

### Description intuitive

Les entiers relatifs permettent de modéliser des situations où deux directions ou deux sens opposés coexistent : crédit/débit, température au-dessus/en-dessous de zéro, gain/perte, altitude/profondeur.

### Construction à partir de ℕ

On construit ℤ en introduisant pour chaque naturel `n` un opposé `−n`, de sorte que :

```
n + (−n) = 0
```

Formellement, ℤ est le quotient de `ℕ × ℕ` par la relation d'équivalence :

```
(a, b) ~ (c, d) ⇔ a + d = b + c
```

L'entier `a − b` est alors la classe du couple `(a, b)`.

### Exemples

- `−5` : une température de 5 degrés sous zéro.
- `+12` : un gain de 12 points.
- `−100` : un débit de 100 euros.
- `0` : le point de référence neutre.

### Propriétés algébriques

- **Anneau commutatif** : `(ℤ, +, ×)` est un anneau.
- **Addition** : commutative, associative, neutre `0`, opposé `−a`.
- **Multiplication** : commutative, associative, neutre `1`.
- **Distributivité** : `a × (b + c) = a×b + a×c`.
- **Ordre** : ordre total compatible avec l'addition.

### Règles des signes

```
(+a) × (+b) = +ab
(+a) × (−b) = −ab
(−a) × (+b) = −ab
(−a) × (−b) = +ab
```

Ces règles garantissent la cohérence de l'anneau ℤ et de ses extensions.

### Division euclidienne dans ℤ

```
Pour tout a ∈ ℤ et b ∈ ℤ*, il existe un unique couple (q, r) ∈ ℤ² tel que :
a = bq + r, avec 0 ≤ r < |b|
```

Exemple : `−17 = 5 × (−4) + 3`, donc `q = −4` et `r = 3`.

### PGCD et PPCM

- **PGCD** : Plus Grand Commun Diviseur de deux entiers.
- **PPCM** : Plus Petit Commun Multiple.

Exemple : `PGCD(48, 18) = 6` et `PPCM(48, 18) = 144`.

L'algorithme d'**Euclide** permet de calculer efficacement le PGCD :

```
PGCD(a, b) = PGCD(b, a mod b)
```

### Où utilise-t-on les entiers relatifs ?

- Finance : soldes bancaires, dettes, crédits.
- Physique : charges électriques, directions sur un axe.
- Informatique : entiers signés, coordonnées relatives.
- Météorologie : températures négatives.
- Jeux vidéo : scores, vies, positions sur une carte.

---

## Les nombres rationnels — ℚ

### Définition formelle

L'ensemble des **nombres rationnels**, noté `ℚ`, est l'ensemble des fractions d'entiers :

```
ℚ = { p/q | p ∈ ℤ, q ∈ ℤ*, q ≠ 0 }
```

Deux fractions `p/q` et `r/s` représentent le même rationnel si et seulement si :

```
ps = qr
```

### Description intuitive

Les rationnels modélisent les rapports, les proportions, les parts et les taux. Ils permettent de résoudre des équations de la forme `ax = b` avec `a, b ∈ ℤ` et `a ≠ 0`.

### Construction à partir de ℤ

ℚ est le **corps des fractions** de ℤ. On construit ℚ en autorisant formellement la division par tout entier non nul, à condition d'identifier les fractions équivalentes.

### Exemples

- `1/2` : la moitié d'un gâteau.
- `−3/4` : une dette de trois quarts.
- `22/7` : approximation rationnelle de π.
- `0,75 = 3/4` : un pourcentage de 75 %.

### Propriétés algébriques

- **Corps commutatif** : `(ℚ, +, ×)` est un corps.
- **Addition** : `a/b + c/d = (ad + bc)/(bd)`.
- **Multiplication** : `(a/b) × (c/d) = (ac)/(bd)`.
- **Inverse** : si `a/b ≠ 0`, alors `(a/b)⁻¹ = b/a`.
- **Ordre** : ordre total dense sans trou : entre deux rationnels distincts, il existe toujours un autre rationnel.

### Densité de ℚ

Pour tous `a, b ∈ ℚ` tels que `a < b`, il existe `c ∈ ℚ` tel que `a < c < b`. Par exemple, `c = (a + b)/2`.

### Décimales périodiques

Tout rationnel admet un développement décimal fini ou périodique.

Exemples :
- `1/2 = 0,5` (fini)
- `1/3 = 0,333...` (périodique)
- `1/7 = 0,142857142857...` (périodique de période 6)
- `5/4 = 1,25` (fini)

Réciproquement, tout développement décimal fini ou périodique représente un rationnel.

### Limitations de ℚ

ℚ n'est pas complet : certaines suites de rationnels convergent vers des limites qui ne sont pas rationnelles.

Exemple : la suite définie par `u₀ = 1` et `uₙ₊₁ = (uₙ + 2/uₙ)/2` converge vers `√2`, qui n'est pas rationnel.

### Où utilise-t-on les rationnels ?

- Cuisine : proportions d'ingrédients.
- Statistiques : probabilités, fréquences.
- Finance : taux d'intérêt, ratios.
- Informatique : nombres à virgule flottante (approximations).
- Physique : échelles, rapports de grandeur.

---

## Les nombres réels — ℝ

### Définition formelle

L'ensemble des **nombres réels**, noté `ℝ`, est la complétion de ℚ. Il contient tous les rationnels ainsi que les **nombres irrationnels**, c'est-à-dire les nombres qui ne peuvent pas s'écrire comme fraction d'entiers.

### Description intuitive

Les réels représentent toutes les grandeurs continues : longueurs, durées, températures, positions. La droite numérique réelle est un modèle géométrique où chaque point correspond à un unique réel.

### Construction de ℝ

Il existe plusieurs constructions équivalentes :

1. **Coupures de Dedekind** : un réel est une partition de ℚ en deux ensembles `A` et `B` tels que tout élément de `A` est inférieur à tout élément de `B`.
2. **Suites de Cauchy** : un réel est une classe d'équivalence de suites de Cauchy de rationnels.
3. **Développements décimaux infinis** : un réel est représenté par une suite infinie de chiffres après la virgule.

### Nombres rationnels vs irrationnels

- **Rationnels** : ℚ ⊂ ℝ.
- **Irrationnels** : ℝ \ ℚ.

Exemples d'irrationnels :
- `√2 ≈ 1,41421356...`
- `π ≈ 3,14159265...`
- `e ≈ 2,71828182...`
- `φ = (1 + √5)/2 ≈ 1,61803399...` (nombre d'or)

### Propriétés algébriques

- **Corps commutatif complet** : `(ℝ, +, ×)` est un corps ordonné complet.
- **Ordre total** : tout sous-ensemble non vide majoré admet une borne supérieure.
- **Densité** : entre deux réels distincts, il existe un rationnel et un irrationnel.
- **Complétude** : toute suite de Cauchy de réels converge dans ℝ.

### Théorème de la borne supérieure

Tout sous-ensemble non vide de ℝ majoré admet une borne supérieure dans ℝ. Cette propriété distingue fondamentalement ℝ de ℚ.

### Valeur absolue

```
|x| = { x   si x ≥ 0
      { −x  si x < 0
```

Propriétés :
- `|x| ≥ 0`
- `|xy| = |x||y|`
- `|x + y| ≤ |x| + |y|` (inégalité triangulaire)

### Intervalles réels

- `[a, b]` : fermé, inclut `a` et `b`.
- `]a, b[` : ouvert, exclut `a` et `b`.
- `[a, b[` ou `]a, b]` : semi-ouverts.
- `]−∞, +∞[` = ℝ.

### Puissances et logarithmes

Pour `a > 0` et `x ∈ ℝ` :
- `a^x = exp(x ln a)`
- `logₐ(x) = ln(x) / ln(a)`

### Suites et limites

Une suite `(uₙ)` de réels converge vers `L ∈ ℝ` si :

```
∀ ε > 0, ∃ N ∈ ℕ, ∀ n ≥ N, |uₙ − L| < ε
```

Exemple : `uₙ = 1/n` converge vers `0`.

### Continuité et dérivabilité

Les fonctions réelles `f : ℝ → ℝ` peuvent être continues, dérivables, intégrables. L'analyse réelle étudie ces propriétés en profondeur.

### Où utilise-t-on les réels ?

- Physique : mesures continues, équations du mouvement.
- Ingénierie : calculs numériques, simulations.
- Économie : modèles continus, croissance exponentielle.
- Informatique : représentation en virgule flottante (`float`, `double`).
- Géométrie : coordonnées, distances, angles.

---

## Les nombres complexes — ℂ

### Définition formelle

L'ensemble des **nombres complexes**, noté `ℂ`, est défini par :

```
ℂ = { a + bi | a, b ∈ ℝ }
```

où `i` est l'unité imaginaire telle que :

```
i² = −1
```

### Description intuitive

Les nombres complexes étendent les réels en permettant de résoudre des équations comme `x² + 1 = 0`, qui n'admettent pas de solution réelle. Ils possèdent une représentation géométrique naturelle dans le plan complexe.

### Représentation algébrique

Un complexe `z` s'écrit :

```
z = a + bi
```

- `a = Re(z)` est la **partie réelle**.
- `b = Im(z)` est la **partie imaginaire**.

### Représentation géométrique

Dans le plan complexe :
- L'axe horizontal représente la partie réelle.
- L'axe vertical représente la partie imaginaire.
- Le point d'affixe `z = a + bi` a pour coordonnées `(a, b)`.

### Module et argument

- **Module** : `|z| = √(a² + b²)`
- **Argument** : `θ = arg(z)` tel que `cos θ = a/|z|` et `sin θ = b/|z|`

### Forme trigonométrique

```
z = |z| (cos θ + i sin θ)
```

### Forme exponentielle (formule d'Euler)

```
e^(iθ) = cos θ + i sin θ
```

donc :

```
z = |z| e^(iθ)
```

### Conjugué

```
z̄ = a − bi
```

Propriétés :
- `z + z'̄ = z̄ + z'̄`
- `z × z'̄ = z̄ × z'̄`
- `z × z̄ = |z|²`

### Opérations sur les complexes

**Addition** :
```
(a + bi) + (c + di) = (a + c) + (b + d)i
```

**Multiplication** :
```
(a + bi)(c + di) = (ac − bd) + (ad + bc)i
```

**Division** :
```
(a + bi)/(c + di) = [(a + bi)(c − di)] / (c² + d²)
```

### Théorème fondamental de l'algèbre

Tout polynôme non constant à coefficients complexes admet au moins une racine complexe. Par conséquent, un polynôme de degré `n` possède exactement `n` racines complexes comptées avec multiplicité.

### Racines carrées d'un nombre négatif

```
√(−a) = i√a  pour a > 0
```

Exemples :
- `√(−1) = i`
- `√(−4) = 2i`
- `√(−9) = 3i`

### Formules de Moivre

```
(cos θ + i sin θ)^n = cos(nθ) + i sin(nθ)
```

### Applications des complexes

- Électricité : impédances, circuits alternatifs.
- Mécanique quantique : amplitudes de probabilité.
- Traitement du signal : transformée de Fourier.
- Géométrie plane : rotations, homothéties.
- Fractales : ensemble de Mandelbrot, ensemble de Julia.

---

## Systèmes numériques avancés

### Nombres algébriques

Un nombre est **algébrique** s'il est racine d'un polynôme non nul à coefficients entiers.

Exemples :
- `√2` est algébrique : racine de `x² − 2 = 0`.
- `∛5` est algébrique : racine de `x³ − 5 = 0`.
- Tout rationnel est algébrique.

### Nombres transcendants

Un nombre réel ou complexe est **transcendant** s'il n'est pas algébrique.

Exemples célèbres :
- `π` (transcendant, démontré par Lindemann en 1882)
- `e` (transcendant, démontré par Hermite en 1873)

### Nombres imaginaires purs

Un complexe de la forme `bi` avec `b ∈ ℝ*` est dit **imaginaire pur**.

### Nombres quaternions — ℍ

Les **quaternions**, introduits par **William Rowan Hamilton** en 1843, étendent les complexes avec trois unités imaginaires `i`, `j`, `k` satisfaisant :

```
i² = j² = k² = ijk = −1
ij = k,  jk = i,  ki = j
ji = −k, kj = −i, ik = −j
```

Un quaternion s'écrit `q = a + bi + cj + dk` avec `a, b, c, d ∈ ℝ`. La multiplication des quaternions n'est pas commutative.

### Nombres octonions — 𝕆

Les **octonions** étendent les quaternions avec huit dimensions. Ils perdent l'associativité de la multiplication mais conservent une forme d'alternative.

### Nombres p-adiques

Les **nombres p-adiques** sont construits à partir d'une métrique différente de celle des réels, basée sur la divisibilité par un nombre premier `p`. Ils sont utilisés en théorie des nombres et en géométrie arithmétique.

### Cardinaux infinis

Georg Cantor a montré que :
- `ℕ`, `ℤ` et `ℚ` sont **dénombrables** (cardinal `ℵ₀`).
- `ℝ` est **non dénombrable** (cardinal `2^ℵ₀`, appelé cardinal du continu).
- `ℂ` a le même cardinal que `ℝ`.

### Hyperréels

Les **hyperréels** enrichissent ℝ avec des infiniment petits et des infiniment grands, utilisés en analyse non standard.

---

## Relations et hiérarchie

### Inclusions strictes

```
ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ ⊂ ℂ
```

Chaque inclusion est stricte :
- `−1 ∈ ℤ` mais `−1 ∉ ℕ`.
- `1/2 ∈ ℚ` mais `1/2 ∉ ℤ`.
- `√2 ∈ ℝ` mais `√2 ∉ ℚ`.
- `i ∈ ℂ` mais `i ∉ ℝ`.

### Tableau comparatif détaillé

| Propriété | ℕ | ℤ | ℚ | ℝ | ℂ |
|-----------|---|---|---|---|---|
| Contient 0 | Oui | Oui | Oui | Oui | Oui |
| Contient les négatifs | Non | Oui | Oui | Oui | Oui |
| Division interne | Non | Non | Oui (sauf 0) | Oui (sauf 0) | Oui (sauf 0) |
| Ordre total | Oui | Oui | Oui | Oui | Non |
| Densité | Non | Non | Oui | Oui | Non dans ℝ² |
| Complétude | Non | Non | Non | Oui | Oui (topologique) |
| Algébriquement clos | Non | Non | Non | Non | Oui |

### Passage d'un ensemble à l'autre

- **ℕ → ℤ** : ajout des opposés pour rendre la soustraction toujours possible.
- **ℤ → ℚ** : ajout des quotients pour rendre la division toujours possible (sauf par 0).
- **ℚ → ℝ** : complétion pour les limites de suites.
- **ℝ → ℂ** : adjonction de `i` pour résoudre `x² + 1 = 0`.

---

## Où et comment sont utilisés ces nombres ?

### En informatique

- **ℕ** : boucles, indices, compteurs, tailles de structures.
- **ℤ** : entiers signés, coordonnées, différences.
- **ℚ** : calculs exacts avec des fractions, applications financières.
- **ℝ** : flottants, graphismes, simulations physiques.
- **ℂ** : traitement du signal, imagerie, machine learning.

### En physique

- **ℕ** : quantification (nombre de photons, niveaux d'énergie).
- **ℤ** : charges élémentaires (en unités de `e`).
- **ℚ** : rapports de fréquences, harmoniques.
- **ℝ** : positions, temps, champs continus.
- **ℂ** : mécanique quantique, électromagnétisme.

### En économie

- **ℕ** : nombres d'individus, de biens.
- **ℤ** : variations (hausse/baisse).
- **ℚ** : ratios financiers, parts.
- **ℝ** : modèles continus, taux de croissance.
- **ℂ** : modèles avancés, transformées.

### En cryptographie

- **ℕ** : factorisation, nombres premiers.
- **ℤ** : arithmétique modulaire.
- **ℚ** : courbes elliptiques rationnelles.
- **ℝ/ℂ** : rarement utilisés directement, mais utiles en analyse de sécurité.

### En géométrie

- **ℕ** : dimensions entières, nombres de côtés.
- **ℤ** : coordonnées discrètes, réseaux.
- **ℚ** : coordonnées rationnelles.
- **ℝ** : géométrie euclidienne, coordonnées continues.
- **ℂ** : géométrie plane, transformations conformes.

---

## Exercices complets et progressifs

### Exercices sur ℕ

**Exercice 1.1** : Donner les cinq axiomes de Peano et vérifier que `S(S(0)) = 2`.

**Exercice 1.2** : Décomposer `720` en produit de facteurs premiers.

**Exercice 1.3** : Calculer `PGCD(252, 180)` par l'algorithme d'Euclide.

**Exercice 1.4** : Démontrer par récurrence que `1 + 2 + ... + n = n(n+1)/2`.

**Exercice 1.5** : Combien y a-t-il de nombres premiers entre `1` et `100` ?

### Exercices sur ℤ

**Exercice 2.1** : Effectuer les calculs suivants :
- `−5 + 12`
- `−7 − (−3)`
- `(−4) × (−6)`
- `−24 ÷ 8`

**Exercice 2.2** : Trouver `x ∈ ℤ` tel que `3x + 7 = −5`.

**Exercice 2.3** : Effectuer la division euclidienne de `−47` par `6`.

**Exercice 2.4** : Démontrer que la somme de deux entiers pairs est paire.

**Exercice 2.5** : Résoudre dans ℤ l'équation `7x ≡ 3 [mod 10]`.

### Exercices sur ℚ

**Exercice 3.1** : Simplifier les fractions suivantes :
- `24/36`
- `−45/60`
- `121/143`

**Exercice 3.2** : Calculer `1/2 + 1/3 + 1/6`.

**Exercice 3.3** : Résoudre `(2x + 1)/3 = (x − 4)/5`.

**Exercice 3.4** : Démontrer que `0,999... = 1`.

**Exercice 3.5** : Trouver un rationnel compris strictement entre `1/2` et `2/3`.

### Exercices sur ℝ

**Exercice 4.1** : Démontrer que `√2` est irrationnel.

**Exercice 4.2** : Résoudre dans ℝ l'inéquation `|2x − 5| < 3`.

**Exercice 4.3** : Déterminer la borne supérieure de l'ensemble `{1 − 1/n | n ∈ ℕ*}`.

**Exercice 4.4** : Calculer `lim (n→∞) (3n² + 2n − 1)/(n² + 5)`.

**Exercice 4.5** : Montrer que la suite `uₙ = (−1)^n` ne converge pas.

### Exercices sur ℂ

**Exercice 5.1** : Mettre sous forme algébrique `(3 + 2i)(1 − 4i)`.

**Exercice 5.2** : Calculer le module et un argument de `z = 1 + i√3`.

**Exercice 5.3** : Résoudre dans ℂ l'équation `z² + 4z + 13 = 0`.

**Exercice 5.4** : Exprimer `cos(3θ)` en fonction de `cos θ`.

**Exercice 5.5** : Représenter dans le plan complexe l'ensemble des `z` tels que `|z − 1| = 2`.

### Exercices transversaux

**Exercice 6.1** : Classer les nombres suivants dans les ensembles ℕ, ℤ, ℚ, ℝ, ℂ :
- `−7`
- `0`
- `3/4`
- `√5`
- `2 − 5i`
- `π`
- `0,123456...` (non périodique)

**Exercice 6.2** : Construire un nombre réel non rationnel à l'aide d'une suite de Cauchy de rationnels.

**Exercice 6.3** : Démontrer que `ℚ` est dense dans `ℝ`.

**Exercice 6.4** : Montrer que `ℂ` est algébriquement clos (admis ou démonstration partielle).

**Exercice 6.5** : Expliquer pourquoi `ℝ` ne peut pas être ordonné comme sous-ensemble de `ℂ`.

---

## Ressources, livres et liens

### Livres recommandés

1. **"Les Nombres"** — Georges Ifrah  
   Histoire universelle des nombres et des numérations.

2. **"Théorie des nombres"** — Adrien-Marie Legendre  
   Traité classique sur l'arithmétique et la théorie des nombres.

3. **"Introduction à la théorie des nombres"** — Gérald Tenenbaum  
   Cours moderne et accessible sur l'arithmétique.

4. **"Analysis"** — Tom M. Apostol  
   Analyse réelle et complexe, complète et rigoureuse.

5. **"Principles of Mathematical Analysis"** — Walter Rudin  
   Référence classique en analyse réelle.

6. **"Complex Analysis"** — Lars Ahlfors  
   Référence majeure sur l'analyse complexe.

7. **"What Is Mathematics?"** — Richard Courant et Herbert Robbins  
   Introduction générale aux mathématiques.

### Liens en ligne

- [Wikipédia — Nombre](https://fr.wikipedia.org/wiki/Nombre)
- [Wikipédia — Ensemble de nombres](https://fr.wikipedia.org/wiki/Ensemble_de_nombres)
- [MathWorld — Number](https://mathworld.wolfram.com/Number.html)
- [Khan Academy — Nombres complexes](https://fr.khanacademy.org/math/algebra2/x2ec2f6f830c9fb89:complex)
- [Brilliant — Number Theory](https://brilliant.org/wiki/number-theory/)
- [MIT OpenCourseWare — Mathematics](https://ocw.mit.edu/courses/mathematics/)
- [arXiv — Number Theory](https://arxiv.org/list/math.NT/recent)

### Chaînes et plateformes éducatives

- **3Blue1Brown** (YouTube) : visualisations des nombres complexes, de l'analyse, etc.
- **Numberphile** (YouTube) : culture mathématique autour des nombres.
- **Khan Academy** : cours interactifs et exercices.
- **Brilliant** : apprentissage par la pratique.

### Outils de calcul

- **Python** avec `sympy`, `numpy`, `matplotlib`.
- **WolframAlpha** : calculs symboliques et numériques.
- **GeoGebra** : géométrie et nombres complexes.
- **SageMath** : mathématiques libres et complètes.

### Communautés

- **Math StackExchange** : questions et réponses.
- **Reddit r/math** : discussions générales.
- **Discord HACKERS_TCHAD** : communauté d'apprentissage et de hacking éthique.

---

## Annexes techniques

### Annexe A : Notations

| Symbole | Signification |
|---------|---------------|
| ℕ       | Nombres naturels |
| ℤ       | Entiers relatifs |
| ℚ       | Rationnels |
| ℝ       | Réels |
| ℂ       | Complexes |
| ℍ       | Quaternions |
| 𝕆       | Octonions |
| ∀       | Pour tout |
| ∃       | Il existe |
| ∈       | Appartient à |
| ⊂       | Inclus dans |
| ⇒       | Implique |
| ⇔       | Équivalent à |

### Annexe B : Tables de vérité des opérations

**Addition dans ℤ** :
```
  + |  0   1  −1
----|------------
  0 |  0   1  −1
  1 |  1   2   0
 −1 | −1   0  −2
```

**Multiplication dans ℤ** :
```
  × |  0   1  −1
----|------------
  0 |  0   0   0
  1 |  0   1  −1
 −1 |  0  −1   1
```

### Annexe C : Code Python illustratif

```python
# Manipulation des ensembles de nombres en Python

# Naturels et entiers
n = 5
z = -7

# Rationnels sous forme de fractions
from fractions import Fraction
q = Fraction(3, 4)
print(q + Fraction(1, 2))  # 5/4

# Réels (flottants)
r = 3.141592653589793

# Complexes
c = 3 + 4j
print(abs(c))      # 5.0
print(c.conjugate())  # (3-4j)

# Vérification d'appartenance (approximative pour les réels)
import math
print(math.sqrt(2))  # 1.4142135623730951
```

### Annexe D : Frises chronologiques

**Avant J.-C.** :
- 35 000 ans : os d'Ishango.
- 3000 av. J.-C. : numération égyptienne et mésopotamienne.
- 500 av. J.-C. : Pythagore et l'irrationalité.

**Après J.-C.** :
- 598–668 : Brahmagupta et le zéro.
- 1202 : Fibonacci, *Liber Abaci*.
- 1545 : Cardan, *Ars Magna*.
- 1572 : Bombelli et les nombres complexes.
- 1858 : Peano, axiomes de l'arithmétique.
- 1872 : Dedekind, coupures.
- 1874 : Cantor, théorie des ensembles.
- 1882 : Lindemann, transcendance de π.

### Annexe E : Glossaire

- **Anneau** : structure algébrique avec deux opérations (addition et multiplication) satisfaisant certaines propriétés.
- **Corps** : anneau où tout élément non nul possède un inverse pour la multiplication.
- **Corps ordonné** : corps muni d'une relation d'ordre compatible avec les opérations.
- **Complétude** : propriété selon laquoute toute suite de Cauchy converge.
- **Densité** : propriété selon laquelle entre deux éléments distincts, il existe un autre élément de l'ensemble.
- **Dénombrable** : ensemble en bijection avec ℕ.
- **Transcendant** : nombre non algébrique.

---

## Conclusion

Les nombres constituent le langage fondamental des mathématiques et des sciences. De la simplicité des naturels utilisés pour compter à la richesse des complexes permettant de modéliser les phénomènes les plus subtils, chaque ensemble de nombres résout des limitations de son prédécesseur et ouvre de nouveaux horizons conceptuels et pratiques.

Ce document, rédigé par **HACKERS_TCHAD**, propose une vue d'ensemble aussi large que profonde. Pour aller plus loin, il est recommandé de pratiquer régulièrement les exercices, d'explorer les ressources citées et de ne jamais cesser de se demander : "À quel ensemble appartient ce nombre, et pourquoi ?"

---

## Licence

Ce document est fourni à des fins éducatives. Vous êtes libres de le partager, de le modifier et de l'adapter, sous réserve de conserver la mention de l'auteur original **HACKERS_TCHAD**.

---

**Fin du document.**

```
HACKERS_TCHAD — Éducation, Code, Mathématiques, Hacking Éthique.
```
