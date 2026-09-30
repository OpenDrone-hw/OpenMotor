# Incoming inspection

Draft. It has not been used on a delivery. It lists the checks the production quotation request asks the maker to report, so the same checks can be repeated on receipt. No sample size is set: the source documents do not give one, and it is decided before the first delivery is inspected.

## Checks

| # | Check | How | Record |
|---|---|---|---|
| 1 | Visual | Compare bell finish against the approved gold and green colour references and the logo against the artwork. Look for anodising defects, scratches and dents on bell and base | Pass or fail, photo of any failure |
| 2 | Identity | Stator size, mount pattern and wire length against the released drawing | Measured values |
| 3 | Shaft | Shaft diameter and length against the drawing, straightness by hand rotation | Measured values |
| 4 | Bearing noise | Spin by hand, then run unloaded on the bench. Listen for roughness, rubbing and axial play | Pass or fail |
| 5 | KV | Measure at a fixed supply voltage on the bench and compare with the variant KV | Measured KV |
| 6 | Balance | Run unloaded and check vibration, or dynamic balance on a balancer if one is available | Vibration or residual unbalance |
| 7 | Report | Compare the maker's inspection report for the lot with the results above | Match or mismatch |

## Record

One line per motor in `qc/records/<delivery>.csv`: serial, variant, one column per check, verdict, date, inspector. The verdict is entered by the person who inspected the motor.
