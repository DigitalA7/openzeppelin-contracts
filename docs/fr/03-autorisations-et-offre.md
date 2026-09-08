# Autorisations, mint et burn

`approve` accorde une autorisation ; `transferFrom` permet au bénéficiaire de la consommer. Approuver ne transfère rien.
**Exemple :** autorisation de 5, dépense de 2 : reste 3. Ici, une autorisation maximale `uint256` n'est pas décrémentée.
`ERC20Burnable` permet de brûler ses tokens, ou ceux d'un titulaire ayant autorisé la dépense.
`ERC20Capped` limite l'offre courante : un burn peut libérer une capacité de mint.
Les fonctions publiques de mint et leurs permissions restent à définir par le projet.
`SafeERC20` gère différentes valeurs de retour ; il ne garantit pas la valeur économique du token.

[Burn](../../contracts/token/ERC20/extensions/ERC20Burnable.sol) · [Plafond](../../contracts/token/ERC20/extensions/ERC20Capped.sol) · [Appels](../../contracts/token/ERC20/utils/SafeERC20.sol) · [Tests](../../test/token/ERC20/ERC20.behavior.js)

[Suite : ERC721 et NFT](04-erc721.md)
