import java.util.Scanner;

// Base class
class Cylinder {
    protected double radius;
    protected double height;

    // Initialise height and radius using the constructor
    public Cylinder(double radius, double height) {
        this.radius = radius;
        this.height = height;
    }
}

// Derived class
class CylinderVol extends Cylinder {

    // Using the base class constructor, the constructor initialises height and radius.
    public CylinderVol(double radius, double height) {
        super(radius, height);
    }

    // Method to calculate the volume of the cylinder
    public double getVolume() {
        return Math.PI * radius * radius * height;
    }

    // Method to calculate the surface area of the cylinder
    public double getArea() {
        return 2 * Math.PI * radius * (radius + height);
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Obtain the user's input for radius and height
        System.out.print("Enter the radius of the cylinder: ");
        double radius = scanner.nextDouble();
        System.out.print("Enter the height of the cylinder: ");
        double height = scanner.nextDouble();

        // Create an instance of CylinderVol
        CylinderVol cylinder = new CylinderVol(radius, height);

        // Calculate and display the volume and surface area
        System.out.println("Volume: " + cylinder.getVolume());
        System.out.println("Surface Area: " + cylinder.getArea());
        
        // Close the scanner
        scanner.close();
    }
}