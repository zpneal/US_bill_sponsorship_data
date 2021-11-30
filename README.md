# US Bill Sponsorship Data
This repo contains data on bill sponsorship in the US Senate and US House of Representatives from 1973 (93rd session) to 2019 (115th session). 

The data take the form of separate bipartite incidence matrices for each session and chamber. In a given matrix **M**, M<sub>ik</sub> = 1 if legislator *i* sponsored bill *k*, and otherwise is 0. The row names contain the legislator's name, party affiliation, state, and GovTrackID. The column names identify the bill; these data include only bills and joint resolutions because only these have the force of law if passed.

There are a couple cautions about these data:
* They do not distinguish a bill's *sponsor* (the first person named on the bill) and its *co-sponsors* (all subsequently named sponsors).
* They include only bills and joint resolutions because only these have the force of law if passed. They do not contain simple resolutions or concurrent resolutions.
* Before the 96th session, a bill in the US House of Representatives could have a *maximum* of 25 sponsors.
* A weighted one-mode co-sponsorship network, where the strength of the edge between two legislators is the number of bills they sponsored together, can be generated via bipartite projection. This can be useful for studying political networks and collaboration relations, however see Neal (2014).

The data are available in two formats:
* `sponsorship.csv.zip` is a zip file that contains a separate CSV file for each chamber and session
* `sponsorship.RData` is an R image that contains a separate sparse matrix for each chamber and session

If you use these data, please cite one or more of the following papers that describe and use the data:
* Neal, Z. (2014). The backbone of bipartite projections: Inferring relationships from co-authorship, co-sponsorship, co-attendance and other co-behaviors. Social Networks, 39, 84-97.
* Neal, Z. P. (2020). A sign of the times? Weak and strong polarization in the US Congress, 1973–2016. Social Networks, 60, 103-112. https://doi.org/10.1016/j.socnet.2018.07.007
* Aref, S., & Neal, Z. (2020). Detecting coalitions by optimally partitioning signed networks of political collaboration. Scientific reports, 10(1), 1-10. https://doi.org/10.1038/s41598-020-58471-z
* Aref, S., & Neal, Z. P. (2021). Identifying hidden coalitions in the US House of Representatives by optimally partitioning signed networks based on generalized balance. Scientific reports, 11(1), 1-9. https://doi.org/10.1038/s41598-021-98139-w
* Domagalski, R., Neal, Z. P., & Sagan, B. (2021). Backbone: An R package for extracting the backbone of bipartite projections. Plos one, 16(1), e0244363. https://doi.org/10.1371/journal.pone.0244363
* Neal, Z. P., Domagalski, R., & Yan, X. (2022). Homophily in collaborations among US House Representatives, 1981–2018. Social Networks, 68, 97-106. https://doi.org/10.1016/j.socnet.2021.04.007

If you have any questions about these data, or run into any problems using it, please contact me by email at [zpneal@msu.edu](mailto:zpneal@msu.edu) or on Twitter at [@zpneal](https://twitter.com/zpneal).
