swagger: "2.0"
x-collection-name: Blizzard
x-complete: 1
info:
  title: World of Warcraft
  description: welcome-to-the-restful-apis-exposed-through-the-world-of-warcraft-community-site-as-a-service-to-the-world-of-warcraft-community-
  version: 1.0.0
host: us.battle.net
basePath: /api/wow/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /character/{realm}/{characterName}:
    get:
      summary: Get Character Realm Charactername
      description: Fetches a single character at a time through an HTTP GET request
        to a URL describing the character profile resource. By default, a basic dataset
        will be returned and with each request and zero or more additional fields
        can be retrieved. The core dataset returned includes the character's realm,
        name, level, last modified timestamp, thumbnail, race id, achievement points
        value, gender id and class id.
      operationId: getCharacterRealmCharactername
      x-api-path-slug: characterrealmcharactername-get
      parameters:
      - in: path
        name: characterName
        description: The character name
      - in: query
        name: fields
        description: Indicates that one or more of the optional datasets is to be
          retrieved
      - in: path
        name: realm
        description: The realm name
      responses:
        200:
          description: OK
      tags:
      - Character
      - Realm
      - CharacterName
  /guild/{realm}/{guildName}:
    get:
      summary: Get Guild Realm Guildname
      description: Fetches a single guild at a time through an HTTP GET request to
        a url describing the guild profile resource. By default, a basic dataset will
        be returned and with each request and zero or more additional fields can be
        retrieved. The core dataset returned includes the guild's name, level, faction
        and achievement points.
      operationId: getGuildRealmGuildname
      x-api-path-slug: guildrealmguildname-get
      parameters:
      - in: query
        name: fields
        description: Indicates that one or more of the optional datasets is to be
          retrieved
      - in: path
        name: guildName
        description: The guild name
      - in: path
        name: realm
        description: The realm name
      responses:
        200:
          description: OK
      tags:
      - Guild
      - Realm
      - GuildName
  /realm/status:
    get:
      summary: Get Realm Status
      description: Retrieves realms status information. This information is limited
        to whether or not the realm is up, the type and state of the realm and the
        current population.
      operationId: getRealmStatus
      x-api-path-slug: realmstatus-get
      responses:
        200:
          description: OK
      tags:
      - Realm
      - Status
  /auction/data/{realm}:
    get:
      summary: Get Auction Data Realm
      description: Provides a per-realm list of recently generated auction house data
        dumps. The current auctions data is represented as JSON structures containing
        auction data for the tree auctions houses available on each realm.
      operationId: getAuctionDataRealm
      x-api-path-slug: auctiondatarealm-get
      parameters:
      - in: path
        name: realm
        description: The realm name
      responses:
        200:
          description: OK
      tags:
      - Auction
      - Data
      - Realm
  /item/{itemId}:
    get:
      summary: Get Item Itemid
      description: Provides detailed item information.
      operationId: getItemItem
      x-api-path-slug: itemitemid-get
      parameters:
      - in: path
        name: itemId
        description: The item ID
      responses:
        200:
          description: OK
      tags:
      - Item
      - ItemId
  /arena/{realm}/{teamSize}/{teamName}:
    get:
      summary: Get Arena Realm Teamsize Teamname
      description: Provides detailed arena team information.
      operationId: getArenaRealmTeamsizeTeamname
      x-api-path-slug: arenarealmteamsizeteamname-get
      parameters:
      - in: path
        name: realm
        description: The realm name
      - in: path
        name: teamName
        description: The team name
      - in: path
        name: teamSize
        description: The team size
      responses:
        200:
          description: OK
      tags:
      - Arena
      - Realm
      - TeamSize
      - TeamName
  /data/character/races:
    get:
      summary: Get Data Character Races
      description: Provides a list of character races.
      operationId: getDataCharacterRaces
      x-api-path-slug: datacharacterraces-get
      responses:
        200:
          description: OK
      tags:
      - Data
      - Character
      - Races
  /data/character/classes:
    get:
      summary: Get Data Character Classes
      description: Provides a list of character classes.
      operationId: getDataCharacterClasses
      x-api-path-slug: datacharacterclasses-get
      responses:
        200:
          description: OK
      tags:
      - Data
      - Character
      - Classes
  /data/guild/rewards:
    get:
      summary: Get Data Guild Rewards
      description: Provides a list of all guild rewards.
      operationId: getDataGuildRewards
      x-api-path-slug: dataguildrewards-get
      responses:
        200:
          description: OK
      tags:
      - Data
      - Guild
      - Rewards
  /data/guild/perks:
    get:
      summary: Get Data Guild Perks
      description: Provides a list of all guild perks.
      operationId: getDataGuildPerks
      x-api-path-slug: dataguildperks-get
      responses:
        200:
          description: OK
      tags:
      - Data
      - Guild
      - Perks
  /data/item/classes:
    get:
      summary: Get Data Item Classes
      description: Provides a list of item classes.
      operationId: getDataItemClasses
      x-api-path-slug: dataitemclasses-get
      responses:
        200:
          description: OK
      tags:
      - Data
      - Item
      - Classes