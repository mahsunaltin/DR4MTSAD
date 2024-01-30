# DR4MTSAD (Exploring the Influence of Dimensionality Reduction on Anomaly Detection Performance in Multivariate Time Series) 🚀

## Overview 👀
This repository contains the implementation and analysis of two advanced unsupervised anomaly detection models - MUTANT and Anomaly-Transformer - applied to time series data. The focus of this project is on integrating dimensionality reduction techniques to enhance the performance and efficiency of these models.


## Results 🔥

<table style="border-collapse: collapse; border: none; border-spacing: 0px;">
	<caption>
		<b>Results:</b> Extensive Performance Comparison of MUTANT and Anomaly-Transformer Models Under Various Dimensionality Reduction Techniques Across MSL, SMAP and SWaT Datasets
	</caption>
	<tr>
		<td rowspan="2" style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>Model</b>
		</td>
		<td rowspan="2" style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b># Dimensions</b>
			<br>
			<b>Remaining</b>
		</td>
		<td rowspan="2" style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>DR Layer</b>
			<br>
			<b>(Technique)</b>
		</td>
		<td colspan="3" style="border-bottom: 0px solid rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>MSL</b>
		</td>
		<td colspan="3" style="border-bottom: 0px solid rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>SMAP</b>
		</td>
		<td colspan="3" style="border-bottom: 0px solid rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>SWaT</b>
		</td>
	</tr>
	<tr>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>Precision</b>
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>Recall</b>
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>F1-score</b>
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>Precision</b>
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>Recall</b>
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>F1-score</b>
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>Precision</b>
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>Recall</b>
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>F1-score</b>
		</td>
	</tr>
	<tr>
		<td rowspan="7" style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			MUTANT
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			(Original)
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			None
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9464</b>
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9520
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9492
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9658
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9787
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9722
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9805
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9881
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9842
		</td>
	</tr>
	<tr>
		<td rowspan="3" style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			To Half Dim.
			<br>
			27 - 12 - 25
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			PCA
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9307
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9807
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9551
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9725
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9630
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9678
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9729
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>1.0000</b>
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9863</b>
		</td>
	</tr>
	<tr>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Rand. Proj.
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.8619
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>1.0000</b>
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9258
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9703
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9782
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9742
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9782
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9882
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9832
		</td>
	</tr>
	<tr>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			UMAP
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.8846
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9762
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9281
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9836
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9453
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9640
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9491
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9838
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9661
		</td>
	</tr>
	<tr>
		<td rowspan="3" style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			To Lowest Dim.
			<br>
			8 - 8 - 8
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			PCA
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9184
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9848
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9505
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9882
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9659
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9769</b>
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9632
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9866
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9748
		</td>
	</tr>
	<tr>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Rand. Proj.
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9331
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9762
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9542
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9550
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9866</b>
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9706
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9728
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9856
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9792
		</td>
	</tr>
	<tr>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			UMAP
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9341
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9914
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9619</b>
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9913</b>
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9399
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9649
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9833</b>
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9788
		</td>
		<td style="border-bottom: 2px double black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9810
		</td>
	</tr>
	<tr>
		<td rowspan="12" style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Anomaly-Transformer
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			(Original)
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			None
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9188
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9473
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9329
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9381
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9939
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9652
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.8844
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>1.0000</b>
		</td>
		<td style="border-bottom: 1px solid black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9386
		</td>
	</tr>
	<tr>
		<td rowspan="3" style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			To Half Dim.
			<br>
			27 - 12 - 25
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			PCA
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9146
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9436
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9289
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9111
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9916
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9497
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9223
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>1.0000</b>
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9596
		</td>
	</tr>
	<tr>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Rand. Proj.
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9191
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9773
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9473
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9160
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9950
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9539
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.8889
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>1.0000</b>
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9412
		</td>
	</tr>
	<tr>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			UMAP
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9178
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9735
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9448
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9264
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9993</b>
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9615
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.8482
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>1.0000</b>
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9179
		</td>
	</tr>
	<tr>
		<td rowspan="4" style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			3 - 3 - 3
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			PCA
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9172
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9676
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9417
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9072
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9945
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9489
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9706
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9495
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9600</b>
		</td>
	</tr>
	<tr>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Rand. Proj.
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9180
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9793</b>
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9477</b>
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9335
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9919
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9618
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9891</b>
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.8619
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9212
		</td>
	</tr>
	<tr>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			UMAP
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9171
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9560
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9361
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9320
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9915
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9608
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9807
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9229
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9509
		</td>
	</tr>
	<tr>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			t-SNE
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9164
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9490
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9324
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9310
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9962
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9625
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9843
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9082
		</td>
		<td style="border-bottom: 1px dotted black; text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9447
		</td>
	</tr>
	<tr>
		<td rowspan="4" style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			To Lowest Dim.
			<br>
			2 - 2 - 2
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			PCA
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9180
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9683
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9425
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9070
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9930
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9481
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9492
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9696
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9593
		</td>
	</tr>
	<tr>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Rand. Proj.
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9210</b>
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9473
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9340
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9429</b>
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9524
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9476
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9876
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.8862
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9341
		</td>
	</tr>
	<tr>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			UMAP
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9183
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9677
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9423
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9330
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9945
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9628
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9890
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.8871
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9352
		</td>
	</tr>
	<tr>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			t-SNE
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9197
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9749
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9465
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9353
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9977
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>0.9655</b>
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9854
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9237
		</td>
		<td style="text-align: center; padding-right: 3pt; padding-left: 3pt;">
			0.9536
		</td>
	</tr>
</table>


### Models 💾
- **MUTANT**: Leveraging Graph Convolutional Networks (GCNs) and attention-based Variational Auto-Encoders (VAEs).
- **Anomaly-Transformer**: Utilizing association discrepancies for anomaly identification.

### Dimensionality Reduction Techniques 🔄
- PCA (Principal Component Analysis)
- UMAP (Uniform Manifold Approximation and Projection)
- t-SNE (t-Distributed Stochastic Neighbor Embedding)
- Random Projection

## Notebooks 📓
- `Anomaly_Transformer.ipynb`: Training and testing the Anomaly-Transformer model. 
- `MUTANT.ipynb`: Training and testing the MUTANT model.
- `ApplyDimensionalityReduction.ipynb`: Application of various dimensionality reduction techniques to the datasets.

## Data 📊
The `data` directory contains the following datasets used for empirical analysis:
- **MSL**: Mars Science Laboratory Rover dataset.
- **SMAP**: Soil Moisture Active Passive Satellite dataset.
- **SWaT**: Secure Water Treatment dataset.

## Results 📈
- `Results.md`: A detailed markdown file containing the results and findings of the model training and testing.

## How to Use 🔧
Each Jupyter Notebook is self-contained and includes the necessary code for model training, testing, and applying dimensionality reduction techniques. Follow the steps in each notebook to replicate the experiments.

### Important Note 🗒️

While running the Anomaly-Transformer model, please change the file `Anomaly-Transformer/data_factory/data_loader.py`.

## Key Findings 💡
- Significant enhancement in anomaly detection performance with dimensionality reduction.
- Notable reduction in training times, especially when data is reduced to its lowest dimensions.
- Both MUTANT and Anomaly-Transformer models show adaptability and robustness across various datasets and dimensionality reduction scenarios.

## Contributing 🤝
Contributions to this project are welcome! Please refer to the issues tab for pending enhancements and bug fixes.

## Citation 📖
If you use this work in your research, please cite:

"Exploring the Influence of Dimensionality Reduction on Anomaly Detection Performance in Multivariate Time Series"

## Related Repos 📂

https://github.com/mahsunaltin/3DMesh 

## License 📄
This project is licensed under the terms of the MIT license.
