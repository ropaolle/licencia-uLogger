## Länkar

* [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* [Git reference](http://gitref.org/basic/)

## Git

#### Arbetsflöde
[1.x-dev]> *git status -s* `# Visa aktuella förändringar, -s = kortfattat`  
[1.x-dev]> *git add -A* `# Lägg till och ta bort filer samt förändringar`  
[1.x-dev]> *git commit -m 'message'* `# Commit lokalt`  
[1.x-dev]> *git tag -a alfa2 -m 'the second alfa'* `# Tagga commit`  
[1.x-dev]> *git push origin 1.x-dev* `# Push till GitHub`  

##### Merge
[1.x-dev]> *git checkout master* `# Byt till master`  
[master]> *git merge 1.x-dev* `# Merge 1.x-dev med master `  
[master]> *git push origin master* `# Push till GitHub`

## Snippets

### Highlight input

```css
td.highlight { border: 1px solid red; }
```

```php
if (number > 0) {
    $(this).closest('td').addClass('highlight');
} else {
    $(this).closest('td').removeClass('highlight');
}
```

```php
echo "<pre>" . htmlspecialchars($new_contents) . "</pre>";
```

### Jquery/Javascript

```javascript
console.dir(result);
```  

## Vanliga Git-kommandon
<<<<<<< HEAD

##### Log och status  
[master]> *git status* `# Visa aktuella förändringar`  
[master]> *gitk --all* `# Öppna grafiskt statusfönster`  
[master]> *git log --graph --all --oneline* `# List alla commits (avsluta med Q).`  

##### Branch
[master]> *git checkout 1.x-dev* `# Gå till branch`  
[master]> *git branch 1.x-dev* `# Skapa ny branch`  
[master]> *git checkout -b 1.x-dev* `# Skapa och gå till`  

##### Diff
[master]> *git diff* `# Ändringar sen senaste commit`  
[master]> *git diff snippets.md* `# Ändringar i specifik fil`  

##### Tag
[master]> *git tag* `# Lista alla taggar`  
[master]> *git tag test1* `# Lightweight - Namn på en commit`  
[master]> *git tag -a 1.x-alfa -m 'Första releasen baserad på licencia.se temat.'* `# Annotated - Fullt object med info`  
[master]> *git push --tags* `# Kopiera taggar til GitHub`  

##### Add
[master]> *git add -A* `# Stages All`  
[master]> *git add .* `#  Stages new and modified, without deleted`  
[master]> *git add -u* `# Stages modified and deleted, not new files`  
[master]> *git add -i* `# Addera interaktivt`  
[master]> *?* `# Kommentar`  
[master]> *?* `# Kommentar`  

<<<<<<< HEAD
### Merge
Merge 1.x-dev med master & kopiera till GitHub

git checkout master  
git merge 1.x-dev  
git push origin master  

=======

##### Log och status  
[master]> *git status* `# Visa aktuella förändringar`  
[master]> *gitk --all* `# Öppna grafiskt statusfönster`  
[master]> *git log --graph --all --oneline* `# List alla commits (avsluta med Q).`  

##### Branch
[master]> *git checkout 1.x-dev* `# Gå till branch`  
[master]> *git branch 1.x-dev* `# Skapa ny branch`  
[master]> *git checkout -b 1.x-dev* `# Skapa och gå till`  

##### Diff
[master]> *git diff* `# Ändringar sen senaste commit`  
[master]> *git diff snippets.md* `# Ändringar i specifik fil`  

##### Tag
[master]> *git tag* `# Lista alla taggar`  
[master]> *git tag test1* `# Lightweight - Namn på en commit`  
[master]> *git tag -a RC1 -m 'the first release candidate'* `# Annotated - Fullt object med info`  

##### Add
[master]> *git add -A* `# Stages All`  
[master]> *git add .* `#  Stages new and modified, without deleted`  
[master]> *git add -u* `# Stages modified and deleted, not new files`  
[master]> *git add -i* `# Addera interaktivt`  
[master]> *?* `# Kommentar`  
[master]> *?* `# Kommentar`  
>>>>>>> 1.x-dev

##### Commit
[master]> *git commit -m 'commit message'* `# Commit changes`  
[master]> *git commit --amend* `# Om man missat något i sista comitten, kompletterar utan att skapa en ny`  

##### GitHub Push/Pull 
[master]> *git push origin master* `# Kopiera till github`  
[master]> *git pull origin master* `# Hämta från github`  

<<<<<<< HEAD
Övrig
Ignorera filer eller mappar genom att skapa en *.gitignore* i aktuell mapp.

=======
##### Commit
[master]> *git commit -m 'commit message'* `# Commit changes`  
[master]> *git commit --amend* `# Om man missat något i sista comitten, kompletterar utan att skapa en ny`  

##### GitHub Push/Pull 
[master]> *git push origin master* `# Kopiera till github`  
[master]> *git pull origin master* `# Hämta från github`  

#### Övrig
>>>>>>> 1.x-dev

##### Radslut
[master]> *git config core.autocrlf false* `Stäng av automatisk hantering av radslut.`  

<<<<<<< HEAD
Log
gitk --all - Gui (windows?)
git log --graph --all --oneline



Tag
$ git tag v0.5.6 - Lightweight
$ git tag -a RC1 -m 'the first release candidate' - Annotated with comment

Add
git add -i - Interactive

Diff
git diff - Change since last commit
git diff index.html Specifik fil
=======
##### Ignorera filer
Ignorera alla filer utom *.gitignore*.
```
*
!.gitignore
```

##### Dummy
[master]> *?* `# Kommentar`  
>>>>>>> 1.x-dev
=======
#### Övrig

##### Radslut
[master]> *git config core.autocrlf false* `Stäng av automatisk hantering av radslut.`  

##### Ignorera filer
Ignorera alla filer utom *.gitignore*.
```
*
!.gitignore
```

##### Dummy
[master]> *?* `# Kommentar`  
>>>>>>> 1.x-dev