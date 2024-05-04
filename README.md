#include <stdio.h>

// Function to calculate and display BMI
void BMI(int, float);

int main(void) {
int w; // Variable to store weight
float h; // Variable to store height

    // Prompt user for weight and height
printf("Input the weight: ");
scanf("%d", &w);
printf("Input the height: ");
scanf("%f", &h);

    // Call the BMI function with provided weight and height
BMI(w, h);
}
/// Function to calculate and display BMI
void BMI(int weight, float height) {
    // Calculate BMI using the provided formula
float temp = weight / (height * height);

    // Display the calculated BMI
printf("BMI = %f\n", temp);
printf("\nGrade: ");

    // Determine BMI grade and display it
temp< 18.5 ? printf("Under ") : temp < 25 ? printf("Normal ") : temp < 30 ? printf("Over ") : temp < 40 ? printf("Obese ") : printf("Error");
}

