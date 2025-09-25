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

*Ce cours couvre les deux premières étapes essentielles de l'étude de fonction en Terminale.*
