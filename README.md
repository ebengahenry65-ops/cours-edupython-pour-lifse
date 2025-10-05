# cours-edupython-pour-lifse
<!doctype html>
<html lang="fr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>EduPythonFacile — Cours complets Python NSI Première</title>
  <meta name="description" content="Cours, exercices et explications complètes pour la spécialité NSI Première sur EduPython." />
  <style==
  </style>
</head>
<body>
<header>
  <div class="container">
    <nav>
      <div class="logo"><div class="mark">Py</div><div>EduPythonFacile</div></div>
      <div><a href="#cours">Cours</a> <a href="#commandes">Commandes</a> <a href="#exercices">Exercices</a> <a class="btn" href="#commencer">Commencer</a></div>
    </nav>
  </div>
</header>

<main class="container">
  <h1 id="commencer">Programme NSI — Première Spécialité</h1>
  <p>Ce site regroupe tous les cours nécessaires pour maîtriser Python avec EduPython, incluant des explications détaillées des commandes, exemples concrets, et exercices progressifs.</p>

  <section id="cours">
    <h2 class="section-title">Cours détaillés — NSI Première</h2>

    <div class="card">
      <h3>1. Introduction à Python et EduPython</h3>
      <p>Python est un langage interprété, lisible et utilisé en NSI pour développer des algorithmes, manipuler des données et créer des programmes.</p>
      <ul>
        <li><strong>print()</strong> — affiche un message à l’écran</li>
        <li><strong>input()</strong> — lit une entrée clavier</li>
        <li><strong>type()</strong> — donne le type d’une donnée</li>
      </ul>
      <pre><code>nom = input("Quel est ton nom ? ")
print("Bonjour", nom)
print(type(nom))</code></pre>
      <p><em>Astuce :</em> Dans EduPython, le terminal d’exécution se trouve en bas. Vous pouvez y interagir avec votre code.</p>
    </div>

    <div class="card">
      <h3>2. Variables et types de données</h3>
      <p>Une variable stocke une valeur. Python reconnaît plusieurs types : <code>int</code> (entier), <code>float</code> (réel), <code>str</code> (chaîne de caractères), <code>bool</code> (booléen).</p>
      <pre><code>x = 10        # entier
pi = 3.14     # réel
nom = "Léo"   # chaîne
actif = True  # booléen

print(type(pi))</code></pre>
      <details>
        <summary>Exercice</summary>
        <p>Créer un programme qui calcule l’aire d’un cercle à partir du rayon donné par l’utilisateur.</p>
      </details>
    </div>

    <div class="card">
      <h3>3. Opérations et priorités</h3>
      <p>Python suit les priorités classiques des mathématiques : parenthèses, puissances, multiplication/division, addition/soustraction.</p>
      <pre><code>a = 3 + 4 * 2       # 11
b = (3 + 4) * 2     # 14
c = 2 ** 3          # 8
print(a, b, c)</code></pre>
    </div>

    <div class="card">
      <h3>4. Conditions et booléens</h3>
      <p>Les conditions permettent de prendre des décisions. Les opérateurs de comparaison sont : <code>==</code>, <code>!=</code>, <code><</code>, <code>></code>, <code><=</code>, <code>>=</code>.</p>
      <pre><code>age = int(input('Âge : '))
if age >= 18:
    print('Majeur')
else:
    print('Mineur')</code></pre>
      <p>Combiner plusieurs conditions avec <code>and</code>, <code>or</code>, <code>not</code>.</p>
    </div>

    <div class="card">
      <h3>5. Boucles et répétitions</h3>
      <p>Deux types de boucles : <strong>for</strong> (itérative) et <strong>while</strong> (tant que).</p>
      <pre><code># Afficher les carrés de 1 à 10
for i in range(1, 11):
    print(i, i**2)

# Boucle while
compteur = 0
while compteur < 5:
    print('Compteur =', compteur)
    compteur += 1</code></pre>
      <p><strong>range(n)</strong> génère une suite d’entiers de 0 à n-1. Vous pouvez préciser un début et un pas : <code>range(debut, fin, pas)</code>.</p>
    </div>

    <div class="card">
      <h3>6. Fonctions et paramètres</h3>
      <p>Une fonction regroupe du code réutilisable. On la définit avec <code>def</code>.</p>
      <pre><code>def somme(a, b):
    return a + b

print(somme(3, 4))</code></pre>
      <p><strong>return</strong> permet de renvoyer une valeur. Sans return, la fonction ne retourne rien.</p>
    </div>

    <div class="card">
      <h3>7. Listes et dictionnaires</h3>
      <p>Les listes stockent des collections de valeurs modifiables. Les dictionnaires associent des clés à des valeurs.</p>
      <pre><code>notes = [12, 14, 16]
notes.append(18)
print(notes)

infos = {"nom": "Ana", "note": 17}
print(infos["nom"])</code></pre>
    </div>

    <div class="card">
      <h3>8. Fichiers et lecture/écriture</h3>
      <p>Lire et écrire des fichiers avec <code>open()</code> :</p>
      <pre><code>with open('exemple.txt', 'w') as f:
    f.write('Bonjour monde')

with open('exemple.txt', 'r') as f:
    print(f.read())</code></pre>
    </div>

    <div class="card">
      <h3>9. POO (Programmation Orientée Objet)</h3>
      <pre><code>class Rectangle:
    def __init__(self, largeur, hauteur):
        self.largeur = largeur
        self.hauteur = hauteur
    def aire(self):
        return self.largeur * self.hauteur

r = Rectangle(4, 5)
print(r.aire())</code></pre>
    </div>
  </section>

  <section id="commandes">
    <h2 class="section-title">Commandes Python essentielles</h2>
    <div class="card">
      <ul>
        <li><code>print(objet)</code> : affiche du texte ou une variable</li>
        <li><code>input()</code> : récupère une saisie clavier</li>
        <li><code>len(liste)</code> : renvoie la taille d’une liste</li>
        <li><code>type(objet)</code> : indique le type d’une donnée</li>
        <li><code>int(), float(), str()</code> : conversions de type</li>
        <li><code>range(n)</code> : génère une suite d’entiers</li>
        <li><code>for</code>, <code>while</code> : boucles de répétition</li>
        <li><code>if/elif/else</code> : conditions</li>
        <li><code>def</code> : création d’une fonction</li>
        <li><code>import</code> : importer un module externe</li>
        <li><code>class</code> : définir une classe pour la POO</li>
      </ul>
    </div>
  </section>

  <section id="exercices">
    <h2 class="section-title">Exercices et explications</h2>
    <div class="card">
      <p>Chaque notion ci-dessus est accompagnée d’exemples et d’exercices. Les solutions sont commentées pour comprendre chaque étape.</p>
      <ul>
        <li>Exercices sur les boucles et les conditions</li>
        <li>Problèmes de manipulation de listes et dictionnaires</li>
        <li>Création de fonctions et mini-projets (calculatrice, jeux, fichiers)</li>
      </ul>
    </div>
  </section>
</main>
</body>
</html>
