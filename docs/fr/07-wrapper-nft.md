# Envelopper un NFT

`ERC721Wrapper` conserve l'original et crée un NFT portant le même identifiant, par exemple pour ajouter des fonctions de gouvernance.
**Exemple :** Alice approuve le wrapper puis dépose le NFT 42. Le wrapper garde l'original ; Alice reçoit sa représentation 42.
Le retrait brûle la représentation et restitue l'original au destinataire choisi. Transférer la représentation peut donc changer qui récupérera l'original.
**Piège :** un transfert direct avec `transferFrom` ne déclenche pas le callback. Utiliser le parcours prévu ; une récupération dépend des fonctions exposées par le contrat final.

[Code](../../contracts/token/ERC721/extensions/ERC721Wrapper.sol) · [Tests](../../test/token/ERC721/extensions/ERC721Wrapper.test.js)

[Suite : ERC4626 et parts de coffre](08-erc4626-coffres.md)
