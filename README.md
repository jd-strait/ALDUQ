# ALDUQ
Automatic landmark detection model for planar shape data

Detailedcode.zip is a zipped folder containing the following Matlab programs:

**Main programs**

`ALDfixed.m` - MCMC for fixed number of landmarks model (inferring \theta)
`ALDunknown.m` - MCMC for unknown number of landmarks model (inferring k and \theta)
`FindBestk.m` - repeated parallel MCMC runs of ALDfixed.m for criterion-based approach for selecting number of landmarks

**Sub programs**

`ClosedIntSqDist.m`
`curve_to_q.m`
`InnerProd_Q.m`
`MoveProb.m`
`OpenIntSqDist.m`
`q_to_curve.m`
`ReSampleCurve.m`
`ShiftF.m`

Wrapper to replicate paper examples from "Automatic Detection and Uncertainty Quantification of Landmarks on Elastic Curves" (https://www.tandfonline.com/doi/full/10.1080/01621459.2018.1527224):

`ExampleCode.m`

**Data**

`mice.mat` (with help file `MiceLabels.txt`)
`MPEG7closed.mat` (with help file `MPEG7closedLabels.txt`)
`ToyCurve.mat` (with help file `ToyCurveLabels.txt`)

E-mail Justin Strait (justin.strait@uga.edu) with any questions about the code.
