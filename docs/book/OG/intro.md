(Chap_OGintro)=
# Overlapping Generations Macro Model

Put OG intro here.

To include:
* OG compared to other macro models used for policy analysis. E.g.,:
  * Econometric macro models
    * These predict future macro outcomes based on past data
    * They can be accurate *if there are not policy changes*
    * Drawback is that they can't do counterfactual analysis very well (i.e., can't predict the impact of policy changes)
    * Their biggest use is to form a macroeconomic baseline
  * Solow growth models
    * A classic economic model, can account for counterfactual policy
    * Limited in that uses representative agents, so no distributional analysis
    * Uses an infinitely-lived agent, so no intergenerational impacts available and no ability to model age-specific policies
    * Best suited for long run analysis
  * DSGE models
    * Can model short and long run impacts
    * Can do counterfactual analysis
    * Can have heterogeneous agents (therefore can do distributional analysis across income, e.g.)
    * Uses an infinitely lived agent, so no intergenerational impacts available and no ability to model age-specific policies
    * Solution algorithms are not suitable for large policy changes given the approximations used to solve the model
  * Hybrid macro model (e.g., JCT MEG model)
    * Long run solution is similar to OG models steady-state
    * But in short run, agents are myopic and general equilibrium does not hold
    * Can model short and long run impacts
    * Can do counterfactual analysis
    * Can have heterogeneous agents (therefore can do distributional analysis across income, e.g.)
    * Do have finitely-lived agents so can do intergenerational impacts (but again, not eq'm impacts over the transition from the current state to the long run eq'm
  * Overlapping generations models
    * Can do short and long run analysis and *imposes equilibrium in all periods along the economy's transition path and in the long run steady-state*
    * Can have heterogeneous agents (therefore can do distributional analysis across income, e.g.)
    * Has finitely-lived agents so can do intergenerational impacts
    * Solution algorithm is global and therefore can accommodate large policy changes
* Brief overview of OG-Core + link to its documentation
* How country calibrations interact
* Installing OG-Core
* Running the model
* Changing parameters and running the model (exercises here, just with SS)
* Interpreting output
  * Exercises to use plot and table functions
* Detailing model parameters that would calibrate with country model
  * Macro params -> exercise using pandas datareader to get data from FRED
  * Demographics -> exercise to get UN data for specific country
  * Earnings processes -> exercise to do approximation method of Marcelo


(SecOGintroFootnotes)=
## Footnotes

<!-- [^citation_note]: See {cite}`AuerbachEtAl:1981,AuerbachEtAl:1983`, {cite}`AuerbachKotlikoff:1983a,AuerbachKotlikoff:1983b,AuerbachKotlikoff:1983c`, and {cite}`AuerbachKotlikoff:1985`. -->
