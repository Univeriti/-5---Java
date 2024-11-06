public class CalculateXY {
    public static void main(String[] args) {
        // Given constants
        double a = 1.256;
        double b = 3.5;
        double c = 0.53;
        double z = 7;

        // Calculate x using the formula: x = a * Math.exp(-b * a) * Math.cos(c) + z
        double x = a * Math.exp(-b * a) * Math.cos(c) + z;
        
        // Calculate y using the formula: y = (Math.pow(a, 2) + 5 * a + 6) / (Math.pow(a, 2) + 1)
        double y = (Math.pow(a, 2) + 5 * a + 6) / (Math.pow(a, 2) + 1);

        // Output the results
        System.out.printf("Calculated x: %.4f\n", x);
        System.out.printf("Calculated y: %.4f\n", y);
    }
}
import math

# Function definition
def f(x, a, b):
    if x < 3:
        return math.sqrt(5 * x**2 - a)
    elif x == 3:
        return b * x + 8
    elif 3 < x < 11:
        return math.cos(x)
    else:
        return "x is out of the defined range"

# Input values for a and b from the user
a = float(input("Enter the value of a: "))
b = float(input("Enter the value of b: "))

# Input value for x from the user
x = float(input("Enter the value of x: "))

# Calculate and display the result
result = f(x, a, b)
print("f(x) =", result)
