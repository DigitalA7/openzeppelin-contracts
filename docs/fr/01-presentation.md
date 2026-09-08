# Les tokens : carte et architecture

Un standard décrit une interface ; le projet définit la valeur et les droits associés.
ERC-20 suit des quantités interchangeables ; ERC-721 un propriétaire par identifiant ; ERC-1155 et ERC-6909 des quantités par identifiant.
ERC-4626 représente les parts d'un coffre. Un wrapper représente un actif immobilisé.
Un stablecoin décrit un objectif économique ; un token de gouvernance, un usage.
[x402](https://github.com/DigitalA7/x402/tree/main/docs/fr) organise des paiements HTTP avec des actifs existants.

**Architecture :** les [interfaces](../../contracts/interfaces) décrivent les fonctions ; les [contrats](../../contracts/token) les implémentent ; les extensions ajoutent des comportements ; les [tests](../../test/token) illustrent les cas attendus.
Ce fork conserve le code OpenZeppelin et sa [licence MIT](../../LICENSE).

[Suite : ERC20 et decimales](02-erc20.md)
