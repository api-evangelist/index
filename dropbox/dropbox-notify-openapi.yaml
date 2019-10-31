swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox Notify Appendix API v1
  description: the-dropbox-notify--is-a-part-of-dropbox-core-ap-with-a-separate-endpoint-for-notification-call-
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api-notify.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /longpoll_delta:
    get:
      summary: A long-poll endpoint to wait for changes on an account.
      description: |-
        A long-poll endpoint to wait for changes on an account. In conjunction with [/delta](https://www.dropbox.com/developers/core/docs#delta),
        this call gives you a low-latency way to monitor an account for file changes.

        Note that this call goes to **api-notify.dropbox.com** instead of *api.dropbox.com*.

        Unlike most other API endpoints, this call does not require OAuth authentication. The passed in `cursor` can
        only be acquired via an authenticated call to [/delta](https://www.dropbox.com/developers/core/docs#delta).
      operationId: a-longpoll-endpoint-to-wait-for-changes-on-an-account-in-conjunction-with-deltahttpswwwdropboxcomdev
      x-api-path-slug: longpoll-delta-get
      parameters:
      - in: query
        name: cursor
        description: A delta cursor as returned from a call to [/delta](https://www
      - in: query
        name: timeout
        description: An optional integer indicating a timeout, in seconds
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Notify