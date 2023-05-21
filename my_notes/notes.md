## When to use fit_transform and transform?
https://stackoverflow.com/questions/62920350/when-to-use-fit-transform-and-transform

fit_transform() is a method that combines the functionality of fit() and transform() methods. fit() is used to learn about the required aspects of the supplied data and returns the new object with the learned parameters. It does not change the supplied data in any waytransform() is used to actually transform the supplied data to the new form12.

For example, when using an imputer to fill missing values in your training data using the median, first you need to calculate what that median value is, this is what happens when you call fit(). Now you have the median value but you haven’t altered your dataset, to do that you need to change (or transform) your dataset. This is what happens when you call transform(). Often you want to calculate a median value and use that median value to replace NaNs or some other non-value, fit_transform() does both of these steps in one go for convenience1

## notes for azure installation
https://github.com/josepholaide/MLOps-Practice/blob/main/Week%201/README.md 

I am following this course with my private CentOS server...