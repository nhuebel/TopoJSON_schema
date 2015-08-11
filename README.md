This is a JSON schema representing the TopoJSON specification as described [here](https://github.com/mbostock/topojson-specification/blob/master/README.md).

It has been tested with the following online validators
* http://www.jsonschemavalidator.net/
* http://json-schema-validator.herokuapp.com/index.jsp
and the TopoJSON files in the test subfolder and the ones found at found at https://github.com/mbostock/topojson/tree/master/examples.


=Notes=
* Scale and translate in the transform of a topology object are fixed to two-element arrays of numbers according to the specification. However, in my opinion the dimension needs to coorespont with the dimension of the used geometry objects.
* This implementation allows to skip the Topology object and to start with a Geometry object.

=Issues=
* The validity of the inices in the arcs are not checked. Needs to be done programatically.
* The coherence of dimenstions of all objects are not checked. Needs to be handled programatically.