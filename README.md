# Area-Calculating-In-Java
# WAP using class Rectangle and calculate area using method

    import java.util.Scanner;

    /**
     * Main class to handle user input and rectangle calculations.
     */
    public class MyProgram {
    public static void main(String[] args) {
        // Use try-with-resources to ensure the Scanner closes automatically
        try (Scanner sc = new Scanner(System.in)) {
            Rectangle r1 = new Rectangle();

            System.out.print("Enter height: ");
            r1.setHeight(sc.nextFloat());

            System.out.print("Enter width: ");
            r1.setWidth(sc.nextFloat());

            // Display the area
            r1.displayArea();
        } catch (Exception e) {
            System.err.println("Error reading input: " + e.getMessage());
        }
    }
}

    /**
     * Rectangle class representing the geometric shape.
     */
    class Rectangle {
    private float height;
    private float width;

    // Setters to follow encapsulation principles
    public void setHeight(float height) {
        this.height = height;
    }

    public void setWidth(float width) {
        this.width = width;
    }

    /**
     * Calculates and prints the area to the console.
     */
    public void displayArea() {
        float area = height * width;
        System.out.println("Area = " + area);
    }
}
