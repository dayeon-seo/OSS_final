# OSS_final 
> 20220051 Dayeon Seo

### Brain Tumor MRI Classification
> This program is designed to classifing brain tumor MRI images.

### About program

##### Training Dataset
* Data sets: Glioma_tumor, Meningioma_tumor, No_tumor, Pituitary_tumor

##### Used Algorithms
* K-Neighbors
* Min-Max Scaling

##### Hyperparameter
<pre>
<code>

clf = KNeighborsClassifier(n_neighbors=1,p=2,weights='distance')

</code>
</pre>

##### Min-Max SCaling
<pre>
<code>

min_on_training=X_train.min(axis=0)
max_on_training=X_train.max(axis=0)
range_on_training=(X_train - min_on_training).max(axis=0)
X_train_scaled=(X_train - min_on_training)/range_on_training

</code>
</pre>
