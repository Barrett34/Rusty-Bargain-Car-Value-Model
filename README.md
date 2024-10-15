# Rusty-Bargain-Car-Value-Model
Rusty Bargain has made a new app to attract new customers that will determine the market value for your vehicle. 

## Introduction

Rusty Bargain used car sales service is developing an app to attract new customers. In that app, you can quickly find out the market value of your car. We need to build the model to determine the value. 

Rusty Bargain is interested in:

- the quality of the prediction
- the speed of the prediction
- the time required for training

## Data Description

Features

- DateCrawled — date profile was downloaded from the database
- VehicleType — vehicle body type
- RegistrationYear — vehicle registration year
- Gearbox — gearbox type
- Power — power (hp)
- Model — vehicle model
- Mileage — mileage (measured in km due to dataset's regional specifics)
- RegistrationMonth — vehicle registration month
- FuelType — fuel type
- Brand — vehicle brand
- NotRepaired — vehicle repaired or not
- DateCreated — date of profile creation
- NumberOfPictures — number of vehicle pictures
- PostalCode — postal code of profile owner (user)
- LastSeen — date of the last activity of the user

Target

- Price — price (Euro)

## Conclusion

The project was started with data exploration and removing duplicates, missing value rows of data and determining what data to use for features to find the target, price of the vehicle. We droppped missing values because the features were any column that represented any sort of variable that would affect the price. Duplicates were dropped since the model didn't recognize the same vehicle with the same features. The features and target were then explored with graphical representations including bar charts, and pie charts that displayed their distributions.

We used Linear Regression, Random Forest, Gradient Boosting Regression, LightGBM, and Cat Boot Regressor models were used for validaiton. After training, LightGBM had the lowest RMSE with a 2.85 second training time and less than 1 second prediction time. The model showed high quality results with short time to train.
