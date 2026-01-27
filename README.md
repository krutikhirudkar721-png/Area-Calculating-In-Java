# Area-Calculating-In-Java
# Write a Program using class Rectangle and calculate area using (method)

       import java.util.Scanner;

    public class MyProgram {
        public static void main(String[] args) {
            try (Scanner sc = new Scanner(System.in)) {
                Rectangle r1 = new Rectangle();
                System.out.print("Enter height: ");
                r1.setHeight(sc.nextFloat());
                System.out.print("Enter width: ");
                r1.setWidth(sc.nextFloat());
                r1.displayArea();
            } catch (Exception e) {
                System.err.println("Error reading input: " + e.getMessage());
            }
        }
    }
        class Rectangle {
            private float height;
            private float width;
            public void setHeight(float height) {
                this.height = height;
            }
            public void setWidth(float width) {
                this.width = width;
            }
            public void displayArea() {
                float area = height * width;
                  System.out.println("Area = " + area);
             }
        }

