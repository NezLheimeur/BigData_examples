# BigData_exemples

## A/ Spark ML : Iris classification

**_Data : iris.csv_**

The notebook **iris_ml_spark.ipynb** script, present a Spark Pipeline that transform and process the data before applying differnet classification model:
- Decision tree Classifier; 
- The Random Forest Classifier ;
- LogisticRegression Classifier.
Then Compare their performance

## B/ Spark : parallelisation of the image processing algorithm « MedianFilter »

The median filter consists in replace the value of a pixel _p[i,j]_ by the median value of the list :
_[p[i-1,j-1],p[i-1,j],p[i-1,j+1],p[i,j-1],p[i,j],p[i,j+1],p[i+1,j-1],p[i+1,j],p[i+1,j+1]]_

The notebook **median_filter_spark.ipynb** present a parallisation of this filter using **spark**.

The script is executed on the **lena_noizy.jpg** image and generate the new file **lena_filter.jpg**

## C/ Dask ML : flower classification

**_Data : flower_images.zip_**

the notebook **iris_ml_spark.ipynb**  use Dask to apply to apply a pipeline on different images before segmenting them. 
The following pipeline is:
- convert to gray scale
- apply segmentation
- get num of labels
Then plot hystogram of numbers of labels.

## D/ Dask : parallelisation of the image processing algorithm « MedianFilter »


The notebook **median_filter_dask.ipynb** present a parallisation of the  Median filter presented above using **dask**.

The script is executed on the **lena_noizy.jpg** image and generate the new file **lena_filter.jpg**
