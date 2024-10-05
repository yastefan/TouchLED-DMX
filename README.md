# TouchLED - A TouchDesigner LED and DMX Library

TouchLED is a library to simplify the control of LEDs and DMX fixtures in TouchDesigner and to provide a consistent workflow. A visualiser enables the creation of complex mappings without additional hardware or software.
For all those who are not yet familiar with TouchDesigner: You get a professional (for non-commercial purposes) free LED mapping solution with endless creative possibilities.

## Concept

LEDs or fixtures are arranged in SOPs in 3D space. Each individual point simbolises a pixel or DMX parameter. The SOP input is displayed on a selectable plane in order to display video content (TOPs) on the LEDs/fixtures. 

A minimal setup consists of an SOP, the **Mapper** component and the **DMX_Universe** component. The SOP specifies the shape and position of the LEDs, the mapper places a video on the LEDs and the DMX_Universe sends the data to the LEDs or fixtures. In this example, the SOP is a straight line with 10 points, e.g. a WS2812 LED strip with 10 LEDs. The **Mapper** maps a color gradient to the LEDs via the TOP input and the DMX universe components send the data to the controller of the LED strips via sACN. 

![simple_example](https://github.com/yastefan/TouchLED-DMX/blob/main/Assets/simple.jpg)

In the following example, there are three LED strips with 10 LEDs each arranged as a triangle and a circle with 40 LEDs. The **Visualizer** components are also used here to simulate the behaviour of the LED strips.

![simple2_example](https://github.com/yastefan/TouchLED-DMX/blob/main/Assets/simple2.jpg)
