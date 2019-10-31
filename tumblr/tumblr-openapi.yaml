swagger: "2.0"
x-collection-name: Tumblr
x-complete: 1
info:
  title: Tumblr
  description: ntshare-photos-mobile-apps-and-social-network-using-tumblrs-apis-n----
  version: 1.0.0
host: api.tumblr.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blog/{base-hostname}/info:
    get:
      summary: Get Blog Base Hostname Info
      description: This method returns general information about the blog, such as
        the title, number of posts, and other high-level data.
      operationId: blog.base_hostname.info.get
      x-api-path-slug: blogbasehostnameinfo-get
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Info
  /blog/{base-hostname}/avatar/{size}:
    get:
      summary: Get Blog Base Hostname Avatar Size
      description: Retrieves a blog's avatar in one of 9 different sizes.
      operationId: blog.base_hostname.avatar.size.get
      x-api-path-slug: blogbasehostnameavatarsize-get
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      - in: path
        name: size
        description: The size of the avatar (square, one value for both length and
          width)
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Avatar
      - Size
  /blog/{base-hostname}/followers:
    get:
      summary: Get Blog Base Hostname Followers
      description: Retrieves a blog's followers.
      operationId: blog.base_hostname.followers.get
      x-api-path-slug: blogbasehostnamefollowers-get
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      - in: query
        name: limit
        description: 'The number of results to return: 1???20, inclusive'
      - in: query
        name: offset
        description: Result to start at
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Followers
  /blog/{base-hostname}/posts/{type}:
    get:
      summary: Get Blog Base Hostname Adds Type
      description: Retrieves published posts.
      operationId: blog.base_hostname.posts.type.get
      x-api-path-slug: blogbasehostnamepoststype-get
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      - in: query
        name: format
        description: Specifies the post format to return, other than HTML
      - in: query
        name: id
        description: A specific post ID
      - in: query
        name: limit
        description: 'The number of posts to return: 1???20, inclusive'
      - in: query
        name: notes_info
        description: Indicates whether to return notes information (specify true or
          false)
      - in: query
        name: offset
        description: Post number to start at
      - in: query
        name: reblog_info
        description: Indicates whether to return reblog information (specify true
          or false)
      - in: query
        name: tag
        description: Limits the response to posts with the specified tag
      - in: path
        name: type
        description: The type of post to return
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Posts
      - Type
  /blog/{base-hostname}/posts/queue:
    get:
      summary: Get Blog Base Hostname Adds Queue
      description: Retrieves queued posts.
      operationId: blog.base_hostname.posts.queue.get
      x-api-path-slug: blogbasehostnamepostsqueue-get
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Posts
      - Queue
  /blog/{base-hostname}/posts/draft:
    get:
      summary: Get Blog Base Hostname Adds Draft
      description: Retrieves draft posts.
      operationId: blog.base_hostname.posts.draft.get
      x-api-path-slug: blogbasehostnamepostsdraft-get
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Posts
      - Draft
  /blog/{base-hostname}/posts/submission:
    get:
      summary: Get Blog Base Hostname Adds Submission
      description: Retrieves submission posts.
      operationId: blog.base_hostname.posts.submission.get
      x-api-path-slug: blogbasehostnamepostssubmission-get
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Posts
      - Submission
  /blog/{base-hostname}/post:
    post:
      summary: Add Blog Base Hostname Add
      description: Creates a new video blog post.
      operationId: blog.base_hostname.post.post
      x-api-path-slug: blogbasehostnamepost-post
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      - in: query
        name: caption
        description: The user-supplied caption
      - in: query
        name: data
        description: A video file, as URL-encoded binary
      - in: query
        name: date
        description: The GMT date and time of the post, as a string
      - in: query
        name: embed
        description: HTML embed code for the video
      - in: query
        name: markdown
        description: Indicates whether the post uses markdown syntax
      - in: query
        name: tags
        description: Comma-separated tags for this post
      - in: query
        name: tweet
        description: 'Manages the autotweet (if enabled) for this post: set to off
          for no tweet, or enter text to override the default tweet'
      - in: query
        name: type
        description: The type of post to create
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Post
  /blog/{base-hostname}/post/edit:
    post:
      summary: Add Blog Base Hostname Add Edit
      description: Edits a blog post.
      operationId: blog.base_hostname.post.edit.post
      x-api-path-slug: blogbasehostnamepostedit-post
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      - in: query
        name: date
        description: The GMT date and time of the post, as a string
      - in: query
        name: id
        description: The ID of the post to edit
      - in: query
        name: markdown
        description: Indicates whether the post uses markdown syntax
      - in: query
        name: tags
        description: Comma-separated tags for this post
      - in: query
        name: tweet
        description: 'Manages the autotweet (if enabled) for this post: set to off
          for no tweet, or enter text to override the default tweet'
      - in: query
        name: type
        description: The post type
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Post
      - Edit
  /blog/{base-hostname}/post/reblog:
    post:
      summary: Add Blog Base Hostname Add Reblog
      description: Reblogs a post.
      operationId: blog.base_hostname.post.reblog.post
      x-api-path-slug: blogbasehostnamepostreblog-post
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      - in: query
        name: comment
        description: A comment added to the reblogged post
      - in: query
        name: date
        description: The GMT date and time of the post, as a string
      - in: query
        name: id
        description: The ID of the reblogged post on tumblelog
      - in: query
        name: markdown
        description: Indicates whether the post uses markdown syntax
      - in: query
        name: reblog_key
        description: The reblog key for the reblogged post ??? get the reblog key
          with a /posts request
      - in: query
        name: tags
        description: Comma-separated tags for this post
      - in: query
        name: tweet
        description: 'Manages the autotweet (if enabled) for this post: set to off
          for no tweet, or enter text to override the default tweet'
      - in: query
        name: type
        description: The post type
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Post
      - Reblog
  /blog/{base-hostname}/post/delete:
    post:
      summary: Add Blog Base Hostname Add Delete
      description: Deletes a post.
      operationId: blog.base_hostname.post.delete.post
      x-api-path-slug: blogbasehostnamepostdelete-post
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      - in: query
        name: id
        description: The ID of the post to delete
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
      - Post
      - Delete
  /user/dashboard:
    get:
      summary: Get User Dashboard
      description: Use this method to retrieve the dashboard that matches the OAuth
        credentials submitted with the request.
      operationId: user.dashboard.get
      x-api-path-slug: userdashboard-get
      parameters:
      - in: query
        name: limit
        description: 'The number of results to return: 1???20, inclusive'
      - in: query
        name: offset
        description: Post number to start at
      - in: query
        name: since_id
        description: Return posts that have appeared after this ID
      - in: query
        name: type
        description: The type of post to return
      responses:
        200:
          description: OK
      tags:
      - User
      - Dashboard
  /user/likes:
    get:
      summary: Get User Likes
      description: Use this method to retrieve the liked posts that match the OAuth
        credentials submitted with the request.
      operationId: user.likes.get
      x-api-path-slug: userlikes-get
      parameters:
      - in: query
        name: limit
        description: 'The number of results to return: 1???20, inclusive'
      - in: query
        name: offset
        description: Liked post number to start at
      responses:
        200:
          description: OK
      tags:
      - User
      - Likes
  /user/following:
    get:
      summary: Get User Following
      description: Use this method to retrieve the blogs followed by the user whose
        OAuth credentials are submitted with the request.
      operationId: user.following.get
      x-api-path-slug: userfollowing-get
      parameters:
      - in: query
        name: limit
        description: 'The number of results to return: 1???20, inclusive'
      - in: query
        name: offset
        description: Result number to start at
      responses:
        200:
          description: OK
      tags:
      - User
      - Following
  /user/follow:
    post:
      summary: Add User Follow
      description: Follow a blog.
      operationId: user.follow.post
      x-api-path-slug: userfollow-post
      parameters:
      - in: query
        name: url
        description: The URL of the blog to follow
      responses:
        200:
          description: OK
      tags:
      - User
      - Follow
  /user/unfollow:
    post:
      summary: Add User Unfollow
      description: Unfollow a blog.
      operationId: user.unfollow.post
      x-api-path-slug: userunfollow-post
      parameters:
      - in: query
        name: url
        description: The URL of the blog to unfollow
      responses:
        200:
          description: OK
      tags:
      - User
      - Unfollow