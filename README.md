# Tamil Nadu Wetland Encroachment Potential
**Google Earth Engine App**

GEE App link : https://balakumaran247.users.earthengine.app/view/tnwetlandencroachpotential

Mapping the possibility of wetlands being encroached in the future is presented in this Google Earth Engine App.
Under the hood this application calculates the encroachment potential by classification of Sentinel-2 datasets using Gradient Tree Boost Classifier.

The Wetland Boundary layer mapped for the period 2017-2018 at 1:50,000 scale for the entire Tamil Nadu state is used in this application.

The location of the points (wetland, non-wetland and bad pixels) for training the model was created with advice from experts and from interpreting UAV drone images.

Gradient Tree Boost model was selected from several other model choices based on the accuracy obtained and further hyperparameter tuning was carried out as a means of maximizing the predictive performance.
Finalising the model with 100 trees, shrinkage parameter of 0.005, sampling rate of 0.7 and LeastAbsoluteDeviation as loss function. Overall accuracy of the model is 86.9% and kappa coefficient of 0.78.

---

![GEE App Welcome Screen](/resources/GEE_app_screen.jpg)

![Encroachment Potential Map Screen](/resources/encroachment_potential_map.jpg)