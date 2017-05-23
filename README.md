# canvas-in-svg

The visualization demonstrates the use of an embedded Canvas in an SVG element. While this example includes only a single SVG element, an embedded canvas may make sense when a number of SVG elements needs to be generated, with each requiring to render large datasets that would othwewise overwhelm the DOM. 

In this example, up to 50,000 elements can be generated and visualized in the embedded canvas with no impact to the DOM (other than creating the canvas). Mouse hit detection of data elements is performed with a 4x4 pixel zone under the current mouse position. While the example is admittedly a bit of a Rube Goldberg kind of project, it nevertheless attempts to demonstrate the following concepts:

- Creation of an embedded canvas
- Generation of normally distributed numbers
- Generation of correlated sets of numbers
- Computation of correlation coefficient
- Drawing of large number of data points in the canvas, while controlling opacity
- Mouse data point hit detection in the canvas (even at 50K elements on the canvas)
- D3 scales, axes, element creation, event handling and update pattern
- Dynamic reconfiguration of a D3 axis
- Usage of HTLM5 elements such as radio button, range and checkbox
