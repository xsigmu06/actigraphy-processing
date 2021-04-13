# actigraphy-processing

## Code for bachelor thesis: Automated diagnose of sleep disorders using actigraphy wearable device

+ if github won't load .ipynb file: https://nbviewer.jupyter.org/github/xsigmu06/actigraphy-processing/tree/main/

### Algorithm results

- Tested (+ combination = 27 total): | SO threshold 3,5,10 | time window (minutes) 3,5,10 | angle 3,5,10 |

|SO threshold | time window (minutes) | angle | sensitivity (%)| specificity (%)|accuracy (%)|MCC (-)| note |
| --- | --- | --- | --- | --- | --- | --- | ---|
|10 |3  |5 | 78.18| 65.78| 75.15|    0.39| - |
|10 |5  |5 | 70.41	|75.54| 72.04|   0.38| - |
|10 |10 |5 | 53.91|  83.94| 62.87	 |      0.31| - |    
| ... | ... | ... | ... | ... | ... | ... |  ... |
|10 |5 |10 | 75.99 | 70.37 | 74.83 | 0.40 | balanced|
|10 |3 |10 | 82.61 | 60.61 | 77.03 | 0.40 | accuracy|
|10 |10 |3 | 48.96 | 85.32 | 59.55 | 0.28 | specificity|
|3 |3 |10 | 83.66 | 54.11 | 75.94 | 0.36 | sensitivity|


### Feature definitions

|TIB|SOL|TST|WASO|SWR|SFI|SE|
|---|---|---|---|---|---|---|
|Time In Bed|Sleep Onset Latency|Total Sleep Time|Wake After Sleep Onset|Sleep-Wake Ratio|Sleep Fragmentation Index|Sleep Efficiency|
|min|min|min|min|-|-|%|
| duration of time in bed (possibly without non-sleep activities)| duration of wake epochs before sleep onset)| duration of all sleep epochs| duration of wake epochs from SO to sleep end| TST/WASO| number of wake intervals from SO to sleep end / TST in hours | TST/TIB*100|
+ 1 epoch = 30 s
