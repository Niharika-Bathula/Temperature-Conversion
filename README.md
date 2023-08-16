# Temperature-Conversion
def celsius_to_fahrenheit(celsius):
    return (celsius * 9/5) + 32

def fahrenheit_to_celsius(fahrenheit):
    return (fahrenheit - 32) * 5/9

scale = input("Enter the scale (C/F): ")
temperature = float(input("Enter the temperature: "))

if scale.upper() == "C":
    converted_temperature = celsius_to_fahrenheit(temperature)
    print("Converted temperature in Fahrenheit:", converted_temperature)
elif scale.upper() == "F":
    converted_temperature = fahrenheit_to_celsius(temperature)
    print("Converted temperature in Celsius:", converted_temperature)
else:
    print("Invalid scale. Please enter 'C' or 'F'.")
