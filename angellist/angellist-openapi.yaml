swagger: "2.0"
x-collection-name: AngelList
x-complete: 1
info:
  title: AngelList
  description: the-angellist-api-provides-developers-with-a-restful-interface-to-the-angellist-data-set--for-more-information-read-the-oauth-faq-
  termsOfService: https://angel.co/terms
  contact:
    name: AngelList
    url: https://angel.co/api
    email: api@angel.co
  version: v1
host: api.angel.co
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accreditation:
    get:
      summary: Get Accreditation
      description: Pulls the accreditation for a startup and users.
      operationId: accreditation
      x-api-path-slug: accreditation-get
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
  /comments:
    get:
      summary: Get Comments
      description: Pulls the comments for given object.
      operationId: comments
      x-api-path-slug: comments-get
      parameters:
      - in: query
        name: commentable_id
      - in: query
        name: commentable_type
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Comments
    post:
      summary: Add Comment
      description: Adds a comment for given object
      operationId: comment
      x-api-path-slug: comments-post
      parameters:
      - in: query
        name: comment
      - in: query
        name: commentable_id
      - in: query
        name: commentable_type
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Comments
  /comments/{comment_id}:
    delete:
      summary: Delete Comment
      description: Deletes a comment for given object
      operationId: comment
      x-api-path-slug: commentscomment-id-delete
      parameters:
      - in: path
        name: comment_id
        description: The comment id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Comments
  /follows:
    delete:
      summary: Delete Follow
      description: Delete the follow for given user or startup.
      operationId: follows
      x-api-path-slug: follows-delete
      parameters:
      - in: query
        name: id
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Follow
    post:
      summary: Add Follow
      description: Add a follow for user or startup on AngelList.
      operationId: follows
      x-api-path-slug: follows-post
      parameters:
      - in: query
        name: id
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Follow
  /follows/batch:
    get:
      summary: Get Batch of Follows
      description: Returns a batched lists of follows
      operationId: followsBatch
      x-api-path-slug: followsbatch-get
      parameters:
      - in: query
        name: ids
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Follow
  /follows/relationship:
    get:
      summary: Get Follows Relationship
      description: Gets the relationships for followers
      operationId: followsRelationship
      x-api-path-slug: followsrelationship-get
      parameters:
      - in: query
        name: source_id
      - in: query
        name: target_id
      - in: query
        name: target_type
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Relationships
  /jobs:
    get:
      summary: Get Jobs
      description: Get jobs.
      operationId: jobs
      x-api-path-slug: jobs-get
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Jobs
  /jobs/{job_id}:
    get:
      summary: Get Job
      description: Get job.
      operationId: job
      x-api-path-slug: jobsjob-id-get
      parameters:
      - in: path
        name: job_id
        description: The id for the job
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Jobs
  /like:
    post:
      summary: Add Like
      description: Add like.
      operationId: like
      x-api-path-slug: like-post
      parameters:
      - in: query
        name: likable_id
      - in: query
        name: likable_type
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Likes
  /likes:
    get:
      summary: Get Likes
      description: Get likes
      operationId: likes
      x-api-path-slug: likes-get
      parameters:
      - in: query
        name: likable_id
      - in: query
        name: likable_type
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Likes
    post:
      summary: Add Like
      description: Add Like
      operationId: likes
      x-api-path-slug: likes-post
      parameters:
      - in: query
        name: likable_id
      - in: query
        name: likable_type
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Likes
  /likes/{like_id}:
    delete:
      summary: Delete Like
      description: Delete Like
      operationId: likes
      x-api-path-slug: likeslike-id-delete
      parameters:
      - in: query
        name: likable_type
      - in: path
        name: like_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Likes
  /me:
    get:
      summary: Get Me
      description: Get Me
      operationId: me
      x-api-path-slug: me-get
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
  /press:
    get:
      summary: Get Press
      description: Get Press
      operationId: press
      x-api-path-slug: press-get
      parameters:
      - in: query
        name: startup_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Press
  /press/{press_id}:
    get:
      summary: Get Press
      description: Get Press
      operationId: press
      x-api-path-slug: presspress-id-get
      parameters:
      - in: path
        name: press_id
      - in: query
        name: startup_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Press
  /reviews:
    get:
      summary: Get Reviews
      description: Get Reviews
      operationId: reviews
      x-api-path-slug: reviews-get
      parameters:
      - in: query
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Reviews
  /reviews/{review_id}:
    get:
      summary: Get Review
      description: Get Review
      operationId: reviews
      x-api-path-slug: reviewsreview-id-get
      parameters:
      - in: path
        name: review_id
      - in: query
        name: startup_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Reviews
  /search:
    get:
      summary: Search AngelList
      description: Search AngelList.
      operationId: search
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: query
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Search
  /search/slugs:
    get:
      summary: Search Slugs
      description: Search by slug
      operationId: search
      x-api-path-slug: searchslugs-get
      parameters:
      - in: query
        name: query
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Search
  /startups:
    get:
      summary: Search Startups
      description: Search Startups
      operationId: startups
      x-api-path-slug: startups-get
      parameters:
      - in: query
        name: filter
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Search
  /startups/{startup_id}:
    get:
      summary: Get Startup
      description: Get Startup
      operationId: startups
      x-api-path-slug: startupsstartup-id-get
      parameters:
      - in: path
        name: startup_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
  /startups/{startup_id}/comments:
    get:
      summary: Get Startup Comments
      description: Get Startup Comments
      operationId: startupComments
      x-api-path-slug: startupsstartup-idcomments-get
      parameters:
      - in: path
        name: startup_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Comments
  /startups/{startup_id}/followers:
    get:
      summary: Get Startup Followers
      description: Get Startup Followers
      operationId: startupFollowers
      x-api-path-slug: startupsstartup-idfollowers-get
      parameters:
      - in: path
        name: startup_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Followers
  /startups/{startup_id}/followers/ids:
    get:
      summary: Get Startup Followers IDs
      description: Get Startup Followers IDs
      operationId: startupFollowersIDs
      x-api-path-slug: startupsstartup-idfollowersids-get
      parameters:
      - in: path
        name: startup_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Followers
  /startups/{startup_id}/roles:
    get:
      summary: Get Startup Roles
      description: Get Startup Roles
      operationId: startupRoles
      x-api-path-slug: startupsstartup-idroles-get
      parameters:
      - in: path
        name: startup_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Roles
  /startup_roles:
    get:
      summary: Get Startup Roles
      description: Get Startup Roles
      operationId: 1Startup_roles
      x-api-path-slug: startup-roles-get
      parameters:
      - in: query
        name: startup_id
      - in: query
        name: v
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Roles
  /status_updates:
    get:
      summary: Get Status Updates
      description: Get Status Updates
      operationId: 1Status_updates
      x-api-path-slug: status-updates-get
      parameters:
      - in: query
        name: startup_id
      - in: query
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Status
    post:
      summary: Add Status Update
      description: Add Status Update
      operationId: statusUpdate
      x-api-path-slug: status-updates-post
      parameters:
      - in: query
        name: message
      - in: query
        name: startup_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Status
  /status_updates/{status_update_id}:
    delete:
      summary: Delete Status Update
      description: Delete Status Update
      operationId: statusUpdate
      x-api-path-slug: status-updatesstatus-update-id-delete
      parameters:
      - in: query
        name: message
      - in: query
        name: startup_id
      - in: path
        name: status_update_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Status
  /tags/{tag_id}:
    get:
      summary: Get Tag
      description: Get Tag
      operationId: tags
      x-api-path-slug: tagstag-id-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
  /tags/{tag_id}/children:
    get:
      summary: Get Tags Children
      description: Get Tags Children
      operationId: tagsChildren
      x-api-path-slug: tagstag-idchildren-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
  /tags/{tag_id}/jobs:
    get:
      summary: Get Jobs by Tag
      description: Get Jobs by Tag
      operationId: jobs
      x-api-path-slug: tagstag-idjobs-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
  /tags/{tag_id}/parents:
    get:
      summary: Get Tag Parents
      description: Get Tag Parents
      operationId: tagParents
      x-api-path-slug: tagstag-idparents-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
  /tags/{tag_id}/startups:
    get:
      summary: Get Startups by Tag
      description: Get Startups by Tag
      operationId: tagStartups
      x-api-path-slug: tagstag-idstartups-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
  /tags/{tag_id}/users:
    get:
      summary: Get Users by Tag
      description: Get Users by Tag
      operationId: tagUsers
      x-api-path-slug: tagstag-idusers-get
      parameters:
      - in: path
        name: tag_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Tags
      - Users
  /users/search:
    get:
      summary: User Search
      description: User Search
      operationId: users
      x-api-path-slug: userssearch-get
      parameters:
      - in: query
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Users
  /users/{user_id}:
    get:
      summary: Get User
      description: Get User
      operationId: user
      x-api-path-slug: usersuser-id-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Users
  /users/{user_id}/followers:
    get:
      summary: Get User Followers
      description: Get User Followers
      operationId: userFollowers
      x-api-path-slug: usersuser-idfollowers-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Users
      - Followers
  /users/{user_id}/followers/ids:
    get:
      summary: Get User Follower IDs
      description: Get User Follower IDs
      operationId: users
      x-api-path-slug: usersuser-idfollowersids-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Users
      - Followers
  /users/{user_id}/following:
    get:
      summary: Get Users Following
      description: Get Users Following
      operationId: usersFollowing
      x-api-path-slug: usersuser-idfollowing-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Users
      - Followers
  /users/{user_id}/following/ids:
    get:
      summary: Get User Following IDs
      description: Get User Following IDs
      operationId: userFollowingIDs
      x-api-path-slug: usersuser-idfollowingids-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Users
      - Followers