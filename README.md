# Dag 9 · Git-grunderna

_Modul 4, UI/UX & Frontendutveckling, Lexicon IT-Proffs_

## Vad du ska göra idag

Du går från att köra Git som ett recept till att förstå det: `status`, `add`, `commit`, `log`, `diff` och `restore`. Du gör minst sex commits med begripliga meddelanden och pushar dem.

## Bakgrund

Git är ett system som sparar historik över dina filer. Varje _commit_ är ett sparat läge med ett meddelande. Du kan alltid gå tillbaka, och alla som tittar på din kod kan se hur arbetet växte fram. Du har kört `add`, `commit` och `push` som ett recept sedan dag 1. Idag förstår du vad de gör. Dag 10 publicerar du på riktigt med GitHub Pages.

## Så arbetar du (samma som alltid)

1. **Forka** dagens repo på GitHub (_Fork → Create fork_).
2. **Klona din fork:** _Code → HTTPS → kopiera adressen_. I terminalen (Ctrl+ö i VS Code): `git clone <adressen>`. Öppna den nya mappen i VS Code och starta _Live Server_.
3. **Gör uppgiften.** Spara och kontrollera i webbläsaren efter varje steg. Gör en commit efter varje avslutat steg: `git add .` och `git commit -m "Beskriv vad du gjorde"`.
4. **Skicka upp** när du är klar: `git push`.
5. **Lämna in i Microsoft Forms.**

Fastnar du: skriv ner exakt var och vad du försökt, och ta det först i nästa handledda pass.

## Uppgiften steg för steg

### Steg 1. Kontrollera Git

Öppna terminalen i VS Code. Skriv `git --version`. Du ska få ett versionsnummer. Skriv sedan `git config user.name` och `git config user.email`. Saknas något: `git config --global user.name "Ditt Namn"` och motsvarande för e-post.

### Steg 2. Titta på läget

I mappen du klonade: `git status`. Läs vad det står, ord för ord. Du ska se "nothing to commit, working tree clean".

### Steg 3. Din första ändring och commit

Ändra titeln i `index.html` till något eget. Kör `git status` (filen är röd), `git add index.html` (grön), `git commit -m "Ändra sidans titel"`. Kör `git log --oneline` och se din commit.

### Steg 4. Gör fem commits till

Gör fem ytterligare små ändringar, en i taget, och gör en commit för varje:

1. ändra en rubriktext
2. lägg till en fjärde maträtt i menyn
3. ändra färgen `--color-primary`
4. lägg till en rad i `README.md` om dig själv
5. ändra öppettiderna i Om oss

Kör alltid `git status` före `git add` och `git log --oneline` efter.

### Steg 5. Skriv bra commit-meddelanden

Ett bra meddelande säger _vad_ och _varför_, i presens eller imperativ: "Lägg till fjärde maträtt i menyn". Undvik "ändrat", "fix", "asdf".

### Steg 6. Se skillnaden

Ändra något utan att committa. Kör `git diff` och läs vad Git ser. Ångra sedan med `git restore <filnamn>`.

### Steg 7. Skicka upp

Kör `git push` och kontrollera på GitHub att alla dina nya commits syns under _Commits_.

## Kontrollista: så vet du att du är klar

- [ ] `git log --oneline` visar minst sex commits med begripliga meddelanden i övningsrepot.
- [ ] Du kan förklara vad `status`, `add`, `commit` och `log` gör.
- [ ] Du har använt `git diff` och `git restore` minst en gång.
- [ ] Du har klistrat in din `git log --oneline` i Forms.

## Tips om du fastnar

- `git: command not found`? Starta om VS Code. Fungerar det fortfarande: be om hjälp i handledningen.
- "Please tell me who you are"? Du har inte ställt in namn och e-post, se steg 1.
- Fastnat i en konstig skärm med `:`? Tryck `q`.
- Läs alltid vad Git säger. Det är oftast ett ganska tydligt meddelande.

## Inlämning

**Deadline: imorgon klockan 09.00.** Allt lämnas in i Microsoft Forms. Du behöver inte redovisa något muntligt.

I formuläret fyller du i:

1. Länk till din fork av det här repot.
2. Reflektion: Klistra in utskriften från `git log --oneline` och skriv vilket av dina commit-meddelanden du är mest nöjd med och varför.

## Vill du mer? (frivilligt)

- Läs om `git commit --amend` och ändra ett meddelande.
- Skapa en `.gitignore` med `.DS_Store`.

---

English Translation :D

# Day 9 · Git Basics

_Module 4, UI/UX & Frontend Development, Lexicon IT-Proffs_

## What to do today

You go from running Git as a recipe to understanding it: `status`, `add`, `commit`, `log`, `diff` and `restore`. You make at least six commits with understandable messages and push them.

## Background

Git is a system that saves history of your files. Each _commit_ is a saved state with a message. You can always go back, and anyone looking at your code can see how the work evolved. You have been running `add`, `commit` and `push` as a recipe since day 1. Today you understand what they do. On day 10 you publish for real with GitHub Pages.

## How you work (same as always)

1. **Fork** today's repo on GitHub (_Fork → Create fork_).
2. **Clone your fork:** _Code → HTTPS → copy the address_. In the terminal (Ctrl+ö in VS Code): `git clone <address>`. Open the new folder in VS Code and start _Live Server_.
3. **Do the task.** Save and check in the browser after each step. Make a commit after each completed step: `git add .` and `git commit -m "Describe what you did"`.
4. **Submit** when you're done: `git push`.
5. **Submit to Microsoft Forms.**

If you get stuck: write down exactly where and what you tried, and take it first in the next guided session.

## The task step by step

### Step 1. Check Git

Open the terminal in VS Code. Type `git --version`. You should get a version number. Then type `git config user.name` and `git config user.email`. Missing something: `git config --global user.name "Your Name"` and equivalent for email.

### Step 2. Check the status

In the folder you cloned: `git status`. Read what it says, word for word. You should see "nothing to commit, working tree clean".

### Step 3. Your first change and commit

Change the title in `index.html` to something of your own. Run `git status` (the file is red), `git add index.html` (green), `git commit -m "Change page title"`. Run `git log --oneline` and see your commit.

### Step 4. Make five more commits

Make five more small changes, one at a time, and commit each one:

1. change a title text
2. add a fourth dish to the menu
3. change the color `--color-primary`
4. add a line to `README.md` about yourself
5. change the opening hours in About us

Always run `git status` before `git add` and `git log --oneline` after.

### Step 5. Write good commit messages

A good message says _what_ and _why_, in the present tense or imperative: "Add fourth dish to the menu". Avoid "changed", "fix", "asdf".

### Step 6. See the difference

Change something without committing. Run `git diff` and read what Git sees. Then undo with `git restore <filename>`.

### Step 7. Submit

Run `git push` and check on GitHub that all your new commits are visible under _Commits_.

## Checklist: how to know you're done

- [ ] `git log --oneline` shows at least six commits with understandable messages in the practice repo.
- [ ] You can explain what `status`, `add`, `commit` and `log` do.
- [ ] You've used `git diff` and `git restore` at least once.
- [ ] You've pasted your `git log --oneline` into Forms.

## Tips if you get stuck

- `git: command not found`? Restart VS Code. If it still works: ask for help in the tutorial.
- "Please tell me who you are"? You haven't set your name and email, see step 1.
- Stuck on a strange screen with `:`? Press `q`.
- Always read what Git says. It's usually a pretty clear message.

## Submission

**Deadline: tomorrow at 09:00.** Everything is submitted in Microsoft Forms. You don't need to present anything verbally.

In the form, fill in:

1. Link to your fork of this repo.

2. Reflection: Paste the output from `git log --oneline` and write which of your commit messages you are most satisfied with and why.

## Want more? (optional)

- Read about `git commit --amend` and change a message.
- Create a `.gitignore` with `.DS_Store`.
