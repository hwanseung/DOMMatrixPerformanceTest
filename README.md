# DOMMatrixPerformanceTest
https://hwanseung.github.io/DOMMatrixPerformanceTest

### default
| count   |        polyfill       |        native        |
|---------|:---------------------:|:--------------------:|
|      10 | 1.5950000000000273ms | 5.57000000000005ms   |
|     100 | 8.620000000000005ms  | 26.49000000000001ms  |
|    1000 | 11.659999999999968ms | 268.0799999999999ms  |
|   10000 | 58.2650000000001ms   | 2676.46ms            |
(in my local computer)


### parameter of multiply function was changed to DOMMatrixReadOnly instead of DOMMatrixInit.
* https://codereview.chromium.org/2606023002/
| count   |        polyfill       |        native        |
|---------|:---------------------:|:--------------------:|
|      10 | 0.14500000000043656ms | 0.2900000000008731ms |
|     100 | 1.110000000000582ms   | 0.9949999999953434ms |
|    1000 | 4.959999999999127ms   | 7.989999999997963ms  |
|   10000 | 53.06999999999971ms   | 83.79500000000553ms  |
|  100000 | 480.7350000000006ms   | 851.5449999999983ms  |
| 1000000 | 4807.380000000005ms   | 9599.649999999994ms  |
(in my local computer)
