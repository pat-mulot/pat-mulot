![banni%C3%A8re%20github](./banniere-dev.png)
## Développeur Fullstack Confirmé
PHP/Laravel - Vue.js - SQL - CI/CD Gitlab
*Du besoin flou à l'application livrée clé en main*

*A propos :*
*Ancien Concepteur/développeur de produits industriels en bureau d'études orienté éco-conception :bulb:, ancien musicien professionnel :guitar:, développeur web fullstack depuis 5 ans en environnement d'entreprise.
L'essentiel de mon travail vit dans des codebases privées/clients, comme pour la plupart des devs pro. Mon parcours et mes réalisations professionnelles :*  
- [profil **LinkedIn**](https://www.linkedin.com/in/patrice-mulot-844a4721b/)
- [**CV**](https://pat-mulot.com/projects/cv/)

***Ici**, vous trouverez le projet de fond sur lequel je travaille aujourd'hui, ainsi que mes tout premiers projets personnels, assumés tels quels.*

# PROJET ACTUEL

## Écosystème Laravel/Vue « metadata-driven » + générateur de code
> Projet personnel de fond, ~2 ans de travail, toujours en cours. **Code privé**, le socle n'est pas stabilisé. Je le décris ici parce qu'il représente l'essentiel de mon travail de conception.

**Le problème :** quand on développe plusieurs applications métier proches, on les redéveloppe presque à l'identique, puis on les maintient séparément. Un correctif de sécurité trouvé sur l'application A ne remonte jamais jusqu'à l'application B. Ce n'est pas un coût de production, c'est un coût de maintenance qui se paie pendant des années et la génération par IA amplifie le phénomène plutôt qu'elle ne le résout : régénérer N fois un code chaque fois légèrement différent, c'est repayer la production, repayer la relecture, et produire N variantes divergentes.

**L'approche :** chaque ressource déclare sa forme une seule fois, champs, relations, contraintes, dans une classe *metadata*, et un générateur produit l'intégralité de ses fichiers source à partir d'une configuration JSON : contrôleurs, modèles, migrations, services, vues, tests, et documentation destinée autant aux humains qu'aux IA. On ne développe plus les applications, on maintient le système qui les génère : un correctif se fait à un seul endroit et se propage par régénération.

**Briques principales :**
- un micro-service d'identité (signature JWT RS256 + JWKS avec clé privée pour signer et clé publique pour vérifier, permissions à grain fin façon keycloak, 2FA).
- Un backend métier e-commerce pour use-case réel (flow de commande à checksum, traçabilité multi-niveaux, idempotence de paiement où un double-clic ou un rechargement ne crée jamais deux commandes ni deux débits)
- un package « core » partagé entre les applications
- le générateur.

*Projet démarré 1 an avant l'arrivée des assistants de code : l'objectif était déjà de réduire la duplication et la dette de maintenance. L'IA est venue accélérer la démarche du projet, pas la motiver.*

---

# PREMIERS PROJETS
*Mes premiers projets personnels, en sortie de formation. Chacun a été mené jusqu'à un état démontrable et déployé, puis je suis passé au suivant. Point de départ de mon parcours dev, publics et assumés tels quels.*  
*voir [les projets](https://github.com/pat-mulot?tab=repositories)*

## Space Pat-Vaders
> Projet réalisé "jour 1" en sortie de formation (2021), expérimentation et premier projet frontend.

*Jeu de tir façon Space Invaders dans une interface fidèle à une Gameboy, jouable au clavier, à la souris ou écran tactile, vagues d'ennemis à difficulté croissante.*

*Intérêt technique : algorithmique de trajectoires et détection de collisions en JS pur, gestion unifiée de trois modes d'entrée (clavier/souris/tactile), interface responsive pensée pour occuper tout l'écran en mobile.*

principaux langages/techno utilisés : Javascript Vanilla

- Repo git : https://github.com/pat-mulot/space-patvaders
- 🎮 Application live : https://pat-mulot.com/games/space-patvaders/
- 🎞️ Vidéo de démo : https://www.youtube.com/watch?v=3elcRETYWRM
  
***Penser a activer le bouton "ON" de la gameboy pour lancer le jeu***

|Aperçu|
|---|
|![space-patvaders-img2](./space-patvaders-img-gb-2.png)|

## CUL DE CHOUETTE
> Projet réalisé "jour 2" en sortie de formation (2021), première application web complète (frontend + backend, contenu administrable).

*Application complète autour du jeu de dés "cul de chouette" (règles communautaires du jeu évoqué dans la série Kaamelott) : accueil et articles administrables, page des règles, comptes joueurs, classement façon borne d'arcade et statistiques par joueur, et le jeu lui-même : lancers en deux temps, détection automatique des figures, mode entraînement ou adversaires scriptés.*

*Intérêt technique : première app fullstack, gestion de contenu administrable (WordPress), comptes et données persistantes (scores, statistiques) ; côté jeu, adversaires aux comportements scriptés différenciés (vitesse, prise de risque, aléa) et détection de figures/scoring complet en JS.*

principaux langages/techno utilisés : Javascript Vanilla, WordPress/PHP

- Repo git : https://github.com/pat-mulot/wpcdc
- 🎮 Jouer en ligne : https://pat-mulot.com/games/wpcdc/public/game/
- 🎞️ Vidéo de démo : https://www.youtube.com/watch?v=YL4Xv0PTakg

|Aperçu||
|---|---|
|![cdc-img1](./cdc-img-jeu-1.png)|![cdc-img2](./cdc-img-jeu-2.png)|

## DivDraw
> Dernier grand projet front avant de me consacrer à mon framework Laravel actuel, expérimentation frontend plus avancée.

*Outil de dessin façon DAO dans le navigateur : ajouter des formes, les redimensionner/pivoter/colorer, les grouper ou fusionner en SVG, grille magnétique, undo/redo, export PNG/SVG.*

*Intérêt technique : la vraie difficulté était la trigonométrie du redimensionnement sous rotation, zoom et grille magnétique combinés, et la gestion de groupes d'éléments fusionnables en une seule forme SVG.*

principaux langages/techno utilisés : Vue.js, SASS

- Repo git : https://github.com/pat-mulot/divdraw
- 🎮 Application live : https://pat-mulot.com/games/divdraw/#/en/creator
- 🎞️ Vidéo de démo : https://www.youtube.com/watch?v=54F96AuAHUM

|Aperçu||
|---|---|
|![exemple-1](./divdraw-3.JPG)|![exemple-2](./ex1.png)|

---

me contacter :
```
pat.mulot.pro@gmail.com
```  
