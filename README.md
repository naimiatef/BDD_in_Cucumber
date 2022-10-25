# Cucumber :
- Cucumber est un framework pour l’implémentation de scénarios de type BDD (Behavior-Driven-Development).
- Cucumber est un cadre de test qui prend en charge le développement axé sur le comportement (BDD).
- Cucumber lui-même est écrit en Ruby, mais il peut être utilisé pour « tester » le code écrit en Ruby ou d’autres langages, y compris, mais sans s’y limiter, Java, C # et Python.
- Cucumber utilise un ***anglais simple*** au format ***Gherkin*** pour exprimer les histoires d’utilisateurs.
- On peut récupérer les script Gherkin via l'api RestAssured
- Cucumber est totalement compatible avec l'outil open source Squash, qui permet de scripter le test en français également.
# BDD (Behavior-Driven-Development) :
- Le BDD est une ***approche*** proposée par Dan North dans son article Introducing BDD. Le fondement du BDD est ***moins de raisonner en terme de tests que de comportements d’un système***.
-  Pour faciliter la communication, il propose de suivre un formalisme simple pour écrire des scénarios : ***Given***, ***When***, ***Then***
    -  Le ***Given*** mot-clé précède le texte définissant le contexte; l'état connu du système (ou condition préalable).
    -  Le ***When*** mot-clé précède le texte définissant une action.
    -  Le ***Then*** mot-clé précède le texte définissant le résultat de l'action sur le contexte (ou résultat attendu).
# Écrire des scénarios avec Cucumber:
- Cucumber permet de rédiger des scénarios en suivant un formalisme appelé le langage ***Gherkin***. 
- Les scénarios sont regroupés par fonctionnalité (***feature***). Ils sont écrits dans un simple fichier texte. Par défaut, Cucumber s’attend à ce que le fichier porte l’extension ***.feature***.
- Imaginons que nous voulions tester le *********************. Nous pourrions écrire les scénarios suivant dans le fichier PlayHagman.feature :
```
Feature: Update password
Scenario: Admin user can update the user password
Given I am in the HR system with an Admin account
When I update password of another user
Then I receive a message for updating password successfully
And user password is updated to the new password
```
