# ACCESS-NRI Model Scaling Repository

## About

The [ACCESS-NRI Model Scaling Repository](https://github.com/ACCESS-NRI/access-model-scaling/) is a collection of Jupyter Notebooks that generate and display scaling data for ACCESS-NRI models.

We expect this data to be useful to both users and developers. It can be used to guide decisions about parallelisation layouts and CPU core counts when developing model configurations in order to ensure good balance between performance and parallel efficiency. It can also help identifying areas where codes can be improved and optimised. Finally, the provided plots and tables that can be used in NCMAS applications and other similar merit allocation schemes when requesting HPC resources.

Currently the repository includes scaling data for the following models:

* [ACCESS-ESM1.6](https://github.com/ACCESS-NRI/access-model-scaling/blob/main/ESM1p6-scaling.ipynb) 
* [ACCESS-rAM3](https://github.com/ACCESS-NRI/access-model-scaling/blob/main/ram3.ipynb)
* [ACCESS-OM3 Global 25km](https://github.com/ACCESS-NRI/access-model-scaling/blob/main/accessom3_global_25km.ipynb)
* [ACCESS-OM3 Pan-Antarctic 4km](https://github.com/ACCESS-NRI/access-model-scaling/blob/main/accessom3_panan_4km.ipynb)

We expect to regularly add new models to this list and update the existing notebooks when new versions of the models are available.

## What is not included in these notebooks

The notebooks do not include any type of resource usage estimate, like SUs per model year, as this information can strongly depend on the actual configuration being used. For ACCESS-NRI configurations, this information can sometimes be found in the [release notes](https://forum.access-hive.org.au/search?q=tags%253Amodel%20%2523access-nri-releases%20order%253Alatest). If this information is not available, or you do not know how to obtain it, we suggest opening a [new help request](https://forum.access-hive.org.au/new-topic?&body=%3Cdiv%20data-theme-toc%253D%22true%22%3E%3C%252Fdiv%3E%0A%0A%3C!--%20These%20are%20comments%20and%20not%20visible%20once%20you%20post.%20Ignore%20or%20delete%20sections%20if%20not%20relevant%20--%3E%0A%0A%3C!--%20Choose%20an%20appropriate%20category.%20If%20not%20sure%252C%20leave%20as%20General%20--%3E%0A%0A%2523%2523%20Description%20of%20request%253A%0A%0A%2523%2523%20Environment%253A%0A%0A%3C!--%20NCI%253F%20ARE%253F%20Gadi%20login%20node%253F%20PBS%20job%253F%20--%3E%0A%0A%3C!--%20List%20software%20versions%20--%3E%0A%0A%2523%2523%20What%20executed%253A%0A%0A%3C!--%20Copy%20and%20paste%20any%20commands%20and%20output%20in%20a%20code%20block%20--%3E%0A%3C!--%20For%20code%20you%20are%20writing%252C%20prepare%20a%20minimal%20reproducible%20example%20(https%253A%252F%252Fforum.access-hive.org.au%252Fdocs%253Ftopic%253D843)%20--%3E%0A%0A%2523%2523%20Actual%20results%253A%0A%0A%3C!--%20Copy%20full%20error%20messages%20--%3E%0A%0A%2523%2523%20Expected%20results%253A%0A%0A%2523%2523%20Additional%20info%253A&category_id=4&tags=help) on the ACCESS-Hive Forum.

## Where do I ask questions?

We welcome feedback and contributions through the [ACCESS-Hive forum](https://forum.access-hive.org.au/). Please create a topic in the #technical category and [follow the guidelines for requesting help from ACCESS-NRI](https://forum.access-hive.org.au/t/access-help-and-support/908) should you need it. You can also open an issue [on Github](https://github.com/ACCESS-NRI/access-model-scaling/issues/new/).

## Running the notebooks

In case you are interested in running the notebooks, please follow [these instructions](docs/running_the_notebooks.md)].
