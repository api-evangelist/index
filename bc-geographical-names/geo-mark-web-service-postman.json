{
  "info": {
    "name": "Geo Mark Web Service Gets a single spatial point representative of the geomark.",
    "_postman_id": "f0c2a0ad-e539-42a0-b54b-a2c110f22ec6",
    "description": "The geomark point resource returns a single spatial feature with a single Point and the geomark attribution.  The point geometry will be created from the first geometry part of the Geomark. Point geomarks will return the first Point part in the geomark.  LineString geomarks will return the first coordinate of the first LineString part in the geomark. Polygon geomarks will return the centroid or another point inside the first Polygon part in the geomark. The geometry and attribution can be downloaded as a spatial download file format in a supported coordinate system. The download files can then be used in a desktop GIS application (e.g. ArcMap), Google Earth or a web mapping application.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Geomarks",
      "item": [
        {
          "id": "86a3ad78-8809-404a-aab3-636c55892820",
          "name": "the-source-geomarks-can-be-specified-by-with-the-geomarkurl-parameter---repeat-the-parameter-if-sour",
          "request": {
            "url": "http://apps.gov.bc.ca/pub/geomark/geomarks/copy?bufferCap=%7B%7D&bufferJoin=%7B%7D&bufferMetres=%7B%7D&bufferMitreLimit=%7B%7D&bufferSegments=%7B%7D&callback=%7B%7D&failureRedirectUrl=%7B%7D&geomarkUrl=%7B%7D&redirectUrl=%7B%7D&resultFormat=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The source geomarks can be specified by with the geomarkUrl parameter.  Repeat the parameter if sourcing from multiple geomarks"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15e807a4-4a93-48f4-b526-1ad01d094336"
            }
          ]
        },
        {
          "id": "2f1656f3-1f88-4557-8a32-caf902ac96d3",
          "name": "create-a-new-geomark-from-the-geometries-read-from-the-body-parameter-or-file-",
          "request": {
            "url": "http://apps.gov.bc.ca/pub/geomark/geomarks/new",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "body",
                  "value": "{}",
                  "disabled": false,
                  "description": "The binary or character content representing the geometry or geometries"
                },
                {
                  "key": "bufferCap",
                  "value": "{}",
                  "disabled": false,
                  "description": "If bufferMetres is specified, The style of buffer to use at the ends of a buffered line"
                },
                {
                  "key": "bufferJoin",
                  "value": "{}",
                  "disabled": false,
                  "description": "If bufferMetres is specified, The style of buffer to use for joins between the line segments for lines and polygons"
                },
                {
                  "key": "bufferMetres",
                  "value": "{}",
                  "disabled": false,
                  "description": "The amount to buffer the geometry in metres, must only contain numerical digits (e"
                },
                {
                  "key": "bufferMitreLimit",
                  "value": "{}",
                  "disabled": false,
                  "description": "If bufferMetres is specified, the maximum ratio of distance from the original geometry to a mitre buffer point and the buffer amount"
                },
                {
                  "key": "bufferSegments",
                  "value": "{}",
                  "disabled": false,
                  "description": "If bufferMetres is specified, the number of line segments used in each quadrant to approximate the curve for round end-cap and join styles"
                },
                {
                  "key": "callback",
                  "value": "{}",
                  "disabled": false,
                  "description": "The callback function a JSON result format would be wrapped in to support Ajax requests"
                },
                {
                  "key": "failureRedirectUrl",
                  "value": "{}",
                  "disabled": false,
                  "description": "The url to redirect if the geomark could not be created"
                },
                {
                  "key": "format",
                  "value": "{}",
                  "disabled": false,
                  "description": "The file format name extension of the input geometry"
                },
                {
                  "key": "multiple",
                  "value": "{}",
                  "disabled": false,
                  "description": "Boolean flag indicating if multiple geometries are to be used for the geomark (true) or only a single geometry from the first geometry (false)"
                },
                {
                  "key": "redirectUrl",
                  "value": "{}",
                  "disabled": false,
                  "description": "The optional external URL to redirect the user to when the geomark is created rather than showing the geomark info page"
                },
                {
                  "key": "resultFormat",
                  "value": "{}",
                  "disabled": false,
                  "description": "The file format the geomark info resource should be returned using"
                },
                {
                  "key": "srid",
                  "value": "{}",
                  "disabled": false,
                  "description": "The srid of the coordinate system the input geometries are in"
                }
              ]
            },
            "description": "Create a new geomark from the geometries read from the 'body' parameter or file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "025925b4-fc8e-4a83-945b-2433ebb7ca83"
            }
          ]
        },
        {
          "id": "bf86d271-7607-435c-9601-f4c77a828c42",
          "name": "the-attribution-can-be-downloaded-as-a-info-file-format--the-download-files-can-then-be-processed-by",
          "request": {
            "url": {
              "protocol": "http",
              "host": "apps.gov.bc.ca",
              "path": [
                "pub",
                "geomark",
                "geomarks/:geomarkId.:fileFormatExtension"
              ],
              "query": [
                {
                  "key": "srid",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "fileFormatExtension",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "geomarkId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The attribution can be downloaded as a info file format. The download files can then be processed by a client application to access the geomark info fields and to get the URLs to the geometry download resources."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db9d2824-d4b0-4d2a-9e48-294ee95bdd37"
            }
          ]
        },
        {
          "id": "f397939d-5b13-4e6c-8551-8d93ffa5fc08",
          "name": "the-source-geomarks-can-be-specified-by-with-the-geomarkurl-parameter---repeat-the-parameter-if-sour",
          "request": {
            "url": {
              "protocol": "http",
              "host": "apps.gov.bc.ca",
              "path": [
                "pub",
                "geomark",
                "geomarks/:geomarkId/boundingBox.:fileFormatExtension"
              ],
              "query": [
                {
                  "key": "srid",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "fileFormatExtension",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "geomarkId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The source geomarks can be specified by with the geomarkUrl parameter.  Repeat the parameter if sourcing from multiple geomarks"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc11161d-6985-4f63-8803-cc0c1cc5b5da"
            }
          ]
        },
        {
          "id": "da70f0e5-6c73-4945-800d-5ed719ae4186",
          "name": "the-geomark-feature-resource-returns-a-single-spatial-feature-with-either-a-single-point-linestring-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "apps.gov.bc.ca",
              "path": [
                "pub",
                "geomark",
                "geomarks/:geomarkId/feature.:fileFormatExtension"
              ],
              "query": [
                {
                  "key": "srid",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "fileFormatExtension",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "geomarkId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The geomark feature resource returns a single spatial feature with either a single (Point, LineString, Polygon) or multi-part geometry (MultiPoint, MultiLineString, MultiPolygon) and the geomark attribution.  The geometry and attribution can be downloaded as a spatial download file format in a supported coordinate system. The download files can then be used in a desktop GIS application (e.g. ArcMap), Google Earth or a web mapping application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2131e456-c9fb-45d6-b166-4d240bea5da6"
            }
          ]
        },
        {
          "id": "80323ed6-5310-49d4-b269-1ebbebb911a9",
          "name": "the-geomark-parts-resource-returns-a-one-or-more-spatial-features--one-for-each-part-of-the-geomarks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "apps.gov.bc.ca",
              "path": [
                "pub",
                "geomark",
                "geomarks/:geomarkId/parts.:fileFormatExtension"
              ],
              "query": [
                {
                  "key": "srid",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "fileFormatExtension",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "geomarkId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The geomark parts resource returns a one or more spatial features. One for each part of the Geomark's geomerty. Each part contains a single (Point, LineString, Polygon) geometry and the geomark attribution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42e12dab-5b6f-4f46-9ec5-b44d01d8c883"
            }
          ]
        },
        {
          "id": "0323d63d-0b18-431c-8402-7a9d45f7815e",
          "name": "the-geomark-point-resource-returns-a-single-spatial-feature-with-a-single-point-and-the-geomark-attr",
          "request": {
            "url": {
              "protocol": "http",
              "host": "apps.gov.bc.ca",
              "path": [
                "pub",
                "geomark",
                "geomarks/:geomarkId/point.:fileFormatExtension"
              ],
              "query": [
                {
                  "key": "srid",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "fileFormatExtension",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "geomarkId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The geomark point resource returns a single spatial feature with a single Point and the geomark attribution.  The point geometry will be created from the first geometry part of the Geomark. Point geomarks will return the first Point part in the geomark.  LineString geomarks will return the first coordinate of the first LineString part in the geomark. Polygon geomarks will return the centroid or another point inside the first Polygon part in the geomark. The geometry and attribution can be downloaded as a spatial download file format in a supported coordinate system. The download files can then be used in a desktop GIS application (e.g. ArcMap), Google Earth or a web mapping application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d94e870-f539-42f0-bf73-056c0a853931"
            }
          ]
        }
      ]
    }
  ]
}