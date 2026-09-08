# Modèles économiques et extensions

Un stablecoin vise une stabilité de valeur ; un token de liquidité représente des droits sur une position ; un rebase ajuste des soldes sans transfert individuel. Ces notions ne désignent pas de nouvelles interfaces ERC.
Pour chaque actif, identifier le droit obtenu, la formule de remboursement et les personnes capables de modifier le système.
`Burnable`, `Capped` et `Pausable` ajoutent des capacités techniques combinables avec ERC-20.
Ici, `ERC20Pausable` bloque transferts, mint et burn via `_update` ; les fonctions publiques de pause et leurs permissions restent à ajouter.
**Piège :** partager un standard ne signifie pas partager les mêmes garanties économiques.

[Pause](../../contracts/token/ERC20/extensions/ERC20Pausable.sol) · [Tests](../../test/token/ERC20/extensions/ERC20Pausable.test.js) · [Livre DEX](https://github.com/DigitalA7/v4-by-example)

[Suite : Limites et verification documentaire](14-limites-et-verification.md)
