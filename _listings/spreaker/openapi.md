swagger: "2.0"
x-collection-name: Spreaker
x-complete: 1
info:
  title: Spreaker API
  version: v1
host: api.spreaker.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /episode/{episode_id}/media:
    get:
      summary: Get Episode Media List
      description: Get Episode Media List
      operationId: getEpisodeEpisodeMedia
      x-api-path-slug: episodeepisode-idmedia-get
      parameters:
      - in: path
        name: episode_id
        description: Unique id of episode
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
      - Media
      - List
  /user/{followed_id}/fans:
    get:
      summary: Get List of Followers
      description: Get List of Followers
      operationId: getUserFollowedFans
      x-api-path-slug: userfollowed-idfans-get
      parameters:
      - in: path
        name: followed_id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - List
      - Of
      - Followers
  /user/{follower_id}/users/fan:
    get:
      summary: Get List of Following
      description: Get List of Following
      operationId: getUserFollowerUsersFan
      x-api-path-slug: userfollower-idusersfan-get
      parameters:
      - in: path
        name: follower_id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - List
      - Of
      - Following