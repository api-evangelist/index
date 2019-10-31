swagger: "2.0"
x-collection-name: Google Cloud Vision
x-complete: 1
info:
  title: Google Cloud Vision
  description: integrates-google-vision-features-including-image-labeling-face-logo-and-landmark-detection-optical-character-recognition-ocr-and-detection-of-explicit-content-into-applications-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: vision.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/images:annotate:
    post:
      summary: Run Image Detection
      description: Run image detection and annotation for a batch of images.
      operationId: vision.images.annotate
      x-api-path-slug: v1imagesannotate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Image Detection