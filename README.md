# actigraphy-processing

## Code for bachelor thesis: Automated diagnose of sleep disorders using actigraphy wearable device

|SO threshold | time window (minutes) | angle | sensitivity (%)| specificity (%)|accuracy (%)|MCC (-)| note |
| --- | --- | --- | --- | --- | --- | --- | ---|
|10 |3  |5 | 78.18| 65.78| 75.15|    0.39| ...|
|10 |5  |5 | 70.41	|75.54| 72.04|   0.38| ...|
|10 |10 |5 | 53.91|  83.94| 62.87	 |      0.31| ...|    
| --- | --- | --- | --- | --- | --- | --- |  ---|
|10 |5 |10 | 75.99 | 70.37 | 74.83 | 0.40 | balanced|
|10 |3 |10 | 82.61 | 60.61 | 77.03 | 0.40 | max accuracy|
|10 |10 |3 | 48.96 | 85.32 | 59.55 | 0.28 | max specificity|
|3 |3 |10 | 83.66 | 54.11 | 75.94 | 0.36 | max sensitivity|

Tried out (+ combination): |SO threshold 3,5,10 | time window (minutes) 3,5,10 | angle 3,5,10 |
