# Wrapped tokens et WETH

Un wrapper immobilise un actif et émet sa représentation.
Ici, `depositFor` reçoit un ERC-20 et crée la même quantité enveloppée ; `withdrawTo` brûle celle-ci et restitue le sous-jacent.
**Exemple :** déposer 10 unités puis en retirer 4 laisse 6 unités, pour un actif sans frais ni rebase.
WETH transforme un dépôt d'ETH natif en solde ERC-20, puis permet le retrait inverse. `ERC20Wrapper` reçoit déjà un ERC-20 : ce n'est pas WETH9.
**Piège :** frais de transfert et variations automatiques de solde peuvent déséquilibrer un wrapper simple. Un actif bridgé ajoute les hypothèses de confiance du bridge.

[Code](../../contracts/token/ERC20/extensions/ERC20Wrapper.sol) · [Tests](../../test/token/ERC20/extensions/ERC20Wrapper.test.js) · [WETH9 externe](https://github.com/gnosis/canonical-weth/blob/master/contracts/WETH9.sol)

[Suite : Wrapper de NFT](07-wrapper-nft.md)
