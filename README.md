# GroceryApp 

## Gitflow:  
Ik maak gebruik van deze branch structuur:
```
Main
└── Dev
	└──Feature/...
└──Hotfix/...
```

In commit messages gebruik ik een vaste template:  
*voorbeelden:*
```
feat(client): add EmailAddress and Password properties
fix(login): verify password using PasswordHelper
docs(readme): add GitFlow structure with emojis
```
De commit message bestaat uit vaste onderdelen:
```
<type>(<wat>): <korte omschrijving>
```
Types:
| Type     | Wat is het?                                    | Branch          |
| -------- | ---------------------------------------------- | --------------- |
| update   | groote update van dev -> main                  | main            |
| hotfix   | hotfix                                         | main/hotfix/... |
| feat     | nieuwe feature                                 | dev/feature/... |
| bugfix   | bugfix                                         | dev/bugfix/...  |
| docs     | documentatie                                   | dev/docs/...    |
| test     | toevoegen / aanpassen van tests                | dev/test/...    |
| style    | format, linting, whitespace                    | dev/style/...   |
| refactor | code refactor (geen nieuwe feature / geen bug) | dev             |  

## Use cases:  
**UC01 Tonen boodschappenlijsten**  
Is compleet.

**UC02 Tonen inhoud boodschappenlijst**   
In het bestand `GroceryListItem.cs` uit het project Grocery.Core.Models:
- De member variabelen wijzigen in properties
- In de constructor de doorgegeven waarden koppelen aan de properties.

**UC03 Tonen producten**  
In het bestand `ProductRepository.cs` uit het project Grocery.Core.Data:
- Initieer in de constructor de lijst met 4 nieuwe producten:  
  - Melk[voorraad 300]
  - Kaas[voorraad 100]
  - Brood[voorraad 400]
  - Cornflakes[voorraad 0]
- In de methode GetAll() zorg je dat de lijst met producten wordt meegegeven.
