# US Bill Sponsorship Data
This repo contains data on bill sponsorship in the US Senate and US House of Representatives from 1973 (93rd session) to 2019 (115th session). 

The data take the form of separate bipartite incidence matrices for each session and chamber. In a given matrix M, Mik = 1 if legislator *i* sponsored bill *k*, and otherwise is 0. The row names contain the legislator's name, party affiliation, state, and GovTrackID. The column names identify the bill; these data include only bills and joint resolutions because only these have the force of law if passed.

The data is available in two formats:
* `sponsorship.csv.zip` is a zip file that contains a separate CSV file for each chamber and session
* `sponsorship.RData` is an R image that contains a separate sparse matrix for each chamber and session

If you use these data, please cite one or more of the following papers that describe and use the data:
* Neal, Z. P. (2020). A sign of the times? Weak and strong polarization in the US Congress, 1973–2016. Social Networks, 60, 103-112. https://doi.org/10.1016/j.socnet.2018.07.007
* Aref, S., & Neal, Z. (2020). Detecting coalitions by optimally partitioning signed networks of political collaboration. Scientific reports, 10(1), 1-10. https://doi.org/10.1038/s41598-020-58471-z
* Aref, S., & Neal, Z. P. (2021). Identifying hidden coalitions in the US House of Representatives by optimally partitioning signed networks based on generalized balance. Scientific reports, 11(1), 1-9. https://doi.org/10.1038/s41598-021-98139-w
* Domagalski, R., Neal, Z. P., & Sagan, B. (2021). Backbone: An R package for extracting the backbone of bipartite projections. Plos one, 16(1), e0244363. https://doi.org/10.1371/journal.pone.0244363
* Neal, Z. P., Domagalski, R., & Yan, X. (2022). Homophily in collaborations among US House Representatives, 1981–2018. Social Networks, 68, 97-106. https://doi.org/10.1016/j.socnet.2021.04.007
