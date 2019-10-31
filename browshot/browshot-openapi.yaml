swagger: "2.0"
x-collection-name: Browshot
x-complete: 1
info:
  title: Browshot
  description: take-screenshots-of-any-website-in-real-time
  termsOfService: https://browshot.com/terms
  contact:
    name: API Support
    url: https://browshot.com/contact
    email: support@browshot.com
  version: 1.17.0
host: api.browshot.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/info:
    get:
      summary: Get information about your account
      description: Get information about your account.
      operationId: GetAccountInfo
      x-api-path-slug: accountinfo-get
      parameters:
      - in: query
        name: details
        description: level of information returned
      responses:
        200:
          description: OK
      tags:
      - Account
      - Info
  /batch/ceate:
    post:
      summary: Requests thousands of screenshtos at once
      description: Get hundreds or thousands of screenshots from a text file. You
        can use this API call or the dashboard. Unlike the other API calls, you must
        issue a POST request with the Content-Type "multipart/form-data" in order
        to upload the text file. The text file must contain the list of URLs to request,
        1 URL per line. Failed screenshots will be tried up to 3 times before giving
        up.
      operationId: CreateBatch
      x-api-path-slug: batchceate-post
      parameters:
      - in: formData
        name: cookie
        description: set a cookie for the URL requested (see Custom POST Data, Referer
          and Cookie) Cookies should be separated by a ; - paid screenshots only
      - in: formData
        name: delay
        description: number of seconds to wait after the page has loaded
      - in: formData
        name: details
        description: level of information available with screenshot/info
      - in: formData
        name: file
        description: text file to use
      - in: formData
        name: flash_delay
        description: number of seconds to wait after the page has loaded if Flash
          elements are present
      - in: formData
        name: format
        description: image as PNG or JPEG
      - in: formData
        name: headers
        description: any custom HTTP headers
      - in: formData
        name: height
        description: thumbnail height
      - in: query
        name: hosting
        description: hosting option - s3 or browshot
      - in: query
        name: hosting_bucket
        description: S3 bucket to upload the screenshot or thumbnail (required for
          S3)
      - in: query
        name: hosting_file
        description: file name to use (for S3 only)
      - in: query
        name: hosting_headers
        description: list of headers to add to the S3 object (for S3 only)
      - in: query
        name: hosting_height
        description: maximum height of the thumbnail to host
      - in: query
        name: hosting_scale
        description: scale of the thumbnail to host
      - in: query
        name: hosting_width
        description: maximum height of the thumbnail to host
      - in: formData
        name: html
        description: saves the HTML of the rendered page which can be retrieved by
          the API call screenshot/html
      - in: formData
        name: instance_id
        description: instance ID to use
      - in: formData
        name: max_wait
        description: maximum number of seconds to wait before triggering the PageLoad
          event
      - in: formData
        name: name
        description: name of the batch
      - in: formData
        name: post_data
        description: send a POST requests with post_data, useful for filling out forms
          - paid screenshots only
      - in: formData
        name: priority
        description: assign priority to the screenshot (for private instances only)
      - in: formData
        name: referer
        description: use a custom referrer header - paid screenshots only
      - in: formData
        name: screen_height
        description: height of the browser window
      - in: formData
        name: screen_width
        description: width of the browser window
      - in: formData
        name: script
        description: URL of javascript file to execute after the page load event
      - in: formData
        name: size
        description: screenshots size - screen (default) or page
      - in: formData
        name: width
        description: thumbnail width
      responses:
        200:
          description: OK
      tags:
      - Batch
      - Ceate
  /batch/info:
    get:
      summary: Get the batch status
      description: Get the status of a batch requested through the API or through
        the dashboard.
      operationId: GetBatchInfo
      x-api-path-slug: batchinfo-get
      parameters:
      - in: query
        name: id
        description: batch ID
      responses:
        200:
          description: OK
      tags:
      - Batch
      - Info
  /browser/info:
    get:
      summary: Get information about a browser
      description: Get information about a browser.
      operationId: GetBrowserInfo
      x-api-path-slug: browserinfo-get
      parameters:
      - in: query
        name: id
        description: browser ID
      responses:
        200:
          description: OK
      tags:
      - Browser
      - Info
  /browser/list:
    get:
      summary: Get all browsers
      description: Get all browsers.
      operationId: GetBrowsersInfo
      x-api-path-slug: browserlist-get
      responses:
        200:
          description: OK
      tags:
      - Browser
      - List
  /instance/info:
    get:
      summary: Get information about an instance
      description: Get information about an instance.
      operationId: GetInstanceInfo
      x-api-path-slug: instanceinfo-get
      parameters:
      - in: query
        name: id
        description: instance ID
      responses:
        200:
          description: OK
      tags:
      - Instance
      - Info
  /instance/list:
    get:
      summary: Get all instances
      description: Get all instances.
      operationId: GetInstancesInfo
      x-api-path-slug: instancelist-get
      responses:
        200:
          description: OK
      tags:
      - Instance
      - List
  /screenshot/create:
    get:
      summary: Request a screenshot
      description: |-
        Screenshots requests to private and shared instances require a positive balance.

        *IMPORTANT*: Remember that you can only do 100 free screenshots per month. To used a premium instance, use instance_id=65 for example.
      operationId: CreateScreenshot
      x-api-path-slug: screenshotcreate-get
      parameters:
      - in: query
        name: cache
        description: use a previous screenshot (same URL, same instance) if it was
          done within  seconds
      - in: query
        name: cookie
        description: set a cookie for the URL requested (see Custom POST Data, Referer
          and Cookie) Cookies should be separated by a ; - paid screenshots only
      - in: query
        name: delay
        description: number of seconds to wait after the page has loaded
      - in: query
        name: details
        description: level of information available with screenshot/info
      - in: query
        name: flash_delay
        description: number of seconds to wait after the page has loaded if Flash
          elements are present
      - in: query
        name: headers
        description: any custom HTTP headers
      - in: query
        name: hosting
        description: hosting option - s3 or browshot
      - in: query
        name: hosting_bucket
        description: S3 bucket to upload the screenshot or thumbnail (required for
          S3)
      - in: query
        name: hosting_file
        description: file name to use (for S3 only)
      - in: query
        name: hosting_headers
        description: list of headers to add to the S3 object (for S3 only)
      - in: query
        name: hosting_height
        description: maximum height of the thumbnail to host
      - in: query
        name: hosting_scale
        description: scale of the thumbnail to host
      - in: query
        name: hosting_width
        description: maximum height of the thumbnail to host
      - in: query
        name: html
        description: saves the HTML of the rendered page which can be retrieved by
          the API call screenshot/html
      - in: query
        name: instance_id
        description: instance ID to use
      - in: query
        name: max_wait
        description: maximum number of seconds to wait before triggering the PageLoad
          event
      - in: query
        name: post_data
        description: send a POST requests with post_data, useful for filling out forms
          - paid screenshots only
      - in: query
        name: priority
        description: assign priority to the screenshot (for private instances only)
      - in: query
        name: referer
        description: use a custom referrer header - paid screenshots only
      - in: query
        name: screen_height
        description: height of the browser window
      - in: query
        name: screen_width
        description: width of the browser window
      - in: query
        name: script
        description: URL of javascript file to execute after the page load event
      - in: query
        name: shots
        description: take multiple screenshots of the same page
      - in: query
        name: shot_interval
        description: number of seconds between 2 screenshots
      - in: query
        name: size
        description: screenshot size - screen (default) or page
      - in: query
        name: url
        description: URL of the page to get a screenshot for
      responses:
        200:
          description: OK
      tags:
      - Screenshot
      - Create
  /screenshot/delete:
    get:
      summary: Delete screenshot data
      description: You can delete details of your screenshots to remove any confidential
        information.
      operationId: DeleteScreenshot
      x-api-path-slug: screenshotdelete-get
      parameters:
      - in: query
        name: data
        description: data to remove
      - in: query
        name: id
        description: screenshot ID
      responses:
        200:
          description: OK
      tags:
      - Screenshot
      - Delete
  /screenshot/host:
    get:
      summary: Host thumbnails on your own S3 account or on Browshot.
      description: You can host screenshots and thumbnails on your own S3 account
        or on Browshot.
      operationId: HostScreenshot
      x-api-path-slug: screenshothost-get
      parameters:
      - in: query
        name: bucket
        description: S3 bucket to upload the screenshot or thumbnail - required with
          hosting=s3
      - in: query
        name: file
        description: file name to use - optional, used with hosting=s3
      - in: query
        name: headers
        description: HTTP headers to add to your S3 object - optional, used with hosting=s3
      - in: query
        name: height
        description: height of the thumbnail
      - in: query
        name: hosting
        description: 'hosting option: s3 or browshot'
      - in: query
        name: id
        description: screenshot ID
      - in: query
        name: scale
        description: scale of the thumbnail
      - in: query
        name: width
        description: width of the thumbnail
      responses:
        200:
          description: OK
      tags:
      - Screenshot
      - Host
  /screenshot/html:
    get:
      summary: Get the HTML code
      description: Retrieve the HTML code of the rendered page. This API call should
        be used when html=1 was specified in the screenshot request.
      operationId: GetHTML
      x-api-path-slug: screenshothtml-get
      parameters:
      - in: query
        name: id
        description: screenshot ID
      responses:
        200:
          description: OK
      tags:
      - Screenshot
      - Html
  /screenshot/info:
    get:
      summary: Query screenshot status
      description: Once a screenshot has been requested, its status must be checked
        until it is either "error" or "finished".
      operationId: GetScreenshotInfo
      x-api-path-slug: screenshotinfo-get
      parameters:
      - in: query
        name: details
        description: level of details about the screenshot and the page
      - in: query
        name: id
        description: screenshot ID received from /api/v1/screenshot/create
      responses:
        200:
          description: OK
      tags:
      - Screenshot
      - Info
  /screenshot/list:
    get:
      summary: Get information about screenshots
      description: Get information about the last 100 screenshots requested.
      operationId: GetMultipleScreenshotsInfo
      x-api-path-slug: screenshotlist-get
      parameters:
      - in: query
        name: limit
        description: maximum number of screenshots information to return
      - in: query
        name: status
        description: get list of screenshot in a given status (error, finished, in_process)
      responses:
        200:
          description: OK
      tags:
      - Screenshot
      - List
  /screenshot/multiple:
    get:
      summary: Request multiple screenshots
      description: |-
        Request multiple screenshots in one API call. The API call accepts all the parameters supported by screenshot/create.
        You can specify up to 10 URLs and 10 instances for a total of 100 screenshots in one API call.
      operationId: CreateMultipleScreenshots
      x-api-path-slug: screenshotmultiple-get
      parameters:
      - in: query
        name: cache
        description: use a previous screenshot (same URL, same instance) if it was
          done within  seconds
      - in: query
        name: cookie
        description: set a cookie for the URL requested (see Custom POST Data, Referer
          and Cookie) Cookies should be separated by a ; - paid screenshots only
      - in: query
        name: delay
        description: number of seconds to wait after the page has loaded
      - in: query
        name: details
        description: level of information available with screenshot/info
      - in: query
        name: flash_delay
        description: number of seconds to wait after the page has loaded if Flash
          elements are present
      - in: query
        name: headers
        description: any custom HTTP headers
      - in: query
        name: hosting
        description: hosting option - s3 or browshot
      - in: query
        name: hosting_bucket
        description: S3 bucket to upload the screenshot or thumbnail (required for
          S3)
      - in: query
        name: hosting_file
        description: file name to use (for S3 only)
      - in: query
        name: hosting_headers
        description: list of headers to add to the S3 object (for S3 only)
      - in: query
        name: hosting_height
        description: maximum height of the thumbnail to host
      - in: query
        name: hosting_scale
        description: scale of the thumbnail to host
      - in: query
        name: hosting_width
        description: maximum height of the thumbnail to host
      - in: query
        name: html
        description: saves the HTML of the rendered page which can be retrieved by
          the API call screenshot/html
      - in: query
        name: instance_id
        description: instance ID to use
      - in: query
        name: max_wait
        description: maximum number of seconds to wait before triggering the PageLoad
          event
      - in: query
        name: post_data
        description: send a POST requests with post_data, useful for filling out forms
          - paid screenshots only
      - in: query
        name: priority
        description: assign priority to the screenshot (for private instances only)
      - in: query
        name: referer
        description: use a custom referrer header - paid screenshots only
      - in: query
        name: screen_height
        description: height of the browser window
      - in: query
        name: screen_width
        description: width of the browser window
      - in: query
        name: script
        description: URL of javascript file to execute after the page load event
      - in: query
        name: size
        description: screenshot size - screen (default) or page
      - in: query
        name: url
        description: URL of the page to get a screenshot for
      responses:
        200:
          description: OK
      tags:
      - Screenshot
      - Multiple
  /screenshot/search:
    get:
      summary: Search for screenshots
      description: Search for screenshots of a specific URL.
      operationId: SearchScreenshot
      x-api-path-slug: screenshotsearch-get
      parameters:
      - in: query
        name: limit
        description: maximum number of screenshots information to return
      - in: query
        name: status
        description: get list of screenshot in a given status (error, finished, in_process)
      - in: query
        name: url
        description: look for a string matching the URL requested
      responses:
        200:
          description: OK
      tags:
      - Screenshot
      - Search
  /screenshot/share:
    get:
      summary: Share a screenshot
      description: You can make your screenshots public, add notes, and share it with
        your friends and colleagues. Only screenshots which are successfully completed
        can be shared.n the thumbnail. You can take a 1024x768 screenshot, crop it
        to 768x768, and get it scaled down to 300x300.
      operationId: ShareScreenshot
      x-api-path-slug: screenshotshare-get
      parameters:
      - in: query
        name: id
        description: screenshot ID
      - in: query
        name: note
        description: note to add on the sharing page
      responses:
        200:
          description: OK
      tags:
      - Screenshot
      - Share
  /screenshot/thumbnail:
    get:
      summary: Retrieve a thumbnail image
      description: |-
        Unlike the other API calls, this API sends back the thumbnail as a PNG file, not JSON. The HTTP response code indicates whether the screenshot was successful (200), or incomplete (404) or failed (404). If the screenshot failed or is not finished, a default image "Not found" is sent.

        You can crop your screenshots. The crop is done first, then the thumbnail. You can take a 1024x768 screenshot, crop it to 768x768, and get it scaled down to 300x300.
      operationId: GetThumbnail
      x-api-path-slug: screenshotthumbnail-get
      parameters:
      - in: query
        name: bottom
        description: bottom edge of the area to be cropped
      - in: query
        name: format
        description: image as PNG or JPEG
      - in: query
        name: height
        description: height of the thumbnail
      - in: query
        name: id
        description: screenshot ID
      - in: query
        name: left
        description: left edge of the area to be cropped
      - in: query
        name: quality
        description: JPEG quality factor (for JPEG thumbnails only)
      - in: query
        name: ratio
        description: Use fit to keep the original page ration, and fill to get a thumbnail
          for the exact width and height
      - in: query
        name: right
        description: right edge of the area to be cropped
      - in: query
        name: scale
        description: scale of the thumbnail
      - in: query
        name: shot
        description: get the second or third screenshot if multiple screenshots were
          requested
      - in: query
        name: top
        description: top edge of the area to be cropped
      - in: query
        name: width
        description: width of the thumbnail
      - in: query
        name: zoom
        description: zoom 1 to 100 percent
      responses:
        200:
          description: OK
      tags:
      - Screenshot
      - Thumbnail