# Dax-Measures-Top-Using-Top-N
Dax Measures Top Using Top N
Top3CertificatesByBudget =
TOPN(
    3,
    SUMMARIZE(
        Movies,
        Movies[Certificate],
        "TotalBudget", SUM(Movies[Budget])
    ),
    [TotalBudget],
    DESC
)
