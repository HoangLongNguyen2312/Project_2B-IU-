# Project_2B-IU-
## Brief introduction about our group project
A syringe pump is a precision motorized device designed to control the movement of fluid in and out of a syringe with high accuracy. The primary mechanism involves a stepper motor that moves a platform attached to the syringe plunger. As the motor rotates, it either pushes or pulls the plunger to deliver or withdraw liquid from the syringe. Meanwhile, the body of the syringe is held firmly in place, ensuring that all movement is confined to the plunger’s action.
These devices are widely used in scientific and medical applications, where precise control of fluid delivery is critical. Basic syringe pumps allow for the infusion (and in some cases, withdrawal) of liquids at a consistent, set rate by adjusting the motor speed.
The ease of control, coupled with their accuracy, makes syringe pumps ideal for tasks that require steady, repeatable delivery of fluids, such as drug infusion, chemical reactions, or even lab-scale experiments in a controlled environment. 

## Block Diagram about our project
```mermaid
flowchart LR
    A[V(in) 12 VDC] --> B[3A Buck Converter Circuit]
    B --> C[5V]
    C --> D[ESP 32]
    B --> E[Buttons]
    B --> F[LCD SCL/ SDA]
    B --> G[Stepper Driver]
    A --> G
    G --> H[Stepper]

