# Oppgave 3

## Sette opp git lokalt:
> git init

## Lage dev branch:

Koblet til GitHub repository:
> git remote add origin https://github.com/larsmra/oppgave3_leksjon3.git

Lage dev branch:
> git checkout -b dev


## Lage fil i dev branch (hiof.js fil med console.log("hiof")):
> echo "console.log(\"hiof\")" >> hiof.js

## Commite disse:
> git add hiof.js
> git commit -m "Laget hiof.js"

## Pushe endringene til repo:
git push --set-upstream origin dev

## Lage en fil i dev branch remote. Hente endringene lokalt:
Lagde en fil på GitHub.

Hentet endringene lokalt:
> git pull origin dev

## Merge filene fra dev i master:
Merge dev og master:
> git merge dev --allow-unrelated-histories

Push til GitHub:
> git push --set-upstream origin master

## Resolve merge conflict:
> git add .
> git commit -m "merge"

## Stash:
Lagde ny fil "stash-test.js":
> git touch stash-test.js
> git add .

Stashe filen:
> git stash

## Pop:
git stash pop

## Cherry-pick:
Lagde ny fil i GitHub, og commita.
Brukte cherry-pick for å hente kun den commiten:
> git cherry-pick 69410df6d6791915c50df4a520a890f4823171f6