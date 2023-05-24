# README

This is my first *GitHub* repository and I’m training the use of **Git** and *GitHub*.” as a paragraph to the “README.md” fil

#### 1. 
`ls` (list)

   Commandet listar ingenting eftersom vi befinner oss i ett tomt directory.
#### 4. 
`mv` *(move)* `newFile.txt newFolder`
#### 5. 
`cd` *(current directory)* `newFolder`
   
   `ls` i newFolder visar newFile.txt

#### 6. 
  `pwd` *(print working directory)*
    `/Users/lilp/Documents/Nerdy/terminal-git-tutorial/newFolder`

#### 8. 
`touch README.md`

 **touch vs echo** 

- `touch filNamn` skapar en ny tom fil, om filen redan existerar får den en ny timestamp av touch, men inget adderas och innehållet förblir detsamma i en redan befintlig fil, 0 byte läggs till och 0 byte skapas.

- `echo " " > filNamn`   
  
 - `echo " " >> filNamn` 
  
  Den första skapar en fil och skriver ut en tom rad (1 byte). Finns filen så gör `>` att det innehållet skrivs över, `>>` adderar till din text, utan att skriva över, med 1 byte.
     
  `echo` *Detta skriver över filens innehåll*`" > filNamn.txt`
  
  `echo "`*Detta adderas i filen*`" >> filNamn.txt` 

- enbart `> filNamn` skapar en tom fil. Då inget command skrivits blir filen helt tom och utan specifikationer. 0 byte.
#### 9.
Git är ett versionshanteringssystem och är idag det mest använda i världen och som stöds av flest tredjepartsplattformar.
Git håller ordning på och lagrar all data från de ändringar som sker i de filer som kodas, antingen i utvecklarnas lokala repository på sin egen dator eller i ett fjärrrepository (likt ett cloud).
När man pushar innehåll så laddas commitade filer upp från lokalt repo till remote repo.
#### 10.
-  **Modified** - Detta stadie är när uvecklaren gjort ändringar i filen men än inte lagt till den i databasen, stadiet innan detta när filerna endast är tillagda är dem untracked.
-   **Staged** - När en fil är staged betyder det att den är modifierad och redo att med de förändringar som gjorts, och ofta tillsammans med en liten beskrivning på ändringarna,  skapa nästa snapshot för hur filen/filerna i working directory status är precis just nu och blir då en commit.
  En commit har en lista på alla de tidigare snapshots som gjort för samma fil, alltså sina parent commits.Det kallas för en merge commit.
   När en commit inte har några tidigare snapshots kallas den för root commit.
-   **Commited** - Att en fil är commited betyder att utvecklaren har säkrat datan och att den pushats till ett remote repo och blivit tillagt som en del av head revision, den commit utvecklaren pulled från. 
![Getting Started](./JBGzy.png)

#### 12.
`git init` *initiera git*

##### *`Initierade tomt Git-arkiv i /Users/lilp/Documents/Nerdy/terminal-git-tutorial/.git/`* 

#### 14.
`git add .` - *addar allt innehåll i current directory till staging area*
`git add filNamn`- addar filen *filNamn*

#### 15.

`git status` - *Visar status*

#### 16.

`git commit -m "`README file for the repository`" 
    - *Adderar ett meddelande till din commit*
#### 17.
En branch skapas för att flera personer ska kunna arbeta på samma projekt från utan att ändra någonting i MASTER, eller för att kunna arbeta på flera olika funktioner samtidigt. 
För att sedan sammanfoga alla förgreningar i historien använder man `git merge` eller `git rebase`. 
#### 18.
`git branch firstbranch` 
- *detta skapar en gren som heter `firstbranch`*
  
`git switch firstbranch`
- detta gör att jag byter gren från `Main`(*Master*) till `firstbranch`

#### 27.
I’m also learning:
  - HTML
  - CSS
  - JavaScript

#### 28.
`git branch -m <namn>` 
- Detta command byter namn från default (brukar vara master, main, trunk) till ett nytt namn.
- 
 *Glöm inte att radera det förra branchnamnet*
#### 29. 
  `git push –u origin main`

  - Detta command pushar Main branch till github repository.

#### 30.
`cd` *nerdy*

`mkdir` *mistymountain*

`cd` *mistymountain*
##### `git clone url`(https://github.com/Strawbejbi/flowermeadow.git)

Nu finns allt det som befann sig i repo *flowermeadow* även i *mistymountain*