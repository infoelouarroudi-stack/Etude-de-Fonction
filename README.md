# Étude de fonctions : Domaine de définition et Limites
*Niveau Terminale*
## 📝 Exercice diagnostic (1h max)

### Énoncé

Soit la fonction 
$f(x) = \frac{x^2 - 1}{x - 1}$

**Questions :**

1. **Domaine de définition :** Déterminer l'ensemble de définition de $f$.

2. **Simplification :** Simplifier l'expression de $f(x)$ quand c'est possible.

3. **Limites :**
   - $\lim_{x \to 1} f(x)$
   - $\lim_{x \to +\infty} f(x)$
   - $\lim_{x \to -\infty} f(x)$

4. **Dérivée :** Calculer $f'(x)$ (sur son domaine).

5. **Variation :** Étudier le signe de $f'(x)$ et dresser le tableau de variation de $f$.

---

## ✅ Correction détaillée

### 1. Domaine

Le dénominateur $x - 1$ ne doit pas être nul →

$D_f = \mathbb{R} \setminus \{1\}$

### 2. Simplification

$f(x) = \frac{x^2 - 1}{x - 1} = \frac{(x-1)(x+1)}{x-1}, \quad x \neq 1$

Donc, pour $x \neq 1$,
$f(x) = x + 1$

### 3. Limites

- Quand $x \to 1$, $f(x) = x + 1 \to 2$. 
  
  ⚠️ **Attention** : la fonction n'est **pas définie** en $x = 1$, donc la limite existe et vaut 2, mais pas $f(1)$.

- Quand $x \to +\infty$, $f(x) = x + 1 \to +\infty$

- Quand $x \to -\infty$, $f(x) = x + 1 \to -\infty$

### 4. Dérivée

Puisque $f(x) = x + 1$ (pour $x \neq 1$),

$f'(x) = 1$

### 5. Variation

Comme $f'(x) = 1 > 0$, la fonction est **strictement croissante** sur chaque intervalle de son domaine :

- $]-\infty, 1[$
- $]1, +\infty[$

**Tableau de variations :**

| $x$ | $-\infty$ |  | $1$ |  | $+\infty$ |
|-----|-----------|--|-----|--|-----------|
| $f(x)$ | $-\infty$ | $\nearrow$ | trou en $x=1$ | $\nearrow$ | $+\infty$ |

---

### 💡 Pourquoi cet exercice est idéal pour une première séance ?

- Il commence simple (domaine)
- Il oblige à réfléchir sur une simplification
- Il introduit la limite et la dérivée en douceur
- Il permet de discuter la différence entre **trou** (point non défini) et asymptote verticale

---

## 1️⃣ Domaine de définition

### Définition

Le **domaine de définition** d'une fonction $f$ est **l'ensemble des réels $x$** pour lesquels la formule de $f(x)$ a un sens.

### Règles principales (à savoir par cœur)

#### Polynômes
- **Règle** : définis sur $\mathbb{R}$
- **Exemple** : $f(x) = 2x^3 - 5x + 1$
- **Domaine** : $\mathbb{R}$

#### Fonctions rationnelles ($\frac{P(x)}{Q(x)}$)
- **Règle** : interdit là où le dénominateur s'annule
- **Exemple** : $f(x) = \frac{x+1}{x^2-1}$
- **Domaine** : $\mathbb{R}\setminus\{-1,1\}$

#### Racines carrées
- **Règle** : sous la racine, l'expression doit être $\geq 0$
- **Exemple** : $f(x) = \sqrt{x-2}$
- **Domaine** : $[2,+\infty)$

#### Logarithme népérien ($\ln(x)$)
- **Règle** : défini seulement pour $x > 0$
- **Exemple** : $f(x) = \ln(x-3)$
- **Domaine** : $(3,+\infty)$

#### Exponentielle ($e^x$)
- **Règle** : définie pour tout $x \in \mathbb{R}$
- **Domaine** : $\mathbb{R}$

#### Combinaisons
- **Règle** : appliquer les règles ensemble
- **Exemple** : $f(x) = \frac{\ln(x)}{x-2}$
- **Domaine** : $(0,+\infty)\setminus\{2\}$

---

## 2️⃣ Limites

### Définition intuitive

La **limite** décrit le comportement de $f(x)$ quand $x$ devient très grand ($+\infty$ ou $-\infty$) ou quand $x$ approche une valeur interdite.

### A. Limites en $+\infty$ ou $-\infty$

#### Polynômes
- $\lim_{x\to +\infty} x^n = +\infty$ si $n$ pair ou impair
- $\lim_{x\to -\infty} x^n = +\infty$ si $n$ pair, et $-\infty$ si $n$ impair

#### Fonctions rationnelles
Comparer les degrés du numérateur et du dénominateur :

- Si $\deg(P) < \deg(Q)$ → limite = 0
- Si $\deg(P) = \deg(Q)$ → limite = rapport des coefficients dominants
- Si $\deg(P) > \deg(Q)$ → limite infinie ($+\infty$ ou $-\infty$ selon les signes)

**Exemple** : $\frac{3x^2+1}{2x^2-5}$ → limite = $\frac{3}{2}$

#### Exponentielle
- $\lim_{x\to +\infty} e^x = +\infty$
- $\lim_{x\to -\infty} e^x = 0$

#### Logarithme
- $\lim_{x\to +\infty} \ln(x) = +\infty$
- $\lim_{x\to 0^+} \ln(x) = -\infty$

### B. Limites en un point interdit

**Exemple typique** : $\frac{1}{x}$ en 0

- Quand $x \to 0^+$, $\frac{1}{x} \to +\infty$
- Quand $x \to 0^-$, $\frac{1}{x} \to -\infty$

---

## 📋 Tableau des limites usuelles (À CONNAÎTRE ABSOLUMENT)

| Expression | Limite | Résultat |
|------------|---------|----------|
| $\frac{1}{x}$ | $x \to +\infty$ | $0$ |
| $\frac{1}{x}$ | $x \to 0^+$ | $+\infty$ |
| $\frac{1}{x}$ | $x \to 0^-$ | $-\infty$ |
| $\frac{1}{x^n}$ | $x \to +\infty$ | $0$ (pour $n > 0$) |
| $\frac{\ln(x)}{x}$ | $x \to +\infty$ | $0$ |
| $\frac{e^x}{x}$ | $x \to +\infty$ | $+\infty$ |
| $\frac{x}{e^x}$ | $x \to +\infty$ | $0$ |
| $\frac{\sin(x)}{x}$ | $x \to 0$ | $1$ |

---

## Opérations sur les limites

### Règles de base
- **Somme** : si les deux limites existent (finies), on peut additionner
- **Produit** : idem (attention aux infinis)
- **Quotient** : possible si dénominateur ≠ 0 en limite

**Exemple** :
$$\lim_{x\to +\infty} \frac{3x^2+1}{x^2-4} = \frac{3}{1} = 3$$

### Cas indéterminés ⚠️

Ces cas demandent de simplifier l'expression :

- $\infty - \infty$
- $\frac{\infty}{\infty}$
- $0 \cdot \infty$
- $\frac{0}{0}$

**Techniques** : factorisation, division par le terme dominant, développement limité.

---

## 🎯 Méthode de travail

### Étape 1 : Domaine de définition
1. Identifier les expressions interdites dans la formule
2. Résoudre les équations correspondantes
3. Exclure ces valeurs du domaine

### Étape 2 : Limites
1. Repérer les points où la fonction n'est pas définie → souvent une **limite infinie** (asymptote verticale)
2. Étudier le comportement en **±∞** → asymptote horizontale ou oblique
3. Utiliser les **limites usuelles** du tableau
4. Appliquer les règles d'opérations

---

## ✅ Points clés à retenir

- Toujours commencer par vérifier le **domaine**
- Connaître par cœur les **limites usuelles**
- Savoir reconnaître et traiter les **cas indéterminés**
- Les limites donnent des informations sur les **asymptotes**

---

## 3️⃣ Dérivée

### Définition

La **dérivée** d'une fonction en un point mesure la **pente de la tangente** en ce point.

$f'(a) = \lim_{h \to 0} \frac{f(a+h) - f(a)}{h}$

### Règles de dérivation usuelles

#### Règles de base
- $(k)' = 0$ (constante)
- $(x^n)' = nx^{n-1}$ (puissance)
- $(u + v)' = u' + v'$ (somme)
- $(uv)' = u'v + uv'$ (produit)
- $\left(\frac{u}{v}\right)' = \frac{u'v - uv'}{v^2}$ (quotient)

#### Dérivée composée
Si $f(x) = u(v(x))$, alors $f'(x) = u'(v(x)) \times v'(x)$

### 📋 Tableau des dérivées des fonctions de base

| Fonction $f(x)$ | Dérivée $f'(x)$ | Domaine de dérivabilité |
|-----------------|-----------------|-------------------------|
| $k$ (constante) | $0$ | $\mathbb{R}$ |
| $x^n$ | $nx^{n-1}$ | $\mathbb{R}$ (si $n \geq 1$) |
| $\frac{1}{x}$ | $-\frac{1}{x^2}$ | $\mathbb{R}^*$ |
| $\sqrt{x}$ | $\frac{1}{2\sqrt{x}}$ | $(0,+\infty)$ |
| $e^x$ | $e^x$ | $\mathbb{R}$ |
| $\ln(x)$ | $\frac{1}{x}$ | $(0,+\infty)$ |
| $\sin(x)$ | $\cos(x)$ | $\mathbb{R}$ |
| $\cos(x)$ | $-\sin(x)$ | $\mathbb{R}$ |

### Exemples de calculs

#### Exemple 1 : Fonction polynomiale
$f(x) = 3x^4 - 2x^2 + 5x - 1$

$f'(x) = 12x^3 - 4x + 5$

#### Exemple 2 : Fonction rationnelle
$f(x) = \frac{x^2 + 1}{x - 2}$

En utilisant la règle du quotient :
$f'(x) = \frac{(2x)(x-2) - (x^2+1)(1)}{(x-2)^2} = \frac{x^2 - 4x - 1}{(x-2)^2}$

#### Exemple 3 : Fonction composée
$f(x) = e^{x^2}$

$f'(x) = e^{x^2} \times 2x = 2xe^{x^2}$

### Applications de la dérivée

#### A. Tableau de variations
Le **signe de $f'(x)$** détermine la croissance/décroissance :

- Si $f'(x) > 0$ sur un intervalle → $f$ est **croissante**
- Si $f'(x) < 0$ sur un intervalle → $f$ est **décroissante**
- Si $f'(x) = 0$ en un point → point critique (extremum possible)

#### B. Équation de la tangente
La tangente à la courbe de $f$ au point d'abscisse $x = a$ a pour équation :

$y = f'(a)(x-a) + f(a)$

**Exemple** : Tangente à $f(x) = x^2$ en $x = 2$
- $f(2) = 4$ et $f'(2) = 4$
- Équation de la tangente : $y = 4(x-2) + 4 = 4x - 4$

#### C. Extremums locaux
- Si $f'(a) = 0$ et $f'$ change de signe en $a$ → $a$ est un extremum local
- Si $f'$ passe du positif au négatif → maximum local
- Si $f'$ passe du négatif au positif → minimum local

### 🎯 Méthode pour étudier les variations

#### Étape 1 : Calculer $f'(x)$
Utiliser les règles de dérivation

#### Étape 2 : Déterminer le domaine de $f'$
Généralement le même que celui de $f$

#### Étape 3 : Résoudre $f'(x) = 0$
Trouver les points critiques

#### Étape 4 : Étudier le signe de $f'(x)$
Tableau de signes

#### Étape 5 : Dresser le tableau de variations
Avec les intervalles de croissance/décroissance et les extremums

---

## ✅ Points clés à retenir

- Toujours commencer par vérifier le **domaine**
- Connaître par cœur les **limites usuelles** et les **dérivées de base**
- Savoir reconnaître et traiter les **cas indéterminés**
- Les limites donnent des informations sur les **asymptotes**
- La dérivée permet de déterminer les **variations** et l'équation de la **tangente**

---

*Ce cours couvre les trois premières étapes essentielles de l'étude de fonction en Terminale.*


-----------------------------------------------
Parfait 👌 Je vais t’aider à préparer ce contrôle d’anglais.

### 1. Utiliser le prétérit (past simple)

* **Affirmative** :
  Sujet + verbe au prétérit (verbe régulier = +ED / verbe irrégulier = forme spéciale).
  Exemple :

* I played football yesterday.

* She went to school last Monday.

* **Négative** :
  Sujet + **did not (didn’t)** + verbe à la **base verbale**.
  Exemple :

* I did not (didn’t) play football yesterday.

* She didn’t go to school last Monday.

---

### 2. Verbes irréguliers (catégories 1 et 2 + ceux vus en cours)

* **Catégorie 1 : les verbes qui changent totalement**
  ex : go → went, see → saw, eat → ate, write → wrote...

* **Catégorie 2 : les verbes qui changent partiellement**
  ex : have → had, make → made, say → said, buy → bought...

* **Réguliers : +ED**
  ex : play → played, watch → watched, study → studied...

👉 Tu dois mémoriser les verbes irréguliers vus dans ta séquence (par exemple : be → was/were, do → did, get → got...).

---

### 3. HOW TO – Introduce a person

Quand on présente quelqu’un en anglais :

* **Simple** :
  This is my friend Sarah.
  He is my brother.
  She is a student.

* **Avec détails** :
  I would like to introduce you to Mr. Brown.
  This is John, he is from London, and he is 15 years old.

---

✅ **Exercices d’entraînement rapides :**

1. Mets au prétérit (affirmative) :

* They (play) tennis last week.
* She (go) to Paris last summer.

2. Mets en négatif :

* I (see) my teacher yesterday.
* We (watch) TV last night.

3. Introduis une personne :

* Ton meilleur ami(e) : prénom, âge, ville, hobby.

---

Veux-tu que je **te crée des phrases déjà résolues** (corrigées), comme ça tu auras un modèle direct pour ton contrôle ?



------------------------------------------------------


D’accord 👍 je vais t’expliquer.

En **France**, le programme de **Mathématiques en classe de 3ᵉ (collège, dernier niveau avant le lycée)** contient plusieurs grands chapitres :

### 📘 Programme officiel de Maths en 3ᵉ

1. **Nombres et calculs**

   * Nombres relatifs, fractions, puissances.
   * Calcul littéral (formules, développement, factorisation).
   * Équations du 1ᵉʳ degré.

2. **Fonctions**

   * Proportionnalité.
   * Fonctions linéaires et affines (droite, coefficient directeur, ordonnée à l’origine).

3. **Géométrie**

   * Théorème de Pythagore.
   * Théorème de Thalès et réciproques.
   * Trigonométrie (sinus, cosinus, tangente).
   * Notions sur les volumes et sections de solides.

4. **Statistiques et probabilités**

   * Moyenne, médiane, étendue.
   * Diagrammes, graphiques.
   * Probabilités simples.

5. **Algorithmique et programmation**

   * Utilisation d’algorithmes simples.
   * Initiation avec Python (calculs, boucles).

---

### 📍 Premier cours en général : **Nombres et calculs → Puissances et priorités des opérations**

#### 🔹 Les puissances

* $a^n = a \times a \times a \times ...$ (n fois).
  Exemple :
* $2^3 = 2 \times 2 \times 2 = 8$.
* $10^4 = 10000$.

#### 🔹 Règles

* $a^m \times a^n = a^{m+n}$.
* $\dfrac{a^m}{a^n} = a^{m-n}$.
* $(a^m)^n = a^{m \times n}$.
* $a^0 = 1$ (si $a \neq 0$).

#### 🔹 Priorités des opérations

* D’abord les puissances,
* puis multiplications/divisions,
* puis additions/soustractions.

👉 Exemple :
$2 + 3 \times 2^3$
= $2 + 3 \times 8$
= $2 + 24 = 26$.

---

Veux-tu que je prépare pour toi **un mini-exercice corrigé** sur ce premier cours pour t’entraîner directement ?


----------------------------------------------------------------------------


Parfait 👌 je vais aussi te résumer et t’aider à réviser cette partie de **technologie**.

### Sujet : Chaîne d’énergie (Chaîne NRJ)

Une chaîne d’énergie explique **comment l’énergie circule et se transforme dans un système technique** (voiture, perceuse, robot, etc.).

#### Les 4 étapes principales :

1. **Alimenter** → Fournir l’énergie (pile, batterie, prise électrique…).
2. **Distribuer** → Acheminer l’énergie (câbles, interrupteur, carte électronique…).
3. **Convertir** → Transformer l’énergie en une autre forme utile (moteur transforme énergie électrique → énergie mécanique).
4. **Transmettre** → Faire passer l’énergie jusqu’à l’organe de sortie (roues, engrenages, courroies…).

---

### Notions d’énergie importantes

* **Énergie électrique** : utilisée dans beaucoup d’appareils.
* **Énergie mécanique** : mouvement (rotation, translation).
* **Énergie thermique** : chaleur (exemple moteur thermique).
* **Énergie chimique** : contenue dans le carburant ou la pile.

👉 Exemple : perceuse électrique

* Alimenter : prise de courant.
* Distribuer : interrupteur.
* Convertir : moteur électrique.
* Transmettre : engrenages + mandrin (qui fait tourner le foret).

---

### Diagramme SysML (simplifié)

C’est un schéma pour représenter le fonctionnement d’un système :

* **Bloc d’entrée** (l’utilisateur) → donne une consigne.
* **Chaîne d’énergie** → fait fonctionner la machine.
* **Bloc de sortie** → résultat (ex : trou percé).

---

### Exercices typiques

1. **Question** : Quelle est la fonction du moteur dans une chaîne d’énergie ?
   👉 Réponse : convertir l’énergie électrique en énergie mécanique.

2. **Question** : Donne les 4 fonctions principales d’une chaîne d’énergie.
   👉 Réponse : alimenter, distribuer, convertir, transmettre.

3. **Question** : Dans un vélo, quelle est la partie qui transmet l’énergie ?
   👉 Réponse : la chaîne, les pédales, les roues dentées.

---

✅ **À réviser pour ton interrogation** :

* Les définitions des 4 blocs (alimenter, distribuer, convertir, transmettre).
* Les différents types d’énergie (électrique, mécanique, chimique, thermique).
* Savoir faire un schéma simple d’une chaîne d’énergie.
* Revoir les exercices faits en classe.

---

Veux-tu que je te prépare **une fiche ultra-courte (recto-verso) de révision** que tu pourras relire vite avant le contrôle ?


-----------------------------

Super 👍 tu veux du niveau plus difficile !
Voici des exercices **avancés sur les puissances et priorités**, comme tu pourrais rencontrer en 3ᵉ voire début lycée.

---

### 🔹 Exercice 1 : Simplifications complexes

1. $\dfrac{3^5 \times 3^2}{3^4}$
2. $\dfrac{2^7}{2^3 \times 2^2}$
3. $(5^2 \times 5^3)^2 \div 5^4$
4. $\dfrac{10^6}{(10^2)^2}$

✅ **Correction**

1. $3^{5+2-4} = 3^3 = 27$
2. $2^{7-(3+2)} = 2^2 = 4$
3. $5^{(2+3)\times 2 - 4} = 5^{10 - 4} = 5^6 = 15625$
4. $10^{6 - (2\times 2)} = 10^{6-4} = 10^2 = 100$

---

### 🔹 Exercice 2 : Priorités avec parenthèses

1. $(2^3 + 3^2) \times 2$
2. $(5^2 - 4^2) \div 3$
3. $(10 - 2 \times 3)^2$
4. $(2^4 + 2^3) \div (2^2)$

✅ **Correction**

1. $(8 + 9)\times 2 = 17 \times 2 = 34$
2. $(25 - 16)\div 3 = 9 \div 3 = 3$
3. $(10 - 6)^2 = 4^2 = 16$
4. $(16 + 8) \div 4 = 24 \div 4 = 6$

---

### 🔹 Exercice 3 : Mélange puissances et fractions

1. $\dfrac{2^5}{2^3} + 2^2$
2. $\dfrac{3^4 - 3^2}{3^2}$
3. $\dfrac{5^3}{5^2} \times (2^3 + 2)$
4. $\dfrac{(4^3 \times 2^2)}{4^2}$

✅ **Correction**

1. $2^{5-3} + 4 = 2^2 + 4 = 4 + 4 = 8$
2. $\dfrac{81 - 9}{9} = \dfrac{72}{9} = 8$
3. $5^{3-2} \times (8+2) = 5 \times 10 = 50$
4. $\dfrac{64 \times 4}{16} = \dfrac{256}{16} = 16$

---

### 🔹 Exercice 4 : Problème (appliqué)

Un carré a un côté de longueur $2^3$ cm.

1. Calcule son périmètre.
2. Calcule son aire.
3. Vérifie que l’aire est bien égale à $(côté)^2$.

✅ **Correction**

1. Côté = $2^3 = 8$ cm → Périmètre = $4 \times 8 = 32$ cm.
2. Aire = $8^2 = 64$ cm².
3. Vérif : $(2^3)^2 = 2^{3\times 2} = 2^6 = 64$. ✅

---

👉 Veux-tu que je monte encore plus le niveau avec des **équations contenant des puissances** (par exemple résoudre $2^x = 8$) ?



