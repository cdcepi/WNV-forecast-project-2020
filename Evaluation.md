### Evaluation

Final reported data for 2020 will finalized in 2021. An analysis will be conducted using the average logarithmic score to assess and compare forecasts across all counties at each time point. A joint manuscript will be prepared to disseminate findings on this comparison and the general performance of submitted forecasts. Participants may publish their own forecasts and results at any time.

**Eligibility**

To be eligible, teams must:

1.	Submit forecasts for all 3,109 counties.

2.	Submit forecasts electronically prior to the deadline (April 30, 2020).

3.	Submit a model description (see [Participation](Participation.md)).

**Results**

Preliminary results will be distributed to all teams. 

### Logarithmic Score

If $p$ is the set of probabilities for a given forecast, and $p_i$ is the probability assigned to the observed outcome $i$, the logarithmic score is:

$$S(p, i) = ln(p_i)$$

For each forecast of each target, $p_i$ will be set to the probability assigned to the single bin containing the observed outcome. Undefined natural logs (which occur when the probability assigned to the observed outcome was 0) will be assigned a value of -10.

**References**

*	Gneiting T and AE Raftery. (2007) Strictly proper scoring rules, prediction, and estimation. Journal of the American Statistical Association. 102(477):359-378. Available at: [https://www.stat.washington.edu/raftery/Research/PDF/Gneiting2007jasa.pdf](https://www.stat.washington.edu/raftery/Research/PDF/Gneiting2007jasa.pdf).
*	Rosenfeld R, J Grefenstette, and D Burke. (2012) A Proposal for Standardized Evaluation of Epidemiological Models. Available at: [http://delphi.midas.cs.cmu.edu/files/StandardizedEvaluationRevised12-11-09.pdf](http://delphi.midas.cs.cmu.edu/files/StandardizedEvaluationRevised12-11-09.pdf).
