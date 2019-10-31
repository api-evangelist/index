{
  "info": {
    "name": "Tumblr Add User Unfollow",
    "_postman_id": "6f5fc60f-65d9-47ff-99f5-5df2d8c490d1",
    "description": "Unfollow a blog.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blog",
      "item": [
        {
          "id": "78009b94-85f3-4e4c-83b9-f9a52d82dc01",
          "name": "blog.base_hostname.info.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/info"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method returns general information about the blog, such as the title, number of posts, and other high-level data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "625f78d7-f2cc-441a-be5e-cfd89b316fb0"
            }
          ]
        },
        {
          "id": "f5ab1beb-8626-4e40-964a-1ae49f9a4b49",
          "name": "blog.base_hostname.avatar.size.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/avatar/:size"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                },
                {
                  "id": "size",
                  "value": "size",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a blog's avatar in one of 9 different sizes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f0a3c26-d96d-4657-8d70-5aa20e1924e4"
            }
          ]
        },
        {
          "id": "072f54c1-8cf8-47a2-826d-947812c66dbf",
          "name": "blog.base_hostname.followers.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/followers"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a blog's followers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2aaa349-5f11-49dc-8462-75433b75908f"
            }
          ]
        },
        {
          "id": "cc9a818a-4fc7-4c12-bbd3-41c53e0fc608",
          "name": "blog.base_hostname.posts.type.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/posts/:type"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "notes_info",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "reblog_info",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tag",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                },
                {
                  "id": "type",
                  "value": "type",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves published posts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c25ef22-4929-4a9a-bc0b-2068d718e59e"
            }
          ]
        },
        {
          "id": "708ae6b1-79e6-41ff-a499-b1e1831c9a03",
          "name": "blog.base_hostname.posts.queue.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/posts/queue"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves queued posts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1af757c-1438-47af-b2e2-604928b37e6f"
            }
          ]
        },
        {
          "id": "6b557080-4458-4ba5-9fe3-09c001a5b40c",
          "name": "blog.base_hostname.posts.draft.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/posts/draft"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves draft posts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "869eb48c-af44-4807-beeb-d3cf58e06f7f"
            }
          ]
        },
        {
          "id": "07a58076-471c-45e7-a632-741f13c14a39",
          "name": "blog.base_hostname.posts.submission.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/posts/submission"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves submission posts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62b34ed6-28e9-4512-9f84-cc04f76d673a"
            }
          ]
        },
        {
          "id": "ee907f17-b164-4fec-90ce-df41e799a630",
          "name": "blog.base_hostname.post.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/post"
              ],
              "query": [
                {
                  "key": "caption",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "data",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "embed",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "markdown",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tweet",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new video blog post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d346c8d-7bd1-45e9-aade-3f945f87ac2e"
            }
          ]
        },
        {
          "id": "93204139-8813-4bf1-9c17-f8c66cd8d4d6",
          "name": "blog.base_hostname.post.edit.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/post/edit"
              ],
              "query": [
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "markdown",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tweet",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Edits a blog post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a680ef3-0c01-4314-b9b8-2bdc0d176f5b"
            }
          ]
        },
        {
          "id": "081b7607-c07c-46e8-8867-09d17ec25721",
          "name": "blog.base_hostname.post.reblog.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/post/reblog"
              ],
              "query": [
                {
                  "key": "comment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "markdown",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "reblog_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tweet",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reblogs a post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6acbff3-c888-45a0-a9c5-7aabf4e91145"
            }
          ]
        },
        {
          "id": "7794ce8e-bbce-48e6-9d49-62e63f91ee6d",
          "name": "blog.base_hostname.post.delete.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/post/delete"
              ],
              "query": [
                {
                  "key": "id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f386dcdb-6b76-421d-a250-c1397f07cf69"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "d1ec42c8-cd3d-4416-920d-9436b21e2640",
          "name": "user.dashboard.get",
          "request": {
            "url": "http://api.tumblr.com/v2/user/dashboard?limit=%7B%7D&offset=%7B%7D&since_id=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Use this method to retrieve the dashboard that matches the OAuth credentials submitted with the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53342fc7-19ec-4ce9-91b4-637b190def4e"
            }
          ]
        },
        {
          "id": "fdf0de47-428d-48bf-b56e-f729037d34c1",
          "name": "user.likes.get",
          "request": {
            "url": "http://api.tumblr.com/v2/user/likes?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Use this method to retrieve the liked posts that match the OAuth credentials submitted with the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c031d663-91f0-4e7c-9a00-957f8e5ce66e"
            }
          ]
        },
        {
          "id": "bb08dfb1-9c69-4e97-bdd1-dc4d1db2afa3",
          "name": "user.following.get",
          "request": {
            "url": "http://api.tumblr.com/v2/user/following?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Use this method to retrieve the blogs followed by the user whose OAuth credentials are submitted with the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b89428ca-cee0-44db-8d65-8e0427676116"
            }
          ]
        },
        {
          "id": "9ff382c4-3d0e-47de-a42b-7623cacee012",
          "name": "user.follow.post",
          "request": {
            "url": "http://api.tumblr.com/v2/user/follow?url=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Follow a blog."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43b63050-7427-4f4f-84e4-7623b96f8a89"
            }
          ]
        },
        {
          "id": "90849221-5e7f-4e4f-85e6-96dbe992bde3",
          "name": "user.unfollow.post",
          "request": {
            "url": "http://api.tumblr.com/v2/user/unfollow?url=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Unfollow a blog."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e217e6a0-4537-4450-a9d5-a4145f74255c"
            }
          ]
        }
      ]
    }
  ]
}