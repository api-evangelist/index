swagger: "2.0"
x-collection-name: AWS Rekognition
x-complete: 1
info:
  title: AWS Rekognition API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CompareFaces:
    get:
      summary: Compare Faces
      description: |-
        Compares a face in the source input image with
              each face detected in the target input image.
      operationId: compareFaces
      x-api-path-slug: actioncomparefaces-get
      parameters:
      - in: query
        name: SimilarityThreshold
        description: The minimum level of confidence in the match you want included
          in the result
        type: string
      - in: query
        name: SourceImage
        description: Source image either as bytes or an S3 object
        type: string
      - in: query
        name: TargetImage
        description: Target image either as bytes or an S3 object
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Faces
  /?Action=CreateCollection:
    get:
      summary: Create Collection
      description: Creates a collection in an AWS Region.
      operationId: createCollection
      x-api-path-slug: actioncreatecollection-get
      parameters:
      - in: query
        name: CollectionId
        description: ID for the collection that you are creating
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Collections
  /?Action=DeleteCollection:
    get:
      summary: Delete Collection
      description: Deletes the specified collection.
      operationId: deleteCollection
      x-api-path-slug: actiondeletecollection-get
      parameters:
      - in: query
        name: CollectionId
        description: ID of the collection to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Collections
  /?Action=DeleteFaces:
    get:
      summary: Delete Faces
      description: Deletes faces from a collection.
      operationId: deleteFaces
      x-api-path-slug: actiondeletefaces-get
      parameters:
      - in: query
        name: CollectionId
        description: Collection from which to remove the specific faces
        type: string
      - in: query
        name: FaceIds
        description: An array of face IDs to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Faces
  /?Action=DetectFaces:
    get:
      summary: Detect Faces
      description: Detects faces within an image (JPEG or PNG) that is provided as
        input.
      operationId: detectFaces
      x-api-path-slug: actiondetectfaces-get
      parameters:
      - in: query
        name: Attributes
        description: A list of facial attributes you would like to be returned
        type: string
      - in: query
        name: Image
        description: The image in which you want to detect faces
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Faces
  /?Action=DetectLabels:
    get:
      summary: Detect Labels
      description: |-
        Detects instances of real-world labels within an image (JPEG or PNG)
               provided as input.
      operationId: detectLabels
      x-api-path-slug: actiondetectlabels-get
      parameters:
      - in: query
        name: Image
        description: The input image
        type: string
      - in: query
        name: MaxLabels
        description: Maximum number of labels you want the service to return in the
          response
        type: string
      - in: query
        name: MinConfidence
        description: Specifies the minimum confidence level for the labels to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Labels
  /?Action=IndexFaces:
    get:
      summary: Index Faces
      description: Detects faces in the input image and adds them to the specified
        collection.
      operationId: indexFaces
      x-api-path-slug: actionindexfaces-get
      parameters:
      - in: query
        name: CollectionId
        description: ID of an existing collection to which you want to add the faces
          that are detected in the      input images
        type: string
      - in: query
        name: DetectionAttributes
        description: (Optional) Returns detailed attributes of indexed faces
        type: string
      - in: query
        name: ExternalImageId
        description: ID you want to assign to all the faces detected in the image
        type: string
      - in: query
        name: Image
        description: Provides the source image either as bytes or an S3 object
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Faces
  /?Action=ListCollections:
    get:
      summary: List Collections
      description: Returns list of collection IDs in your account.
      operationId: listCollections
      x-api-path-slug: actionlistcollections-get
      parameters:
      - in: query
        name: MaxResults
        description: Maximum number of collection IDs to return
        type: string
      - in: query
        name: NextToken
        description: Pagination token from the previous response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Collections
  /?Action=ListFaces:
    get:
      summary: List Faces
      description: Returns metadata for faces in the specified collection.
      operationId: listFaces
      x-api-path-slug: actionlistfaces-get
      parameters:
      - in: query
        name: CollectionId
        description: ID of the collection from which to list the faces
        type: string
      - in: query
        name: MaxResults
        description: Maximum number of faces to return
        type: string
      - in: query
        name: NextToken
        description: If the previous response was incomplete (because there is more
          data to retrieve), Amazon Rekognition      returns a pagination token in
          the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Faces
  /?Action=SearchFaces:
    get:
      summary: Search Faces
      description: For a given input face ID, searches for matching faces in the collection
        the face belongs to.
      operationId: searchFaces
      x-api-path-slug: actionsearchfaces-get
      parameters:
      - in: query
        name: CollectionId
        description: ID of the collection the face belongs to
        type: string
      - in: query
        name: FaceId
        description: ID of a face to find matches for in the collection
        type: string
      - in: query
        name: FaceMatchThreshold
        description: Optional value specifying the minimum confidence in the face
          match to return
        type: string
      - in: query
        name: MaxFaces
        description: Maximum number of faces to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Faces
  /?Action=SearchFacesByImage:
    get:
      summary: Search Faces By Image
      description: |-
        For a given input image, first detects the largest face in the image, and
              then searches the specified collection for matching faces.
      operationId: searchFacesByImage
      x-api-path-slug: actionsearchfacesbyimage-get
      parameters:
      - in: query
        name: CollectionId
        description: ID of the collection to search
        type: string
      - in: query
        name: FaceMatchThreshold
        description: (Optional) Specifies the minimum confidence in the face match
          to return
        type: string
      - in: query
        name: Image
        description: Provides the source image either as bytes or an S3 object
        type: string
      - in: query
        name: MaxFaces
        description: Maximum number of faces to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Faces