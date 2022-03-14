# SportsImageClassification

## Introduction

Sports Classification has considerable importance for digital content in broadcasting companies. Basically, it is a part of human action recognition, which further extends us to video classification. But as of now, in this repository, I have classified the images of 7 different sports aka: Cricket, Swimming, Soccer, Karate, Wrestling, Tennis, Badminton.

## Dataset

Here's the dataset : https://www.kaggle.com/vineeth1999/pgpdataset2022mar07
Original Source (Credits to Dataset): https://s3-ap-southeast-1.amazonaws.com/he-public-data/datasetaff9788.zip

## Data Analysis

- There are totally *8227 training images* and *2056 test images* in the dataset.
- 7 different sports namely Cricket, Swimming, Soccer, Karate, Wrestling, Tennis, Badminton.

Some of the images in the training set can be viewed below:

![alt.text](https://www.kaggleusercontent.com/kf/89665616/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..7JB3LdWm1_SJ8Tf7WieBKQ.MbyxaM89BmMQJW94PNXZpHqIwYFaYwHx55BqhtYeNLQfyAz5v8bwuM6a2wvmLjEEPqgnL3CMNym7qvrHj-Xexbw9u_or_WPyVSwvGMcYFhGBYVpPwlhbToI6OrNTrGWOSyMUhbQWLL-PuIcu4VHm-a0cP-i5O7GhA8f-Db5ToD_nB0Lnxrh7oRi2yZLtlsTZ5GageAsz7ZSVM2RmC_1SQjXNLmv70Rpweh7tz4qjhyE6ubTZrSKKwWHAW7GEpGbHf-G6r59M5nV6ty_qA2CgGsJ1Jw103d7z0INNUW2PK4U-pi9zjtXQ9mNI3WvSHVUzL2-zL55RAjo6tfFmSRDvh-y7dvwYl8P7SB-SLM34hXy2Bcmvu8f_-AqlnTMyeSeVIUqV3uIw1zmXLE8Atgy3AMbV_2TJwQVDsvX_53S8AHXdeBJ3BfeIzzm2b-DYTdKtDBb-XhhKZ1o9GId8MZaOcLndi3e1SohOZKBsaCUWSZVPnGAyfaZ-6j5ZL8cznWiAhV-QAuyf-oF4GXQe668vUsxb3GUM-Zu4JxdornL2cQPkWDMKAyKcemm6mgbs1TI0yVZQXvlILOL3ZFVJyFUaLGrpajE9zOvu9U0AEKX_Sm0pfdA0BP1hIzQ37mvPfl_h2NOJksG_nqJ2mz4IQTz0iQ.n4zLrBzhadmEIUX4FvmJ8Q/__results___files/__results___10_0.png)

Some of the images in the testing set can be viewed below:

![alt.text](https://www.kaggleusercontent.com/kf/89665616/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..7JB3LdWm1_SJ8Tf7WieBKQ.MbyxaM89BmMQJW94PNXZpHqIwYFaYwHx55BqhtYeNLQfyAz5v8bwuM6a2wvmLjEEPqgnL3CMNym7qvrHj-Xexbw9u_or_WPyVSwvGMcYFhGBYVpPwlhbToI6OrNTrGWOSyMUhbQWLL-PuIcu4VHm-a0cP-i5O7GhA8f-Db5ToD_nB0Lnxrh7oRi2yZLtlsTZ5GageAsz7ZSVM2RmC_1SQjXNLmv70Rpweh7tz4qjhyE6ubTZrSKKwWHAW7GEpGbHf-G6r59M5nV6ty_qA2CgGsJ1Jw103d7z0INNUW2PK4U-pi9zjtXQ9mNI3WvSHVUzL2-zL55RAjo6tfFmSRDvh-y7dvwYl8P7SB-SLM34hXy2Bcmvu8f_-AqlnTMyeSeVIUqV3uIw1zmXLE8Atgy3AMbV_2TJwQVDsvX_53S8AHXdeBJ3BfeIzzm2b-DYTdKtDBb-XhhKZ1o9GId8MZaOcLndi3e1SohOZKBsaCUWSZVPnGAyfaZ-6j5ZL8cznWiAhV-QAuyf-oF4GXQe668vUsxb3GUM-Zu4JxdornL2cQPkWDMKAyKcemm6mgbs1TI0yVZQXvlILOL3ZFVJyFUaLGrpajE9zOvu9U0AEKX_Sm0pfdA0BP1hIzQ37mvPfl_h2NOJksG_nqJ2mz4IQTz0iQ.n4zLrBzhadmEIUX4FvmJ8Q/__results___files/__results___11_0.png)

Checking the distribution of each label gives us more information about what model we have to choose for training those images. So down we see both the bar distribution and the pie chart distribution:

![alt.text](https://www.kaggleusercontent.com/kf/89665616/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..7JB3LdWm1_SJ8Tf7WieBKQ.MbyxaM89BmMQJW94PNXZpHqIwYFaYwHx55BqhtYeNLQfyAz5v8bwuM6a2wvmLjEEPqgnL3CMNym7qvrHj-Xexbw9u_or_WPyVSwvGMcYFhGBYVpPwlhbToI6OrNTrGWOSyMUhbQWLL-PuIcu4VHm-a0cP-i5O7GhA8f-Db5ToD_nB0Lnxrh7oRi2yZLtlsTZ5GageAsz7ZSVM2RmC_1SQjXNLmv70Rpweh7tz4qjhyE6ubTZrSKKwWHAW7GEpGbHf-G6r59M5nV6ty_qA2CgGsJ1Jw103d7z0INNUW2PK4U-pi9zjtXQ9mNI3WvSHVUzL2-zL55RAjo6tfFmSRDvh-y7dvwYl8P7SB-SLM34hXy2Bcmvu8f_-AqlnTMyeSeVIUqV3uIw1zmXLE8Atgy3AMbV_2TJwQVDsvX_53S8AHXdeBJ3BfeIzzm2b-DYTdKtDBb-XhhKZ1o9GId8MZaOcLndi3e1SohOZKBsaCUWSZVPnGAyfaZ-6j5ZL8cznWiAhV-QAuyf-oF4GXQe668vUsxb3GUM-Zu4JxdornL2cQPkWDMKAyKcemm6mgbs1TI0yVZQXvlILOL3ZFVJyFUaLGrpajE9zOvu9U0AEKX_Sm0pfdA0BP1hIzQ37mvPfl_h2NOJksG_nqJ2mz4IQTz0iQ.n4zLrBzhadmEIUX4FvmJ8Q/__results___files/__results___13_0.png)

![alt.text](https://www.kaggleusercontent.com/kf/89665616/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..7JB3LdWm1_SJ8Tf7WieBKQ.MbyxaM89BmMQJW94PNXZpHqIwYFaYwHx55BqhtYeNLQfyAz5v8bwuM6a2wvmLjEEPqgnL3CMNym7qvrHj-Xexbw9u_or_WPyVSwvGMcYFhGBYVpPwlhbToI6OrNTrGWOSyMUhbQWLL-PuIcu4VHm-a0cP-i5O7GhA8f-Db5ToD_nB0Lnxrh7oRi2yZLtlsTZ5GageAsz7ZSVM2RmC_1SQjXNLmv70Rpweh7tz4qjhyE6ubTZrSKKwWHAW7GEpGbHf-G6r59M5nV6ty_qA2CgGsJ1Jw103d7z0INNUW2PK4U-pi9zjtXQ9mNI3WvSHVUzL2-zL55RAjo6tfFmSRDvh-y7dvwYl8P7SB-SLM34hXy2Bcmvu8f_-AqlnTMyeSeVIUqV3uIw1zmXLE8Atgy3AMbV_2TJwQVDsvX_53S8AHXdeBJ3BfeIzzm2b-DYTdKtDBb-XhhKZ1o9GId8MZaOcLndi3e1SohOZKBsaCUWSZVPnGAyfaZ-6j5ZL8cznWiAhV-QAuyf-oF4GXQe668vUsxb3GUM-Zu4JxdornL2cQPkWDMKAyKcemm6mgbs1TI0yVZQXvlILOL3ZFVJyFUaLGrpajE9zOvu9U0AEKX_Sm0pfdA0BP1hIzQ37mvPfl_h2NOJksG_nqJ2mz4IQTz0iQ.n4zLrBzhadmEIUX4FvmJ8Q/__results___files/__results___14_0.png)

As we can see from the above plots, the *most frequent occuring sport* in the dataset is *Cricket* and *least frequent occuring sport* in the dataset is *Karate*. Hence from the abov plots we can conclude that the number of images order is (*Cricket >Wrestling >Tennis> Badminton> Soccer> Swimming> Karate*). Also we can see an imbalance in the dataset between the top three sport category and the bottom category. We can use smote or sampling techniques to balance the dataset.

So here we can see some random images of the most frequent and least frequent sport in our dataset.

![alt.text](https://www.kaggleusercontent.com/kf/89665616/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..7JB3LdWm1_SJ8Tf7WieBKQ.MbyxaM89BmMQJW94PNXZpHqIwYFaYwHx55BqhtYeNLQfyAz5v8bwuM6a2wvmLjEEPqgnL3CMNym7qvrHj-Xexbw9u_or_WPyVSwvGMcYFhGBYVpPwlhbToI6OrNTrGWOSyMUhbQWLL-PuIcu4VHm-a0cP-i5O7GhA8f-Db5ToD_nB0Lnxrh7oRi2yZLtlsTZ5GageAsz7ZSVM2RmC_1SQjXNLmv70Rpweh7tz4qjhyE6ubTZrSKKwWHAW7GEpGbHf-G6r59M5nV6ty_qA2CgGsJ1Jw103d7z0INNUW2PK4U-pi9zjtXQ9mNI3WvSHVUzL2-zL55RAjo6tfFmSRDvh-y7dvwYl8P7SB-SLM34hXy2Bcmvu8f_-AqlnTMyeSeVIUqV3uIw1zmXLE8Atgy3AMbV_2TJwQVDsvX_53S8AHXdeBJ3BfeIzzm2b-DYTdKtDBb-XhhKZ1o9GId8MZaOcLndi3e1SohOZKBsaCUWSZVPnGAyfaZ-6j5ZL8cznWiAhV-QAuyf-oF4GXQe668vUsxb3GUM-Zu4JxdornL2cQPkWDMKAyKcemm6mgbs1TI0yVZQXvlILOL3ZFVJyFUaLGrpajE9zOvu9U0AEKX_Sm0pfdA0BP1hIzQ37mvPfl_h2NOJksG_nqJ2mz4IQTz0iQ.n4zLrBzhadmEIUX4FvmJ8Q/__results___files/__results___19_0.png)


![alt.text](https://www.kaggleusercontent.com/kf/89665616/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..7JB3LdWm1_SJ8Tf7WieBKQ.MbyxaM89BmMQJW94PNXZpHqIwYFaYwHx55BqhtYeNLQfyAz5v8bwuM6a2wvmLjEEPqgnL3CMNym7qvrHj-Xexbw9u_or_WPyVSwvGMcYFhGBYVpPwlhbToI6OrNTrGWOSyMUhbQWLL-PuIcu4VHm-a0cP-i5O7GhA8f-Db5ToD_nB0Lnxrh7oRi2yZLtlsTZ5GageAsz7ZSVM2RmC_1SQjXNLmv70Rpweh7tz4qjhyE6ubTZrSKKwWHAW7GEpGbHf-G6r59M5nV6ty_qA2CgGsJ1Jw103d7z0INNUW2PK4U-pi9zjtXQ9mNI3WvSHVUzL2-zL55RAjo6tfFmSRDvh-y7dvwYl8P7SB-SLM34hXy2Bcmvu8f_-AqlnTMyeSeVIUqV3uIw1zmXLE8Atgy3AMbV_2TJwQVDsvX_53S8AHXdeBJ3BfeIzzm2b-DYTdKtDBb-XhhKZ1o9GId8MZaOcLndi3e1SohOZKBsaCUWSZVPnGAyfaZ-6j5ZL8cznWiAhV-QAuyf-oF4GXQe668vUsxb3GUM-Zu4JxdornL2cQPkWDMKAyKcemm6mgbs1TI0yVZQXvlILOL3ZFVJyFUaLGrpajE9zOvu9U0AEKX_Sm0pfdA0BP1hIzQ37mvPfl_h2NOJksG_nqJ2mz4IQTz0iQ.n4zLrBzhadmEIUX4FvmJ8Q/__results___files/__results___21_0.png)

## Training:
So I used resnext50 model with Adam optimizer and CrossEntropyLoss to classify these images and trained it for 15 epochs in 5 folds and overall CV was 0.96390. The below plots show how my model performed epoch by epoch in every fold.

![alt.text](https://www.kaggleusercontent.com/kf/89961255/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..D_4fY6wnJdTvTMmHLQHjuw.b2zD69JODzk9bMA3LtXDAvFj-C7HOcfECVcrMAyYLQMXza3i2SIulUSHogJRf5PY4_Co_SD1OLSClGl7Yw9Eg6-qfvDspZ4kLskdj-4dBuFUBRAVuNkHOFsbukc0vGAUfUnW1mmhdm-nW2QG9niyGySZMLQj5tqD4v6GjKG-gV6ucTkEgUgZ9g3n5vN2c7TIMcXgs0tGCKJENfEnBRaSaQTRy0oGd2_vElo74PJ8y05ZkTOIf_kvrCtyGe1yX1eL6flncNDPrTSpCQm8PcCKp4gZ9XZpSsl98ttPNpRV2M6EHm8IaDnY1xIevAHKZiz9OsQg4oG-wmo5Yks0SAj16tKCtrW541TAmbcSlW8Rv3x2MLKf62VSut0TAkJvZxgTkjanDHxZ3Wv3O9KRbBeNjePy3fjczPimVa8oJs-fmL9ifQ_Mnpf55gUvvYuU4axb65f8J0SkOBePEox1R6jQ4NsEvVpxLUxATYqozNZS40tgGtI6VxeIZCmz33_rCpVu76WG7XR29EdHlMDbaR7HggPUI5pR_e-_fP4mnGbfp9nAmRlSA1P8H4BmPzY7kiUXapa0THauo71i0REm1bXRiQzCQ7X2eLCkvW_gE5ULGSvU53U0ThXbxF2FSj_sPx5ZphqNRbF7k_JLoLqp1s4WfQ.BNgdiGbY6-GoYRFwPgbY7w/__results___files/__results___14_32.png)

![alt.text](https://www.kaggleusercontent.com/kf/89961255/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..D_4fY6wnJdTvTMmHLQHjuw.b2zD69JODzk9bMA3LtXDAvFj-C7HOcfECVcrMAyYLQMXza3i2SIulUSHogJRf5PY4_Co_SD1OLSClGl7Yw9Eg6-qfvDspZ4kLskdj-4dBuFUBRAVuNkHOFsbukc0vGAUfUnW1mmhdm-nW2QG9niyGySZMLQj5tqD4v6GjKG-gV6ucTkEgUgZ9g3n5vN2c7TIMcXgs0tGCKJENfEnBRaSaQTRy0oGd2_vElo74PJ8y05ZkTOIf_kvrCtyGe1yX1eL6flncNDPrTSpCQm8PcCKp4gZ9XZpSsl98ttPNpRV2M6EHm8IaDnY1xIevAHKZiz9OsQg4oG-wmo5Yks0SAj16tKCtrW541TAmbcSlW8Rv3x2MLKf62VSut0TAkJvZxgTkjanDHxZ3Wv3O9KRbBeNjePy3fjczPimVa8oJs-fmL9ifQ_Mnpf55gUvvYuU4axb65f8J0SkOBePEox1R6jQ4NsEvVpxLUxATYqozNZS40tgGtI6VxeIZCmz33_rCpVu76WG7XR29EdHlMDbaR7HggPUI5pR_e-_fP4mnGbfp9nAmRlSA1P8H4BmPzY7kiUXapa0THauo71i0REm1bXRiQzCQ7X2eLCkvW_gE5ULGSvU53U0ThXbxF2FSj_sPx5ZphqNRbF7k_JLoLqp1s4WfQ.BNgdiGbY6-GoYRFwPgbY7w/__results___files/__results___14_65.png)

![alt.text](https://www.kaggleusercontent.com/kf/89961255/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..D_4fY6wnJdTvTMmHLQHjuw.b2zD69JODzk9bMA3LtXDAvFj-C7HOcfECVcrMAyYLQMXza3i2SIulUSHogJRf5PY4_Co_SD1OLSClGl7Yw9Eg6-qfvDspZ4kLskdj-4dBuFUBRAVuNkHOFsbukc0vGAUfUnW1mmhdm-nW2QG9niyGySZMLQj5tqD4v6GjKG-gV6ucTkEgUgZ9g3n5vN2c7TIMcXgs0tGCKJENfEnBRaSaQTRy0oGd2_vElo74PJ8y05ZkTOIf_kvrCtyGe1yX1eL6flncNDPrTSpCQm8PcCKp4gZ9XZpSsl98ttPNpRV2M6EHm8IaDnY1xIevAHKZiz9OsQg4oG-wmo5Yks0SAj16tKCtrW541TAmbcSlW8Rv3x2MLKf62VSut0TAkJvZxgTkjanDHxZ3Wv3O9KRbBeNjePy3fjczPimVa8oJs-fmL9ifQ_Mnpf55gUvvYuU4axb65f8J0SkOBePEox1R6jQ4NsEvVpxLUxATYqozNZS40tgGtI6VxeIZCmz33_rCpVu76WG7XR29EdHlMDbaR7HggPUI5pR_e-_fP4mnGbfp9nAmRlSA1P8H4BmPzY7kiUXapa0THauo71i0REm1bXRiQzCQ7X2eLCkvW_gE5ULGSvU53U0ThXbxF2FSj_sPx5ZphqNRbF7k_JLoLqp1s4WfQ.BNgdiGbY6-GoYRFwPgbY7w/__results___files/__results___14_97.png)

![alt.text](https://www.kaggleusercontent.com/kf/89961255/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..D_4fY6wnJdTvTMmHLQHjuw.b2zD69JODzk9bMA3LtXDAvFj-C7HOcfECVcrMAyYLQMXza3i2SIulUSHogJRf5PY4_Co_SD1OLSClGl7Yw9Eg6-qfvDspZ4kLskdj-4dBuFUBRAVuNkHOFsbukc0vGAUfUnW1mmhdm-nW2QG9niyGySZMLQj5tqD4v6GjKG-gV6ucTkEgUgZ9g3n5vN2c7TIMcXgs0tGCKJENfEnBRaSaQTRy0oGd2_vElo74PJ8y05ZkTOIf_kvrCtyGe1yX1eL6flncNDPrTSpCQm8PcCKp4gZ9XZpSsl98ttPNpRV2M6EHm8IaDnY1xIevAHKZiz9OsQg4oG-wmo5Yks0SAj16tKCtrW541TAmbcSlW8Rv3x2MLKf62VSut0TAkJvZxgTkjanDHxZ3Wv3O9KRbBeNjePy3fjczPimVa8oJs-fmL9ifQ_Mnpf55gUvvYuU4axb65f8J0SkOBePEox1R6jQ4NsEvVpxLUxATYqozNZS40tgGtI6VxeIZCmz33_rCpVu76WG7XR29EdHlMDbaR7HggPUI5pR_e-_fP4mnGbfp9nAmRlSA1P8H4BmPzY7kiUXapa0THauo71i0REm1bXRiQzCQ7X2eLCkvW_gE5ULGSvU53U0ThXbxF2FSj_sPx5ZphqNRbF7k_JLoLqp1s4WfQ.BNgdiGbY6-GoYRFwPgbY7w/__results___files/__results___14_130.png)

![alt.text](https://www.kaggleusercontent.com/kf/89961255/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..D_4fY6wnJdTvTMmHLQHjuw.b2zD69JODzk9bMA3LtXDAvFj-C7HOcfECVcrMAyYLQMXza3i2SIulUSHogJRf5PY4_Co_SD1OLSClGl7Yw9Eg6-qfvDspZ4kLskdj-4dBuFUBRAVuNkHOFsbukc0vGAUfUnW1mmhdm-nW2QG9niyGySZMLQj5tqD4v6GjKG-gV6ucTkEgUgZ9g3n5vN2c7TIMcXgs0tGCKJENfEnBRaSaQTRy0oGd2_vElo74PJ8y05ZkTOIf_kvrCtyGe1yX1eL6flncNDPrTSpCQm8PcCKp4gZ9XZpSsl98ttPNpRV2M6EHm8IaDnY1xIevAHKZiz9OsQg4oG-wmo5Yks0SAj16tKCtrW541TAmbcSlW8Rv3x2MLKf62VSut0TAkJvZxgTkjanDHxZ3Wv3O9KRbBeNjePy3fjczPimVa8oJs-fmL9ifQ_Mnpf55gUvvYuU4axb65f8J0SkOBePEox1R6jQ4NsEvVpxLUxATYqozNZS40tgGtI6VxeIZCmz33_rCpVu76WG7XR29EdHlMDbaR7HggPUI5pR_e-_fP4mnGbfp9nAmRlSA1P8H4BmPzY7kiUXapa0THauo71i0REm1bXRiQzCQ7X2eLCkvW_gE5ULGSvU53U0ThXbxF2FSj_sPx5ZphqNRbF7k_JLoLqp1s4WfQ.BNgdiGbY6-GoYRFwPgbY7w/__results___files/__results___14_163.png)

## Testing:
My model scored around 98% in the testing dataset. Some of the predictions of the test dataset are given below

![alt.text](https://www.kaggleusercontent.com/kf/89974404/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..12FSbNqBxX74S_yDbuqpFw.dfvB_G1SZ7Fc1sswYYwMEtJZ9CcAX0RsWbMzMCvODJJp1PKtvcaN-5zkgnvSL_pADVgJ_WCLzGG747uxMUir0VQeEa4LHxbkGVGJIsYOSg2aVmPYsXqjZwG9GBleRN9vbBASuO9h4axY5Pz8OL-0-juko94NPw0MLrpBQU_VIe2axRN6eA-opeLF19jOiyVA_BorxWI_j_eEg7HQAzNJkY1qmjoJWcgRfi_9zevyNfJXIONwznWrrMRQYdQj_q7Pf6h9u5_e0tDerAwqzjnashB_xX1DpG9WIUBu1ryGLYg_4UMsHoT7Q17HNthHLH2I8ZX3naERqJCEFJm4wxJ22Ir4Y2KDR_MGjW-sE9f-bu4yr13D8ZFJVHCa-idsSbOGxMiauW1ZPxoYbayDWY36peFxFwNsA3KmdkXoGqu25Y72C7UtTCGyJsehQm6pZCsOC_zFafiu_v3FtOP7UfaogG0ovFHSAD-_BT6A0NGneudtRquye9VH6KGMsh_6jObbHiqe6L0boTFc-7tMtTxGR06tfksvb3EFRRmPCloRzIDvuzuFWS7jVo-4MyREOZEyh3pnsINOYdFJ8kieMWt7mIyURFFylWU0CaWpwbPXDaPV93AbefGrsJN2MzZ52JG3-wmalgH7RQc9pwpn9c3_YKza0cQDIbOEKwOMP3d4g8jfK71J2xjImqRn2k8cOrjiuwIJxp2AQtRQJUvJh9yUMw.hGi04uyPRrD_QcQPeNX6ZQ/__results___files/__results___10_0.png)
