**An Interactive Dashboard for the Mixed Strategy Nash Equilibrium in the Production Attacker-Defender Contest**

This Google Colab Notebook contains an interactive dashboard depicting the single mixed strategy Nash equilibrium and related key variables for the Production Attacker-Defender Contest, depending on production threshold T and production payoff k. The dashboard is created in Python.

The Production Attacker-Defender Contest (henceforth, PAD-C) is an asymmetrical contest model (cf. De Dreu & Gross, 2019). Both attacker and defender enter the interaction with an endowment e, and decide how much of their endowment to invest in attack (for the attacker, a) or in defending against such an attack (for the defender, d). Conflict investments are lost, but if the attacker’s investment exceeds that of the defender (a > d), the attacker appropriates the defender's remaining endowment and any potential production winnings and adds them to their own remaining endowment. In contrast, if d is equal to or larger than a, both keep their remaining endowments and potential production winnings. Both parties may also invest all or part of their endowment in production, denoted by b_Att and b_Def. To be successful at production, an individual’s production investment must meet or exceed a fixed threshold T (with 0 ≤ T ≤ e). If they reach or exceed threshold T, each player receives a fixed reward k. Production investments are non-recoverable and made simultaneously with the conflict investments (a and d). The total amount invested in production and attack (or defense) is thus constrained by e such that a + b_Att ≤ e and d + b_Def ≤ e. It is assumed that agents know the threshold at the start of the game. 

The model makes two assumptions regarding the relationship between the parameters. First, production is only feasible if the initial endowment can cover it, that is, with e ≥ T. Second, whenever k ≤ T, and investments in production give a negative return, the production technology is deemed inefficient and not used. Since this reduces the PAD-C game to a normal Attacker-Defender Contest, I also assume k > T. 

The PAD-C has a single mixed-strategy equilibrium (see Méder et al., 2022, for a detailed analysis). For the dashboard, I use the Lemke-Howson algorithm (Lemke & Howson, 1964) to calculate game-theoretic equilibria depending on k and T. 

*References*

De Dreu, C., & Gross, J. (2019). Revisiting the form and function of conflict: Neurobiological, psychological, and cultural mechanisms for attack and defense within and between groups. Behavioral and Brain Sciences, 42, E116. doi:10.1017/S0140525X18002170

Lemke, C. E., & Howson, J. T. (1964). Equilibrium Points of Bimatrix Games. Journal of the Society for Industrial and Applied Mathematics, 12, 413–423.

Méder, Z., Dreu, C. K. W. D., & Gross, J. (2022). Equlibria of Attacker-Defender Games. ArXiv. doi.org/10.48550/arXiv.2202.10072

