# Étude de fonctions : Domaine de définition et Limites
*Niveau Terminale*

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
