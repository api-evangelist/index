swagger: "2.0"
x-collection-name: SoundCloud
x-complete: 1
info:
  title: Sound Cloud
  description: access-host-upload-and-comment-on-audio-
  version: 1.0.0
host: api.soundcloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tracks.json:
    get:
      summary: Get Tracks
      description: Returns a collection of tracks
      operationId: getTracks.json
      x-api-path-slug: tracks-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Tracks
    post:
      summary: Post Tracks
      description: Uploads a track
      operationId: postTracks.json
      x-api-path-slug: tracks-json-post
      responses:
        200:
          description: OK
      tags:
      - Tracks
  /tracks/{track_id}.json:
    get:
      summary: Get Tracks Track
      description: Returns a track by track id
      operationId: getTracksTrack.json
      x-api-path-slug: trackstrack-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
    put:
      summary: Put Tracks Track
      description: Updates a given track
      operationId: putTracksTrack.json
      x-api-path-slug: trackstrack-id-json-put
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
    delete:
      summary: Delete Tracks Track
      description: Deletes a given track
      operationId: deleteTracksTrack.json
      x-api-path-slug: trackstrack-id-json-delete
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
  /tracks/{track_id}/comments.json:
    get:
      summary: Get Tracks Track Comments
      description: Returns comments of a track by track id
      operationId: getTracksTrackComments.json
      x-api-path-slug: trackstrack-idcomments-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Comments
    post:
      summary: Post Tracks Track Comments
      description: Posts a comments to a track by track id
      operationId: postTracksTrackComments.json
      x-api-path-slug: trackstrack-idcomments-json-post
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Comments
  /tracks/{track_id}/permissions.json:
    get:
      summary: Get Tracks Track Permissions
      description: Returns all users with permission for a track by track id
      operationId: getTracksTrackPermissions.json
      x-api-path-slug: trackstrack-idpermissions-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Permissions
    put:
      summary: Put Tracks Track Permissions
      description: Updates the list of permitted users for a track by track id
      operationId: putTracksTrackPermissions.json
      x-api-path-slug: trackstrack-idpermissions-json-put
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Permissions
  /tracks/{track_id}/secret-token.json:
    get:
      summary: Get Tracks Track Secret Token
      description: Returns the secret token for a track by track id. This resource
        can only be used by the track owner.
      operationId: getTracksTrackSecretToken.json
      x-api-path-slug: trackstrack-idsecrettoken-json-get
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Secret
      - Token
    put:
      summary: Put Tracks Track Secret Token
      description: |-
        Resets the secret token for a track by track id. The secret token can not be specified but will be randomly chosen on
                  the server and returned. This resource can only be used by the track owner.
      operationId: putTracksTrackSecretToken.json
      x-api-path-slug: trackstrack-idsecrettoken-json-put
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Secret
      - Token
  /users.json:
    get:
      summary: Get Users
      description: Returns a collection of users
      operationId: getUsers.json
      x-api-path-slug: users-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{user_id}.json:
    get:
      summary: Get Users
      description: Returns a user by user id
      operationId: getUsersUser.json
      x-api-path-slug: usersuser-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{user_id}/tracks.json:
    get:
      summary: Get Users Tracks
      description: Returns a collection of tracks uploaded by user id
      operationId: getUsersUserTracks.json
      x-api-path-slug: usersuser-idtracks-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Tracks
  /users/{user_id}/comments.json:
    get:
      summary: Get Users Comments
      description: Returns a collection of comments made by user id
      operationId: getUsersUserComments.json
      x-api-path-slug: usersuser-idcomments-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Comments
  /users/{user_id}/followings.json:
    get:
      summary: Get Users Followings
      description: Returns a collection of users the user with user id is following
      operationId: getUsersUserFollowings.json
      x-api-path-slug: usersuser-idfollowings-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
  /users/{user_id}/followings/{contact_id}.json:
    get:
      summary: Get Users Followings Contact
      description: Checks if the user with the id contact_id is in the givens user's
        list of contacts.
      operationId: getUsersUserFollowingsContact.json
      x-api-path-slug: usersuser-idfollowingscontact-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - Contact
    put:
      summary: Put Users Followings Contact
      description: Adds the user with the id contact_id to the givens user's list
        of contacts.
      operationId: putUsersUserFollowingsContact.json
      x-api-path-slug: usersuser-idfollowingscontact-id-json-put
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - Contact
    delete:
      summary: Delete Users Followings Contact
      description: Removes the user with the id contact_id from the givens user's
        list of contacts.
      operationId: deleteUsersUserFollowingsContact.json
      x-api-path-slug: usersuser-idfollowingscontact-id-json-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - Contact
  /users/{user_id}/followers.json:
    get:
      summary: Get Users Followers
      description: Returns a collection of users who follow the user with user id
      operationId: getUsersUserFollowers.json
      x-api-path-slug: usersuser-idfollowers-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followers
  /users/{user_id}/followers/{contact_id}.json:
    get:
      summary: Get Users Followers Contact
      description: Checks if the user with contact_id is a follower of the given user.
      operationId: getUsersUserFollowersContact.json
      x-api-path-slug: usersuser-idfollowerscontact-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followers
      - Contact
  /users/{user_id}/favorites.json:
    get:
      summary: Get Users Favorites
      description: Returns a collection of tracks favorited by the user with user
        id
      operationId: getUsersUserFavorites.json
      x-api-path-slug: usersuser-idfavorites-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
  /users/{user_id}/favorites/{track_id}.json:
    put:
      summary: Put Users Favorites Track
      description: Adds the given track to the given user's list of favorites.
      operationId: putUsersUserFavoritesTrack.json
      x-api-path-slug: usersuser-idfavoritestrack-id-json-put
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Track
    delete:
      summary: Delete Users Favorites Track
      description: Deletes the given track from the given user's list of favorites.
      operationId: deleteUsersUserFavoritesTrack.json
      x-api-path-slug: usersuser-idfavoritestrack-id-json-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Track
  /users/{user_id}/groups.json:
    get:
      summary: Get Users Groups
      description: Returns a collection of groups joined by user with user id
      operationId: getUsersUserGroups.json
      x-api-path-slug: usersuser-idgroups-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /users/{user_id}/playlists.json:
    get:
      summary: Get Users Playlists
      description: Returns a collection of playlists created by user with user id
      operationId: getUsersUserPlaylists.json
      x-api-path-slug: usersuser-idplaylists-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Playlists
  /me.json:
    get:
      summary: Get Me
      description: Returns the logged-in user
      operationId: getMe.json
      x-api-path-slug: me-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
    put:
      summary: Put Me
      description: Updates the logged-in user
      operationId: putMe.json
      x-api-path-slug: me-json-put
      responses:
        200:
          description: OK
      tags:
      - Me
  /me/tracks.json:
    get:
      summary: Get Me Tracks
      description: Returns a collection of tracks uploaded by logged-in user
      operationId: getMeTracks.json
      x-api-path-slug: metracks-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Tracks
  /me/comments.json:
    get:
      summary: Get Me Comments
      description: Returns a collection of comments made by logged-in user
      operationId: getMeComments.json
      x-api-path-slug: mecomments-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Comments
  /me/followings.json:
    get:
      summary: Get Me Followings
      description: Returns a collection of users the logged-in user is following
      operationId: getMeFollowings.json
      x-api-path-slug: mefollowings-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Followings
  /me/followings/{contact_id}.json:
    get:
      summary: Get Me Followings Contact
      description: Checks if the user with the id contact_id is in the logged-in user's
        list of contacts.
      operationId: getMeFollowingsContact.json
      x-api-path-slug: mefollowingscontact-id-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Followings
      - Contact
    put:
      summary: Put Me Followings Contact
      description: Adds the user with the id contact_id to the logged-in user's list
        of contacts.
      operationId: putMeFollowingsContact.json
      x-api-path-slug: mefollowingscontact-id-json-put
      responses:
        200:
          description: OK
      tags:
      - Me
      - Followings
      - Contact
    delete:
      summary: Delete Me Followings Contact
      description: Deletes the user with the id contact_id from the logged-in user's
        list of contacts.
      operationId: deleteMeFollowingsContact.json
      x-api-path-slug: mefollowingscontact-id-json-delete
      responses:
        200:
          description: OK
      tags:
      - Me
      - Followings
      - Contact
  /me/followers.json:
    get:
      summary: Get Me Followers
      description: Returns a collection of users who follow the logged-in user
      operationId: getMeFollowers.json
      x-api-path-slug: mefollowers-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Followers
  /me/followers/{contact_id}.json:
    get:
      summary: Get Me Followers Contact
      description: Checks if the user with the id contact_id is a follower of the
        logged-in user
      operationId: getMeFollowersContact.json
      x-api-path-slug: mefollowerscontact-id-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Followers
      - Contact
  /me/favorites.json:
    get:
      summary: Get Me Favorites
      description: Returns a collection of tracks favorited by the logged-in user
      operationId: getMeFavorites.json
      x-api-path-slug: mefavorites-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Favorites
  /me/favorites/{track_id}.json:
    put:
      summary: Put Me Favorites Track
      description: Adds the given track to the logged-in user's list of favorites.
      operationId: putMeFavoritesTrack.json
      x-api-path-slug: mefavoritestrack-id-json-put
      responses:
        200:
          description: OK
      tags:
      - Me
      - Favorites
      - Track
    delete:
      summary: Delete Me Favorites Track
      description: Deletes the given track from the logged-in user's list of favorites.
      operationId: deleteMeFavoritesTrack.json
      x-api-path-slug: mefavoritestrack-id-json-delete
      responses:
        200:
          description: OK
      tags:
      - Me
      - Favorites
      - Track
  /me/groups.json:
    get:
      summary: Get Me Groups
      description: Returns a collection of groups joined by logged-in user
      operationId: getMeGroups.json
      x-api-path-slug: megroups-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Groups
  /me/playlists.json:
    get:
      summary: Get Me Playlists
      description: Returns a collection of playlists created by the logged-in user
      operationId: getMePlaylists.json
      x-api-path-slug: meplaylists-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Playlists
  /playlists.json:
    get:
      summary: Get Playlists
      description: Returns a collection of playlists
      operationId: getPlaylists.json
      x-api-path-slug: playlists-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Playlists
  /playlists/{playlist_id}.json:
    get:
      summary: Get Playlists Playlist
      description: Returns a playlist by playlist id
      operationId: getPlaylistsPlaylist.json
      x-api-path-slug: playlistsplaylist-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Playlists
      - Playlist
  /groups.json:
    get:
      summary: Get Groups
      description: Returns a collection of groups
      operationId: getGroups.json
      x-api-path-slug: groups-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/{group_id}.json:
    get:
      summary: Get Groups
      description: Returns a group by group id
      operationId: getGroupsGroup.json
      x-api-path-slug: groupsgroup-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/{group_id}/users.json:
    get:
      summary: Get Groups Users
      description: Returns a combined collection of moderators, members and contributors
        of the group with group id
      operationId: getGroupsGroupUsers.json
      x-api-path-slug: groupsgroup-idusers-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Users
  /groups/{group_id}/moderators.json:
    get:
      summary: Get Groups Moderators
      description: Returns a collection of moderators of the group with group id
      operationId: getGroupsGroupModerators.json
      x-api-path-slug: groupsgroup-idmoderators-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Moderators
  /groups/{group_id}/members.json:
    get:
      summary: Get Groups Members
      description: Returns a collection of members of the group with group id
      operationId: getGroupsGroupMembers.json
      x-api-path-slug: groupsgroup-idmembers-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
  /groups/{group_id}/contributors.json:
    get:
      summary: Get Groups Contributors
      description: Returns a collection of contributors of the group with group id
      operationId: getGroupsGroupContributors.json
      x-api-path-slug: groupsgroup-idcontributors-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Contributors
  /groups/{group_id}/tracks.json:
    get:
      summary: Get Groups Tracks
      description: Returns a collection of tracks contributed to the group with group
        id
      operationId: getGroupsGroupTracks.json
      x-api-path-slug: groupsgroup-idtracks-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Tracks
  /comments/{comment_id}.json:
    get:
      summary: Get Comments
      description: Returns a comment by comment id
      operationId: getCommentsComment.json
      x-api-path-slug: commentscomment-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Comments
  /resolve.json:
    get:
      summary: Get Resolve
      description: Translates a website URI into an API URI
      operationId: getResolve.json
      x-api-path-slug: resolve-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Resolve
  /tracks.{format}:
    get:
      summary: Get Tracks. Format
      description: Returns a collection of tracks
      operationId: getTracks.Format
      x-api-path-slug: tracks-format-get
      parameters:
      - in: query
        name: bpm-from
        description: Access, host, upload, and comment on audio
      - in: query
        name: bpm-to
        description: Access, host, upload, and comment on audio
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: created_at-from
        description: Access, host, upload, and comment on audio
      - in: query
        name: created_at-to
        description: Access, host, upload, and comment on audio
      - in: query
        name: duration-from
        description: Access, host, upload, and comment on audio
      - in: query
        name: duration-to
        description: Access, host, upload, and comment on audio
      - in: query
        name: filter
        description: Access, host, upload, and comment on audio
      - in: query
        name: ids
        description: Access, host, upload, and comment on audio
      - in: query
        name: order
        description: Access, host, upload, and comment on audio
      - in: query
        name: q
        description: Access, host, upload, and comment on audio
      - in: query
        name: tags
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - ""
      - Format
    post:
      summary: Post Tracks. Format
      description: Post tracks. format.
      operationId: postTracks.Format
      x-api-path-slug: tracks-format-post
      parameters:
      - in: query
        name: asset_data
        description: Access, host, upload, and comment on audio
      - in: query
        name: title
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - ""
      - Format
  /tracks/{track_id}.{format}:
    get:
      summary: Get Tracks Track . Format
      description: Returns a track by track id
      operationId: getTracksTrack.Format
      x-api-path-slug: trackstrack-id-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - ""
      - ""
      - Format
    put:
      summary: Put Tracks Track . Format
      description: Put tracks track . format.
      operationId: putTracksTrack.Format
      x-api-path-slug: trackstrack-id-format-put
      parameters:
      - in: query
        name: asset_data
        description: Access, host, upload, and comment on audio
      - in: query
        name: title
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - ""
      - ""
      - Format
    delete:
      summary: Delete Tracks Track . Format
      description: Delete tracks track . format.
      operationId: deleteTracksTrack.Format
      x-api-path-slug: trackstrack-id-format-delete
      parameters:
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - ""
      - ""
      - Format
  /tracks/{track_id}/comments.{format}:
    get:
      summary: Get Tracks Track Comments. Format
      description: Returns comments of a track by track id
      operationId: getTracksTrackComments.Format
      x-api-path-slug: trackstrack-idcomments-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Comments
      - ""
      - Format
    post:
      summary: Post Tracks Track Comments. Format
      description: Posts a comments to a track by track id
      operationId: postTracksTrackComments.Format
      x-api-path-slug: trackstrack-idcomments-format-post
      parameters:
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Comments
      - ""
      - Format
  /tracks/{track_id}/permissions.{format}:
    get:
      summary: Get Tracks Track Permissions. Format
      description: Returns all users with permission for a track by track id
      operationId: getTracksTrackPermissions.Format
      x-api-path-slug: trackstrack-idpermissions-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Permissions
      - ""
      - Format
    put:
      summary: Put Tracks Track Permissions. Format
      description: Updates the list of permitted users for a track by track id
      operationId: putTracksTrackPermissions.Format
      x-api-path-slug: trackstrack-idpermissions-format-put
      parameters:
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Permissions
      - ""
      - Format
  /tracks/{track_id}/secret-token.{format}:
    get:
      summary: Get Tracks Track Secret Token. Format
      description: Returns the secret token for a track by track id. This resource
        can only be used by the track owner.
      operationId: getTracksTrackSecretToken.Format
      x-api-path-slug: trackstrack-idsecrettoken-format-get
      parameters:
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Secret
      - Token
      - ""
      - Format
    put:
      summary: Put Tracks Track Secret Token. Format
      description: |-
        Resets the secret token for a track by track id. The secret token can not be specified but will be randomly chosen on
                            the server and returned. This resource can only be used by the track owner.
      operationId: putTracksTrackSecretToken.Format
      x-api-path-slug: trackstrack-idsecrettoken-format-put
      parameters:
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Secret
      - Token
      - ""
      - Format
  /users.{format}:
    get:
      summary: Get Users. Format
      description: Returns a collection of users
      operationId: getUsers.Format
      x-api-path-slug: users-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: q
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - Format
  /users/{user_id}.{format}:
    get:
      summary: Get Users . Format
      description: Returns a user by user id
      operationId: getUsersUser.Format
      x-api-path-slug: usersuser-id-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - ""
      - Format
  /users/{user_id}/tracks.{format}:
    get:
      summary: Get Users Tracks. Format
      description: Returns a collection of tracks uploaded by user id
      operationId: getUsersUserTracks.Format
      x-api-path-slug: usersuser-idtracks-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Tracks
      - ""
      - Format
  /users/{user_id}/comments.{format}:
    get:
      summary: Get Users Comments. Format
      description: Returns a collection of comments made by user id
      operationId: getUsersUserComments.Format
      x-api-path-slug: usersuser-idcomments-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Comments
      - ""
      - Format
  /users/{user_id}/followings.{format}:
    get:
      summary: Get Users Followings. Format
      description: Returns a collection of users the user with user id is following
      operationId: getUsersUserFollowings.Format
      x-api-path-slug: usersuser-idfollowings-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - ""
      - Format
  /users/{user_id}/followings/{contact_id}.{format}:
    get:
      summary: Get Users Followings Contact . Format
      description: Checks if the user with the id contact_id is in the givens user's
        list of contacts.
      operationId: getUsersUserFollowingsContact.Format
      x-api-path-slug: usersuser-idfollowingscontact-id-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: contact_id
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - Contact
      - ""
      - ""
      - Format
    put:
      summary: Put Users Followings Contact . Format
      description: Adds the user with the id contact_id to the givens user's list
        of contacts.
      operationId: putUsersUserFollowingsContact.Format
      x-api-path-slug: usersuser-idfollowingscontact-id-format-put
      parameters:
      - in: path
        name: contact_id
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - Contact
      - ""
      - ""
      - Format
    delete:
      summary: Delete Users Followings Contact . Format
      description: Removes the user with the id contact_id from the givens user's
        list of contacts.
      operationId: deleteUsersUserFollowingsContact.Format
      x-api-path-slug: usersuser-idfollowingscontact-id-format-delete
      parameters:
      - in: path
        name: contact_id
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followings
      - Contact
      - ""
      - ""
      - Format
  /users/{user_id}/followers.{format}:
    get:
      summary: Get Users Followers. Format
      description: Returns a collection of users who follow the user with user id
      operationId: getUsersUserFollowers.Format
      x-api-path-slug: usersuser-idfollowers-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followers
      - ""
      - Format
  /users/{user_id}/followers/{contact_id}.{format}:
    get:
      summary: Get Users Followers Contact . Format
      description: Checks if the user with contact_id is a follower of the given user.
      operationId: getUsersUserFollowersContact.Format
      x-api-path-slug: usersuser-idfollowerscontact-id-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: contact_id
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Followers
      - Contact
      - ""
      - ""
      - Format
  /users/{user_id}/favorites.{format}:
    get:
      summary: Get Users Favorites. Format
      description: Returns a collection of tracks favorited by the user with user
        id
      operationId: getUsersUserFavorites.Format
      x-api-path-slug: usersuser-idfavorites-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - ""
      - Format
  /users/{user_id}/favorites/{track_id}.{format}:
    put:
      summary: Put Users Favorites Track . Format
      description: Adds the given track to the given user's list of favorites.
      operationId: putUsersUserFavoritesTrack.Format
      x-api-path-slug: usersuser-idfavoritestrack-id-format-put
      parameters:
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Track
      - ""
      - ""
      - Format
    delete:
      summary: Delete Users Favorites Track . Format
      description: Deletes the given track from the given user's list of favorites.
      operationId: deleteUsersUserFavoritesTrack.Format
      x-api-path-slug: usersuser-idfavoritestrack-id-format-delete
      parameters:
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
      - Track
      - ""
      - ""
      - Format
  /users/{user_id}/groups.{format}:
    get:
      summary: Get Users Groups. Format
      description: Returns a collection of groups joined by user with user id
      operationId: getUsersUserGroups.Format
      x-api-path-slug: usersuser-idgroups-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
      - ""
      - Format
  /users/{user_id}/playlists.{format}:
    get:
      summary: Get Users Playlists. Format
      description: Returns a collection of playlists created by user with user id
      operationId: getUsersUserPlaylists.Format
      x-api-path-slug: usersuser-idplaylists-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Playlists
      - ""
      - Format
  /me.{format}:
    get:
      summary: Get Me. Format
      description: Returns the logged-in user
      operationId: getMe.Format
      x-api-path-slug: me-format-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - ""
      - Format
    put:
      summary: Put Me. Format
      description: Updates the logged-in user
      operationId: putMe.Format
      x-api-path-slug: me-format-put
      responses:
        200:
          description: OK
      tags:
      - Me
      - ""
      - Format
  /me/tracks.{format}:
    get:
      summary: Get Me Tracks. Format
      description: Returns a collection of tracks uploaded by logged-in user
      operationId: getMeTracks.Format
      x-api-path-slug: metracks-format-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Tracks
      - ""
      - Format
  /me/comments.{format}:
    get:
      summary: Get Me Comments. Format
      description: Returns a collection of comments made by logged-in user
      operationId: getMeComments.Format
      x-api-path-slug: mecomments-format-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Comments
      - ""
      - Format
  /me/followings.{format}:
    get:
      summary: Get Me Followings. Format
      description: Returns a collection of users the logged-in user is following
      operationId: getMeFollowings.Format
      x-api-path-slug: mefollowings-format-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Followings
      - ""
      - Format
  /me/followings/{contact_id}.{format}:
    get:
      summary: Get Me Followings Contact . Format
      description: Checks if the user with the id contact_id is in the logged-in user's
        list of contacts.
      operationId: getMeFollowingsContact.Format
      x-api-path-slug: mefollowingscontact-id-format-get
      parameters:
      - in: path
        name: contact_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Me
      - Followings
      - Contact
      - ""
      - ""
      - Format
    put:
      summary: Put Me Followings Contact . Format
      description: Adds the user with the id contact_id to the logged-in user's list
        of contacts.
      operationId: putMeFollowingsContact.Format
      x-api-path-slug: mefollowingscontact-id-format-put
      parameters:
      - in: path
        name: contact_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Me
      - Followings
      - Contact
      - ""
      - ""
      - Format
    delete:
      summary: Delete Me Followings Contact . Format
      description: Deletes the user with the id contact_id from the logged-in user's
        list of contacts.
      operationId: deleteMeFollowingsContact.Format
      x-api-path-slug: mefollowingscontact-id-format-delete
      parameters:
      - in: path
        name: contact_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Me
      - Followings
      - Contact
      - ""
      - ""
      - Format
  /me/followers.{format}:
    get:
      summary: Get Me Followers. Format
      description: Returns a collection of users who follow the logged-in user
      operationId: getMeFollowers.Format
      x-api-path-slug: mefollowers-format-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Followers
      - ""
      - Format
  /me/followers/{contact_id}.{format}:
    get:
      summary: Get Me Followers Contact . Format
      description: Checks if the user with the id contact_id is a follower of the
        logged-in user
      operationId: getMeFollowersContact.Format
      x-api-path-slug: mefollowerscontact-id-format-get
      parameters:
      - in: path
        name: contact_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Me
      - Followers
      - Contact
      - ""
      - ""
      - Format
  /me/favorites.{format}:
    get:
      summary: Get Me Favorites. Format
      description: Returns a collection of tracks favorited by the logged-in user
      operationId: getMeFavorites.Format
      x-api-path-slug: mefavorites-format-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Favorites
      - ""
      - Format
  /me/favorites/{track_id}.{format}:
    put:
      summary: Put Me Favorites Track . Format
      description: Adds the given track to the logged-in user's list of favorites.
      operationId: putMeFavoritesTrack.Format
      x-api-path-slug: mefavoritestrack-id-format-put
      parameters:
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Me
      - Favorites
      - Track
      - ""
      - ""
      - Format
    delete:
      summary: Delete Me Favorites Track . Format
      description: Deletes the given track from the logged-in user's list of favorites.
      operationId: deleteMeFavoritesTrack.Format
      x-api-path-slug: mefavoritestrack-id-format-delete
      parameters:
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Me
      - Favorites
      - Track
      - ""
      - ""
      - Format
  /me/groups.{format}:
    get:
      summary: Get Me Groups. Format
      description: Returns a collection of groups joined by logged-in user
      operationId: getMeGroups.Format
      x-api-path-slug: megroups-format-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Groups
      - ""
      - Format
  /me/playlists.{format}:
    get:
      summary: Get Me Playlists. Format
      description: Returns a collection of playlists created by the logged-in user
      operationId: getMePlaylists.Format
      x-api-path-slug: meplaylists-format-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Playlists
      - ""
      - Format
  /playlists.{format}:
    get:
      summary: Get Playlists. Format
      description: Returns a collection of playlists
      operationId: getPlaylists.Format
      x-api-path-slug: playlists-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: filter
        description: Access, host, upload, and comment on audio
      - in: query
        name: q
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Playlists
      - ""
      - Format
  /playlists/{playlist_id}.{format}:
    get:
      summary: Get Playlists Playlist . Format
      description: Returns a playlist by playlist id
      operationId: getPlaylistsPlaylist.Format
      x-api-path-slug: playlistsplaylist-id-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: playlist_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Playlists
      - Playlist
      - ""
      - ""
      - Format
  /groups.{format}:
    get:
      summary: Get Groups. Format
      description: Returns a collection of groups
      operationId: getGroups.Format
      x-api-path-slug: groups-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Groups
      - ""
      - Format
  /groups/{group_id}.{format}:
    get:
      summary: Get Groups . Format
      description: Returns a group by group id
      operationId: getGroupsGroup.Format
      x-api-path-slug: groupsgroup-id-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: playlist_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Groups
      - ""
      - ""
      - Format
  /groups/{group_id}/users.{format}:
    get:
      summary: Get Groups Users. Format
      description: Returns a combined collection of moderators, members and contributors
        of the group with group id
      operationId: getGroupsGroupUsers.Format
      x-api-path-slug: groupsgroup-idusers-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: playlist_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Users
      - ""
      - Format
  /groups/{group_id}/moderators.{format}:
    get:
      summary: Get Groups Moderators. Format
      description: Returns a collection of moderators of the group with group id
      operationId: getGroupsGroupModerators.Format
      x-api-path-slug: groupsgroup-idmoderators-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: playlist_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Moderators
      - ""
      - Format
  /groups/{group_id}/members.{format}:
    get:
      summary: Get Groups Members. Format
      description: Returns a collection of members of the group with group id
      operationId: getGroupsGroupMembers.Format
      x-api-path-slug: groupsgroup-idmembers-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: playlist_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
      - ""
      - Format
  /groups/{group_id}/contributors.{format}:
    get:
      summary: Get Groups Contributors. Format
      description: Returns a collection of contributors of the group with group id
      operationId: getGroupsGroupContributors.Format
      x-api-path-slug: groupsgroup-idcontributors-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: playlist_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Contributors
      - ""
      - Format
  /groups/{group_id}/tracks.{format}:
    get:
      summary: Get Groups Tracks. Format
      description: Returns a collection of tracks contributed to the group with group
        id
      operationId: getGroupsGroupTracks.Format
      x-api-path-slug: groupsgroup-idtracks-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: playlist_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Tracks
      - ""
      - Format
  /comments/{comment_id}.{format}:
    get:
      summary: Get Comments . Format
      description: Returns a comment by comment id
      operationId: getCommentsComment.Format
      x-api-path-slug: commentscomment-id-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: playlist_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Comments
      - ""
      - ""
      - Format
  /resolve.{format}:
    get:
      summary: Get Resolve. Format
      description: Translates a website URI into an API URI
      operationId: getResolve.Format
      x-api-path-slug: resolve-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: url
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Resolve
      - ""
      - Format