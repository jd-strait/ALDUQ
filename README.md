# ALDUQ
Automatic landmark detection model for planar shape data

Detailedcode.zip is a zipped folder containing the following Matlab programs:

**Main programs**

`ALDfixed.m` - Metropolis-Hastings sampler for fixed number of landmarks model (inferring \theta)

`ALDunknown.m` - reversible jump MCMC for unknown number of landmarks model (inferring k and \theta)

`FindBestk.m` - repeated parallel MCMC runs of ALDfixed.m for criterion-based approach for selecting number of landmarks

**Sub programs**

`ClosedIntSqDist.m` - evaluate distance between closed curve and its linear reconstruction through landmarks

`curve_to_q.m` - convert a two-dimensional curve to its SRVF representation

`InnerProd_Q.m` - compute L2 inner product

`MoveProb.m` - evaluates move probabilities for RJMCMC

`OpenIntSqDist.m` - evaluate distance between open curve and its linear reconstruction through landmarks

`q_to_curve.m` - convert a SRVF to its two-dimensional curve representation

`ReSampleCurve.m` - assuming a dense grid, re-samples two-dimensional curves (at equal spacings) to a desired number of points

`ShiftF.m` - used to shift the starting point of a closed curve (important for posterior processing of labels)

Wrapper to replicate paper examples from "Automatic Detection and Uncertainty Quantification of Landmarks on Elastic Curves" (https://www.tandfonline.com/doi/full/10.1080/01621459.2018.1527224):

`ExampleCode.m`

**Data**

`mice.mat` (with help file `MiceLabels.txt`)

`MPEG7closed.mat` (with help file `MPEG7closedLabels.txt`)

`ToyCurve.mat` (with help file `ToyCurveLabels.txt`)

E-mail Justin Strait (justin.strait@uga.edu) with any questions about the code.
