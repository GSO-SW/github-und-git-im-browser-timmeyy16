[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/7TgmR-X0)
# GitHub-Einführung für SchülerInnen

Herzlich willkommen zu diesem GitHub-Tutorial! 😊

In der heutigen digitalen Welt ist das Verständnis von Versionierung und Kollaboration bei der Softwareentwicklung unerlässlich. Egal, ob du ein angehender Entwickler, ein Schüler, der an einem Projekt arbeitet, oder einfach nur neugierig bist, dieses Tutorial wird dir die Grundlagen von GitHub näherbringen.

GitHub ist nicht nur ein Werkzeug für professionelle Entwickler. Es kann auch für Schulprojekte, Gruppenarbeiten oder persönliche Projekte genutzt werden. Es hilft dir, deinen Code zu organisieren, Änderungen zu verfolgen und mit anderen zusammenzuarbeiten.

In diesem Tutorial lernen Sie:

+ **Commit**: Ein "Commit" ist im Kontext von Git eine Momentaufnahme Ihres Codes. Es dokumentiert die Änderungen, die Sie vorgenommen haben, und ermöglicht es Ihnen (und anderen), zu einem bestimmten Zeitpunkt in der Entwicklungsgeschichte Ihres Projekts zurückzukehren. [Mehr dazu hier](https://docs.github.com/de/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/about-commits).
+ **Branch**: Eine "Branch" (deutsch: Zweig) ermöglicht es Ihnen, an neuen Features oder Bugfixes zu arbeiten, ohne den Hauptcode (oft "master" oder "main" genannt) zu beeinflussen. Dies ist nützlich, um sicherzustellen, dass der Hauptcode stabil bleibt. [Mehr dazu hier](https://docs.github.com/de/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches).
+ **Pull-Request**: Ein "Pull-Request" ist eine Methode, um Änderungen, die Sie in einem Branch gemacht haben, in den Hauptbranch zu integrieren. Es ist auch eine Möglichkeit, Ihre Änderungen zur Überprüfung und Diskussion vorzulegen, bevor sie in den Hauptcode aufgenommen werden. [Mehr dazu hier](https://docs.github.com/de/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).

Lassen Sie uns beginnen!

---
**Ziel**:
Sie sollen lernen, wie man einfache Fehler in Dokumentationsdateien korrigiert und diese Änderungen in ein Git-Repository einpflegt.

**Ausgangssituation**:   
```
Project
|-- documentation.md
|--hello-world.cs
README.md
```

### 1. Repository-Erstellung
**Was sind Repositorys?**   
Ein Repository (oft einfach "Repo" genannt) ist im Kontext von GitHub ein Speicherort oder Container, in dem alle Dateien für ein bestimmtes Projekt gespeichert werden. Es enthält alle Versionen dieser Dateien, sodass Sie Änderungen über die Zeit verfolgen können. Das ermöglicht es mehreren Personen, an einem Projekt zu arbeiten und ihre Änderungen auf eine organisierte und kollaborative Weise zu verwalten.

In Bezug auf GitHub Classroom:

Wenn Sie diesen Leitfaden durchlaufen, gehen wir davon aus, dass Sie bereits ein Repository über GitHub Classroom erstellt haben. GitHub Classroom ist ein Tool, das speziell entwickelt wurde, um den Unterrichtsprozess für Lehrer und Schüler zu vereinfachen. Wenn Sie über einen Link in GitHub Classroom ein Repository erstellen, wird es automatisch auf "internal" gestellt. Das bedeutet, dass das Repository privat bleibt und nur von den eingeladenen Personen eingesehen werden kann.

Die Erstellung von Repositorys und deren detaillierte Konfiguration sind ein eigenes großes Thema und werden in einem kommenden Tutorial ausführlich behandelt. Für jetzt ist es ausreichend zu wissen, dass Sie ein Arbeitsumfeld haben, in dem Sie Ihre Codeänderungen sicher speichern können.

---

### 2. Änderungen committen

- [ ] 1. **Datei Ändern**
  + In der **'hello-world.cs'** Datei gibt es einen Schreibfehler, den Sie korrigieren sollen.  Korrigieren Sie den Text, indem Sie **"Morld"** durch **"World"** ersetzen.
- [ ] 2. **Änderung übernehmen**   
  + Committen Sie Ihre Änderung indem Sie auf den **"Commit changes..."** - Button clicken.   
    ![Commit changes button](https://github.com/GSO-SW/public_content_gso/blob/a0a27f20e215e2e1ee2b3d24cb645f8ce2cb8a25/Tutorial-Cred/GitHub-Tutorial/commit-changes.PNG)   
  + Geben Sie in einem Commit **immer** ein Commit-Text an, welcher beschreibt, welche Änderung gemacht wurde.
![Commit changes message](https://github.com/GSO-SW/public_content_gso/blob/9c8d1907dbb9c6533055e780fcc8ebc2d2d1c829/Tutorial-Cred/GitHub-Tutorial/Commit-Code.PNG)   
- [ ] 3. **Commits ansehen**
    + Clicken Sie auf commits und sehen sie alle commits auf main ein.   
      ![commits](https://github.com/GSO-SW/public_content_gso/blob/b11dc2c9adfbaef9fdc920e3ab3b86c7ba9fec85/Tutorial-Cred/GitHub-Tutorial/commits.PNG)
    + Clicken Sie auf Ihren letzten Commit und sehen Sie die Änderung ein.
    + Hinterlassen Sie einen Kommentar,in der von Ihnen geänderten Zeile (Zeile wird grün angezeigt). Der kommentar 
      könnte folgendermaßen aussehen:
      ``` # Meine erster GitHub Commit :100:``` Die Formatierung geschied bei GitHub immer im [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)-Format.   
      ![Kommentieren](https://github.com/GSO-SW/public_content_gso/blob/b11dc2c9adfbaef9fdc920e3ab3b86c7ba9fec85/Tutorial-Cred/GitHub-Tutorial/commit-zeile.png)
    + Gehen Sie zu der Datei **'hello-world.cs'** und kopieren Sie den Link zu diser Datei indem Sie ![Kommentieren](https://github.com/GSO-SW/public_content_gso/blob/b11dc2c9adfbaef9fdc920e3ab3b86c7ba9fec85/Tutorial-Cred/GitHub-Tutorial/mehr.PNG) anclicken und anschlißen **' copy permalink'** anklicken.
    + Gehen Sie zu der Datei **'documentation.md'** und fürgen Sien den Link unter die Codezeile.

---

### 3. Neue 'Branch' erstellen
- [ ] 1. **Branch erstellen**   
    + Clicken Sie obe auf die Main-Branch und erstellen Sie eine neu Branch mit dem Namen **'neues_feature'**   
      ![neue Branch](https://github.com/GSO-SW/public_content_gso/blob/e184aade392d0c7970d37bcd2e34bfd6cd60928b/Tutorial-Cred/GitHub-Tutorial/neue-branch.PNG)
    + Wenn Sie jetzt die Branch **'main'** und **'neues_feature'** vergleichen, wird Ihnen auffallen, dass in beiden Zweigen die Dateien gleich sind.
- [ ] 2. **'Änderung in neuer Branch**
    + Gehen Sie sicher das Sie sich in der neuen Branch befinden.   
     ![neue Branch](https://github.com/GSO-SW/public_content_gso/blob/169ac742374452340d62b74a0614e74222e88e11/Tutorial-Cred/GitHub-Tutorial/branch-asuwaehlen.PNG)
    + Gehen Sie zu der Datei **'hello-world.cs'** und fügen sie fogende Zeile zur bestehenden hinzu:   
      ```csharp
      Console.WriteLine("Mein neues Feature");
      ```
    + Commiten Sie wieder die Änderung wieder mit dem **"Commit changes..."** - Button.   
       ![Commit changes button](https://github.com/GSO-SW/public_content_gso/blob/a0a27f20e215e2e1ee2b3d24cb645f8ce2cb8a25/Tutorial-Cred/GitHub-Tutorial/commit-changes.PNG)
    + Vergleichen Sie wieder beide Branches und schauen Sie, ob die Dateien die gleichen sind.
  
---

### 4. Pull-Request erstellen
- [ ] 1. **Pull-Request**
    + Wählen Sie die Branch aus, in der Sie ihr neues Feature umgesetzt haben. Anschließend klicken Sie auf **'contribute'** (beitragen)   
    ![contribute](https://github.com/GSO-SW/public_content_gso/blob/0b5a4ffea367b903e5c6bb57c2d8c5b37e2acf18/Tutorial-Cred/GitHub-Tutorial/contribute.PNG)
    + Clicken Sie auf **'Open pull-request'** um eine Anfrage an die main-Branch zu schicken.
- [ ] 2. **Pull-Request-formulieren**
    + Achten Sie darauf, dass die Anfrage von **'neues_feature'** auf **'main'** gestellet wird
      **base:main <- compare:neues_feature**
    + Fügen Sie einen Text hinzu.
    + Klicken Sie auf **'Create pull request'**   
      ![contribute](https://github.com/GSO-SW/public_content_gso/blob/dfef0330c3f407752783058f4eec03c2f60860e5/Tutorial-Cred/GitHub-Tutorial/Pull-request.PNG)

- [ ] 3. **Pull-Request-mergen**
      Sie haben nun eine Anfrage gestellt die Änderungen von **'neues_feature'** auf **'main'** zu übernehmen.
    + Rufen Sie alle Anfragen auf, indem sie auf **'pull requests'** klicken.    
      ![pull-requests](https://github.com/GSO-SW/public_content_gso/blob/0caaeb783e71af139017928ffcc028e198c72162/Tutorial-Cred/GitHub-Tutorial/all-pull-request.PNG)   
    + Schauen Sie welche Änderung die Anfrag enthät indem sie auf **'Files changed'** klicken.   
      ![files-changed](https://github.com/GSO-SW/public_content_gso/blob/0caaeb783e71af139017928ffcc028e198c72162/Tutorial-Cred/GitHub-Tutorial/File-changes.PNG)   
    + Zurück auf **'conversation'** können Sie, den Änderungen zustimmen. Die Branch **'neues_feature'** wird mit der Branch **'main'** gemerged (verschmolzen). Hierfür klicken Sie auf **'Merge pull request'**.   
      ![merge](https://github.com/GSO-SW/public_content_gso/blob/0caaeb783e71af139017928ffcc028e198c72162/Tutorial-Cred/GitHub-Tutorial/merge-pull-request.PNG)   
    + Vergewissern Sie sich das die Änderungen in die main-Branch übernommen wurden.
  
