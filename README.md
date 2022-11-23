MeetupR Nantes
================

# 

<figure>
<img src="https://imgs.xkcd.com/comics/git_2x.png"
data-fig-alt="git_xkcd" data-fig-align="center" width="300"
alt="xkcd comics" />
<figcaption aria-hidden="true">xkcd comics</figcaption>
</figure>

# Pourquoi utiliser Git?

<div class="incremental">

- A on tous sauvé un fichier `final.R`
- … qu’on a modifié en `final_extra_analysis.R`
- … puis en `final_modif_denis.R` et `final_modif_morgane.R`
- … et on a depuis perdu la trace de la dernière sauvegarde 😐

</div>

## Pourquoi utiliser Git?

Un **système de contrôle de version** (SVC) relie et unifie les
différentes versions d’un même projet entre elles.

<figure>
<img
src="https://wac-cdn.atlassian.com/dam/jcr:389059a7-214c-46a3-bc52-7781b4730301/hero.svg?cdnVersion=638"
data-fig-alt="git_tree" data-fig-align="center" width="600"
alt="atlassian tutorial" />
<figcaption aria-hidden="true">atlassian tutorial</figcaption>
</figure>

## Pourquoi utiliser Git?

Un **système de contrôle de version** (SVC) permet de :

- 🧐 garder le fil de ses versions

- ⏳ remonter le temps

- 🤝 collaborer efficacement

- 🔭️ avoir accès à ses projets partout

# Comment utiliser git?

## Comment utiliser git?

✨ utilisable sous RStudio ✨

<figure>
<img src="git_tab_rstudio.png" data-fig-alt="git_tab"
data-fig-align="center" width="600" alt="git tab in RStudio" />
<figcaption aria-hidden="true">git tab in RStudio</figcaption>
</figure>

## Les manoeuvres

<figure>
<img src="git_cmd.png" data-fig-alt="git_cmd" data-fig-align="center"
width="600" alt="git command (adapted from C.Staud)" />
<figcaption aria-hidden="true">git command (adapted from
C.Staud)</figcaption>
</figure>

## Les manoeuvres locales

Sauvegarder les modifications en **local** :

<div class="incremental">

- `git add` (ou ☑) pour selectionner les modifications à sauver
- `git commit` pour valider la nouvelles version du projet
- 🏁 example

</div>

## Les outils

On peut explorer toutes nos modifications :

<div class="incremental">

- **précédentes** avec le `git history` ou `git log`
- **prévue/staged** avec le `git diff`
- 🏁 example

</div>

## Les manoeuvres remote

Sauvegarder les modifications en **remote** :

<div class="incremental">

- `git pull` pour récupérer les modifications existantes
- `git push` pour mettre à jour le remote avec notre local
- 🏁 example

</div>

🔭 Le repository remote est hébergé en ligne (GitHub, GitLab, Gitea), on
peut le **cloner** sur une autre machine!

# Et les branches?

## Les branches

Une **nouvelle branche** permet de :

- 🧦 créer plusieurs versions à partir d’une même base

- 🚦intégrer des corrections une fois validée/terminée

- 🤝 collaborer efficacement

- 🔭️ et on y a encore accès partout

## Le principe I

On *duplique* une base en un nouvelle branche. Les prochains `commit`
sont spécifiques à la branch active (`git show HEAD`).

<figure>
<img
src="https://wac-cdn.atlassian.com/dam/jcr:7afd8460-b7bf-4c42-b997-4f5cf24f21e8/01%2520Branch-2%2520kopiera.png?cdnVersion=638"
data-fig-alt="git branch" data-fig-align="center" width="600"
alt="atlassian tutorial" />
<figcaption aria-hidden="true">atlassian tutorial</figcaption>
</figure>

## Les manoeuvres

<div class="incremental">

- `git branch <new-branch>` pour créer une branche
- `git checkout <new-branch>` pour la définir comme active
- `git push -–set-upstream` pour ajouter la branch au remote
- 🏁 example

</div>

## Le principe II

On *intègre* les `commit` d’une branche dans une autre (`git merge`).

<figure>
<img
src="https://wac-cdn.atlassian.com/dam/jcr:c6db91c1-1343-4d45-8c93-bdba910b9506/02%20Branch-1%20kopiera.png?cdnVersion=638"
data-fig-alt="git merge" data-fig-align="center" width="600"
alt="atlassian tutorial" />
<figcaption aria-hidden="true">atlassian tutorial</figcaption>
</figure>

## Les manoeuvres

<div class="incremental">

- `git merge <my_branch>` intègre *my_branch* dans la branche active
- 💡 le `git pull` est un merge entre le remote et le local
- 😈 Un **merge conflict** peut arriver entre `commit`

</div>

## Les manoeuvres

En collaboration, on peut créer un `pull request` de notre branch sur un
repo remote pour demander à intégrer nos `commit` dans la master branch.

<figure>
<img
src="https://wac-cdn.atlassian.com/dam/jcr:d079cf8a-2bea-4d77-910e-2eac20c8050e/01%20Anatomy%20of%20a%20Pull%20Request.svg?cdnVersion=638"
data-fig-alt="pull request" data-fig-align="center" width="600"
alt="atlassian tutorial" />
<figcaption aria-hidden="true">atlassian tutorial</figcaption>
</figure>

# 

<figure>
<img src="https://imgs.xkcd.com/comics/git_commit_2x.png"
data-fig-alt="git commit" data-fig-align="center" width="400"
alt="xkcd comics" />
<figcaption aria-hidden="true">xkcd comics</figcaption>
</figure>

# Sources

**git**

profy.dev/project/github-minesweeper/

www.atlassian.com/git/tutorials

**RStudio git**

thinkr.fr/travailler-avec-git-via-rstudio-et-versionner-son-code/

**quarto**

https://quarto.org/docs/presentations/revealjs

github.com/quarto-dev/quarto-cli
