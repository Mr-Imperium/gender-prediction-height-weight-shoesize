# gender-prediction-height-weight-shoesize
Gender Prediction from Height, Weight, and Shoe Size

## Project Description
This project demonstrates how to use machine learning to predict the gender of a person based on their height, weight, and shoe size. The code reads in a CSV file containing this data, trains several different classification models, and then evaluates their performance on a test set. The best-performing model is then used to make predictions on new data.

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Data](#data)
4. [Models](#models)
5. [Results](#results)
6. [Contributing](#contributing)
7. [License](#license)

## Installation
To run this project, you'll need to have the following Python libraries installed:
- pandas
- scikit-learn

You can install these libraries using pip:

```
pip install pandas scikit-learn
```

## Usage
To use the gender prediction model, follow these steps:

1. Save the CSV file containing the height, weight, shoe size, and gender data in the same directory as the Python script.
2. Update the `'height_weight_shoesize_gender.csv'` file name in the script to match the name of your CSV file.
3. Run the Python script. This will train the models, evaluate their performance, and provide an example of how to use the best-performing model to make a prediction on a new person's data.

```python
# Example usage
new_person = [[170, 75, 42]]  # height, weight, shoe size
predicted_gender = models['Gradient Boosting'].predict(new_person)[0]
print(f"Predicted gender: {predicted_gender}")
```

## Data
The project uses a CSV file that contains the following columns:
- `Hight`: the height of the person in centimeters
- `Weight`: the weight of the person in kilograms
- `Shoe size`: the shoe size of the person
- `Gender`: the gender of the person (either "male" or "female")

You will need to provide your own CSV file with this data for the project to work.

## Models
The project tries several different machine learning models to predict the gender of a person:
- Random Forest Classifier
- Gradient Boosting Classifier
- AdaBoost Classifier
- Logistic Regression

The performance of each model is evaluated using both accuracy and F1-score, and the best-performing model (Gradient Boosting Classifier) is used for making predictions on new data.

## Results
Best results obtained were by Logistic Regression that gave an accuracy of 0.77, f1-score of 0.78.

This means that the Gradient Boosting Classifier was able to predict the gender with 77% accuracy on the test set.

## Contributing
If you find any issues or have suggestions for improving the project, please feel free to open a new issue or submit a pull request on the project's GitHub repository.

## License
This project is licensed under the [MIT License](LICENSE).
