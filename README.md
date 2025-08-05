# BMI-Health-Risk-Calculator---python-project
BMI &amp; Health Risk Calculator - python project

This is a simple Python project that calculates **Body Mass Index (BMI)** based on user input for height and weight. It then classifies the BMI result into different health risk categories.

## What is BMI?

BMI (Body Mass Index) is a measure of body fat based on height and weight that applies to adult men and women. It helps to assess whether a person is underweight, healthy, overweight, or obese.

## Features

- Interactive user input (no parameters required).
- Height is taken in **centimeters**, weight in **kilograms**.
- Calculates BMI and gives an appropriate **health risk category**.

## BMI Categories

| BMI Range (kg/m²) | Health Category                 |
|-------------------|----------------------------------|
| < 18.5            | Possible nutritional deficiency  |
| 18.5 – 24.9       | Low health risk                  |
| 25 – 29.9         | Increased health risk            |
| ≥ 30              | Very high health risk (Obese)    |

## Python code
def bmi_calculator_function_with_input():
    height_cm=float(input("Enter height_cm here: "))
    weight_kg=float(input("Enter weight_kg here: "))
    height_m=height_cm/100
    bmi=weight_kg/(height_m**2)
    if bmi>=30:
        print(f"Your BMI is {bmi:.2f} and Health Risk is very high")
    elif bmi >=25 and bmi <=29.9:
        print(f"Your BMI is {bmi:.2f} and Health risk increased")
    elif bmi >= 18.5 and bmi <=24.9:
        print(f"Your BMI is {bmi:.2f} and Low health risk")
    else:
        print("Possible nutritional deficiency")

#let's call the function
bmi_calculator_function_with_input()
