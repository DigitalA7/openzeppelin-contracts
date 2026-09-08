# Tokens de gouvernance

`ERC20Votes` suit une puissance de vote avec des points de contrôle historiques. Déléguer ne transfère pas les tokens.
**Exemple :** Alice délègue ses 10 unités à Bob : Bob reçoit les votes, Alice conserve les unités. Un transfert ultérieur ajuste les votes concernés.
Dans cette implémentation, se déléguer à soi-même active son propre pouvoir de vote. `getPastVotes` consulte un état passé.
**Piège :** le token ne décide ni du quorum, ni des propositions, ni de leur exécution : ces règles appartiennent au système de gouvernance.

[Code](../../contracts/token/ERC20/extensions/ERC20Votes.sol) · [Tests](../../test/token/ERC20/extensions/ERC20Votes.test.js) · [Gouvernance](../../contracts/governance)

[Suite : ERC2981 et royalties](11-royalties-erc2981.md)
