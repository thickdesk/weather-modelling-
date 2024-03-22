# Step 1: Hard-coding Variables for Weather Modeling

def temperature_modeling(a, b, c, time):
    """
    Function to model temperature using a quadratic equation.
    
    Parameters:
        a (float): Coefficient a.
        b (float): Coefficient b.
        c (float): Coefficient c.
        time (float): Time in hours.
    
    Returns:
        float: Calculated temperature.
    """
    # Calculate temperature based on time using the quadratic equation
    temperature = a * time**2 + b * time + c
    return temperature

# Hand-coded coefficients for temperature modeling
a_hardcoded, b_hardcoded, c_hardcoded = 0.1, 2, 30

# Display results
print("Step 1: Hard-coded Variables for Weather Modeling")
time_hardcoded = 6  # Example time value
print("Temperature for hardcoded coefficients at time", time_hardcoded, ": ", temperature_modeling(a_hardcoded, b_hardcoded, c_hardcoded, time_hardcoded), "\n")

# Step 2: Keyboard Input for Weather Modeling

# Set coefficients from user input
a_keyboard = float(input("Enter coefficient a: "))
b_keyboard = float(input("Enter coefficient b: "))
c_keyboard = float(input("Enter coefficient c: "))

# Get time from user input
time_keyboard = float(input("Enter time in hours: "))

# Calculate temperature using user-input coefficients and time
temperature_keyboard = temperature_modeling(a_keyboard, b_keyboard, c_keyboard, time_keyboard)

# Display temperature calculated from user-input coefficients and time
print("Temperature for user-input coefficients at time", time_keyboard, ": ", temperature_keyboard)

# Step 3: File Input for Weather Modeling

def read_coefficients_from_file(filename):
    """
    Function to read coefficients from a file.
    
    Parameters:
        filename (str): Name of the file containing coefficients.
    
    Returns:
        tuple: Coefficients (a, b, c) read from the file.
    """
    with open(filename, 'r') as file:
        coefficients = [float(x) for x in file.readline().split()]
    return tuple(coefficients)

filename = "coefficients.txt"
a_file, b_file, c_file = read_coefficients_from_file(filename)

# Get time from user input
time_file = float(input("Enter time in hours: "))

# Calculate temperature using coefficients from the file and user-input time
temperature_file = temperature_modeling(a_file, b_file, c_file, time_file)

# Display temperature calculated from coefficients in the file and user-input time
print("Temperature for coefficients from file at time", time_file, ": ", temperature_file)

# Step 4: File Output for Weather Modeling

def write_temperature_to_file(filename, time, temperature):
    """
    Function to write temperature to a file.
    
    Parameters:
        filename (str): Name of the file to write temperature to.
        time (float): Time for which temperature is calculated.
        temperature (float): Calculated temperature.
    """
    with open(filename, 'w') as file:
        file.write(f"Time: {time} hours\nTemperature: {temperature}")

output_filename = "temperature_output.txt"
write_temperature_to_file(output_filename, time_file, temperature_file)
print("Temperature written to", output_filename)
