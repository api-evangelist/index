swagger: "2.0"
x-collection-name: Fitbit
x-complete: 1
info:
  title: Fitbit
  description: bring-fitbit-health-data-into-your-apps-including-user-activities-sleep-heart-glucose-and-blood-pressure-information-
  version: 1.0.0
host: api.fitbit.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/-{collection-path}apiSubscriptions.json:
    get:
      summary: Get User Collection Path Apisubscriptions.json
      description: Get a list of user's subscriptions for your application in the
        format requested.
      operationId: getUserCollectionPathApisubscriptions.json
      x-api-path-slug: usercollectionpathapisubscriptions-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - -collection-pathapiSubscriptions.json
  /user/-{collection-path}apiSubscriptions/{subscription-id}.json:
    delete:
      summary: Delete User Collection Path Apisubscriptions Subscription .json
      description: Delete a subscription for the user and get a response in the format
        requested.
      operationId: deleteUserCollectionPathApisubscriptionsSubscription.json
      x-api-path-slug: usercollectionpathapisubscriptionssubscriptionid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - -collection-pathapiSubscriptions
      - Subscription-id.json
    post:
      summary: Post User Collection Path Apisubscriptions Subscription .json
      description: Add a subscription for the user to get notifications and get a
        response in the format requested.
      operationId: postUserCollectionPathApisubscriptionsSubscription.json
      x-api-path-slug: usercollectionpathapisubscriptionssubscriptionid-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - -collection-pathapiSubscriptions
      - Subscription-id.json
  /user/-/friends/invitations.json:
    get:
      summary: Get User Friends Invitations.json
      description: Retrieve the list of invites to become freinds for a user in the
        format requested.
      operationId: getUserFriendsInvitations.json
      x-api-path-slug: userfriendsinvitations-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Friends
      - Invitations.json
  /foods/units.json:
    get:
      summary: Get Foods Units.json
      description: Get list of all valid Fitbit food units in the format requested.
      operationId: getFoodsUnits.json
      x-api-path-slug: foodsunits-json-get
      responses:
        200:
          description: OK
      tags:
      - Foods
      - Units.json
  /foods/{food-id}.json:
    get:
      summary: Get Foods Food .json
      description: Get the details of a specific food in Fitbit Food database (or
        private food for the user) in the format requested. Note, that nutritional
        values currently included in response only for the private foods.
      operationId: getFoodsFood.json
      x-api-path-slug: foodsfoodid-json-get
      responses:
        200:
          description: OK
      tags:
      - Foods
      - Food-id.json
  /activities/{id}.json:
    get:
      summary: Get Activities .json
      description: Get the details of a specific activity in Fitbit activities database
        in the format requested. If activity has levels, also get list of activity
        level details.
      operationId: getActivities.json
      x-api-path-slug: activitiesid-json-get
      responses:
        200:
          description: OK
      tags:
      - Activities
      - Id.json
  /activities.json:
    get:
      summary: Get Activities.json
      description: Get a tree of all valid Fitbit public activities from the activities
        catalog as well as private custom activities the user created in the format
        requested. If activity has levels, also get a list of activity level details.
      operationId: getActivities.json
      x-api-path-slug: activities-json-get
      responses:
        200:
          description: OK
      tags:
      - Activities.json
  /user/-/devices.json:
    get:
      summary: Get User Devices.json
      description: Retrieve the list of Fitbit devices for a user in the format requested.
      operationId: getUserDevices.json
      x-api-path-slug: userdevices-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Devices.json
  /user/-/foods/log/goal.json:
    post:
      summary: Post User Foods Log Goal.json
      description: Update (create) a user's daily calorie consumption goal or Food
        Plan and get a response in the format requested. Food Plan could not be created
        unless user already has active goal (Update-Weight-Goal). Depending on the
        weight goal setup only either MAINTENANCE (in case start weight is close to
        target weight or smaller) or one of the four other "lose" food plans could
        be created via intensity POST parameter.
      operationId: postUserFoodsLogGoal.json
      x-api-path-slug: userfoodsloggoal-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Goal.json
    get:
      summary: Get User Foods Log Goal.json
      description: Get a user's current daily calorie consumption goal and/or Food
        Plan in the format requested.
      operationId: getUserFoodsLogGoal.json
      x-api-path-slug: userfoodsloggoal-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Goal.json
  /user/-/meals.json:
    get:
      summary: Get User Meals.json
      description: Get a list of meals user created in his food log in the format
        requested.
      operationId: getUserMeals.json
      x-api-path-slug: usermeals-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Meals.json
  /foods.json:
    post:
      summary: Post Foods.json
      description: Create new private food for a user and get a response in a format
        requested. Created private food could be found in results of Search Foods
        call.
      operationId: postFoods.json
      x-api-path-slug: foods-json-post
      responses:
        200:
          description: OK
      tags:
      - Foods.json
  /user/-/foods/log/water/{water-log-id}.json:
    delete:
      summary: Delete User Foods Log Water Water Log .json
      description: Delete user's water log entry with the given id.
      operationId: deleteUserFoodsLogWaterWaterLog.json
      x-api-path-slug: userfoodslogwaterwaterlogid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Water
      - Water-log-id.json
  /user/-/foods/log/water.json:
    post:
      summary: Post User Foods Log Water.json
      description: Create log entry for a water using units in the unit system that
        corresponds to the Accept-Language header provided (or waterUnit) and get
        a response in the format requested.
      operationId: postUserFoodsLogWater.json
      x-api-path-slug: userfoodslogwater-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Water.json
  /user/-/foods/log/water/date/{date}.json:
    get:
      summary: Get User Foods Log Water Date Date .json
      description: Get a summary and list of a user's water log entries for a given
        day in the format requested using units in the unit system which corresponds
        to the Accept-Language header provided.
      operationId: getUserFoodsLogWaterDateDate.json
      x-api-path-slug: userfoodslogwaterdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Water
      - Date
      - Date.json
  /user/-/foods/log/favorite/{id}.json:
    delete:
      summary: Delete User Foods Log Favorite .json
      description: Delete the food with the given id from user's list of favorite
        foods.
      operationId: deleteUserFoodsLogFavorite.json
      x-api-path-slug: userfoodslogfavoriteid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Favorite
      - Id.json
    post:
      summary: Post User Foods Log Favorite .json
      description: Add the food with the given id to user's list of favorite foods.
      operationId: postUserFoodsLogFavorite.json
      x-api-path-slug: userfoodslogfavoriteid-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Favorite
      - Id.json
  /user/-/activities/goals/weekly.json:
    get:
      summary: Get User Activities Goals Weekly.json
      description: Get a user's current weekly activity goals in the format requested
        using units in the unit system which corresponds to the Accept-Language header
        provided.
      operationId: getUserActivitiesGoalsWeekly.json
      x-api-path-slug: useractivitiesgoalsweekly-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Activities
      - Goals
      - Weekly.json
  /user/-/activities/goals/daily.json:
    get:
      summary: Get User Activities Goals Daily.json
      description: Get a user's current daily activity goals in the format requested
        using units in the unit system which corresponds to the Accept-Language header
        provided.
      operationId: getUserActivitiesGoalsDaily.json
      x-api-path-slug: useractivitiesgoalsdaily-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Activities
      - Goals
      - Daily.json
  /user/-/activities/log/favorite/{id}.json:
    delete:
      summary: Delete User Activities Log Favorite .json
      description: Delete the activity with the given id from user's list of favorite
        activities.
      operationId: deleteUserActivitiesLogFavorite.json
      x-api-path-slug: useractivitieslogfavoriteid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Activities
      - Log
      - Favorite
      - Id.json
    post:
      summary: Post User Activities Log Favorite .json
      description: Adds the activity with the given id to user's list of favorite
        activities.
      operationId: postUserActivitiesLogFavorite.json
      x-api-path-slug: useractivitieslogfavoriteid-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Activities
      - Log
      - Favorite
      - Id.json
  /user/-/foods/log/favorite.json:
    get:
      summary: Get User Foods Log Favorite.json
      description: Get a list of a user's favorite foods in the format requested.
        A user marks a food as favorite on the user's Food Tab tab. A favorite food
        in the list provides a quick way to log the food via the Log Food endpoint.
      operationId: getUserFoodsLogFavorite.json
      x-api-path-slug: userfoodslogfavorite-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Favorite.json
  /user/-/foods/log/frequent.json:
    get:
      summary: Get User Foods Log Frequent.json
      description: Get a list of a user's frequent foods in the format requested.
        A frequent food in the list provides a quick way to log the food via the Log
        Food endpoint.
      operationId: getUserFoodsLogFrequent.json
      x-api-path-slug: userfoodslogfrequent-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Frequent.json
  /user/-/foods/log/recent.json:
    get:
      summary: Get User Foods Log Recent.json
      description: Get a list of a user's recent foods in the format requested. A
        recent food provides a quick way to log the food via the Log Food endpoint.
      operationId: getUserFoodsLogRecent.json
      x-api-path-slug: userfoodslogrecent-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Recent.json
  /user/-/activities/favorite.json:
    get:
      summary: Get User Activities Favorite.json
      description: Get a list of a user's favorite activities in the format requested.
        A user marks an activity as favorite on the user's Activities Tab. The activity
        ids in the list can be used to create a new activity log entry via the Log
        Activity.
      operationId: getUserActivitiesFavorite.json
      x-api-path-slug: useractivitiesfavorite-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Activities
      - Favorite.json
  /user/-/activities/frequent.json:
    get:
      summary: Get User Activities Frequent.json
      description: Get a list of a user's frequent activities in the format requested
        using units in the unit system which corresponds to the Accept-Language header
        provided. A frequent activity record contains the distance and duration values
        recorded the last time the activity was logged. The record retrieved can therefore
        be used to log the activity via the Log Activity with the same or adjusted
        values for distance and duration.
      operationId: getUserActivitiesFrequent.json
      x-api-path-slug: useractivitiesfrequent-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Activities
      - Frequent.json
  /user/-/activities/recent.json:
    get:
      summary: Get User Activities Recent.json
      description: Get a list of a user's recent activities in the format requested
        using units in the unit system which corresponds to the Accept-Language header
        provided. A recent activity record contains the distance and duration values
        recorded the last time the activity was logged. The record retrieved can therefore
        be used to log the activity via the Log Activity with the same or adjusted
        values for distance and duration.
      operationId: getUserActivitiesRecent.json
      x-api-path-slug: useractivitiesrecent-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Activities
      - Recent.json
  /user/{user-id}/sleep/minutesAsleep/date/{start-date-or-end-date}/{end-date-or-period}.json:
    get:
      summary: Get User User Sleep Minutesasleep Date Start Date Or End Date End Date
        Or Period .json
      description: Get time series in the specified range for a given resource in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserSleepMinutesasleepDateStartDateOrEndDateEndDateOrPeriod.json
      x-api-path-slug: useruseridsleepminutesasleepdatestartdateorenddateenddateorperiod-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Sleep
      - MinutesAsleep
      - Date
      - Start-date-or-end-date
      - End-date-or-period.json
  /user/{user-id}/foods/log/caloriesIn/date/{start-date-or-end-date}/{end-date-or-period}.json:
    get:
      summary: Get User User Foods Log Caloriesin Date Start Date Or End Date End
        Date Or Period .json
      description: Get time series in the specified range for a given resource in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserFoodsLogCaloriesinDateStartDateOrEndDateEndDateOrPeriod.json
      x-api-path-slug: useruseridfoodslogcaloriesindatestartdateorenddateenddateorperiod-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Foods
      - Log
      - CaloriesIn
      - Date
      - Start-date-or-end-date
      - End-date-or-period.json
  /user/-/body/log/fat/goal.json:
    post:
      summary: Post User Body Log Fat Goal.json
      description: Create or updates user's fat goal and get a response in the format
        requested.
      operationId: postUserBodyLogFatGoal.json
      x-api-path-slug: userbodylogfatgoal-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Fat
      - Goal.json
    get:
      summary: Get User Body Log Fat Goal.json
      description: Get a user's current fat goal in the format requested.
      operationId: getUserBodyLogFatGoal.json
      x-api-path-slug: userbodylogfatgoal-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Fat
      - Goal.json
  /user/-/body/log/weight/goal.json:
    post:
      summary: Post User Body Log Weight Goal.json
      description: Create or update user's weight goal using units in the unit system
        that corresponds to the Accept-Language header provided and get a response
        in the format requested.
      operationId: postUserBodyLogWeightGoal.json
      x-api-path-slug: userbodylogweightgoal-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Weight
      - Goal.json
    get:
      summary: Get User Body Log Weight Goal.json
      description: Get a user's current weight goal using units in the unit system
        that corresponds to the Accept-Language header provided in the format requested.
      operationId: getUserBodyLogWeightGoal.json
      x-api-path-slug: userbodylogweightgoal-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Weight
      - Goal.json
  /user/-/body/log/fat/{body-fat-log-id}.json:
    delete:
      summary: Delete User Body Log Fat Body Fat Log .json
      description: Delete user's body fat log entry with the given id.
      operationId: deleteUserBodyLogFatBodyFatLog.json
      x-api-path-slug: userbodylogfatbodyfatlogid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Fat
      - Body-fat-log-id.json
  /user/-/body/log/fat/{body-weight-log-id}.json:
    delete:
      summary: Delete User Body Log Fat Body Weight Log .json
      description: Delete user's body weight log entry with the given id.
      operationId: deleteUserBodyLogFatBodyWeightLog.json
      x-api-path-slug: userbodylogfatbodyweightlogid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Fat
      - Body-weight-log-id.json
  /user/-/body/log/fat.json:
    post:
      summary: Post User Body Log Fat.json
      description: Create log entry for a body fat and get a response in the format
        requested.
      operationId: postUserBodyLogFat.json
      x-api-path-slug: userbodylogfat-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Fat.json
  /user/-/body/log/weight.json:
    post:
      summary: Post User Body Log Weight.json
      description: Create log entry for a body weight using units in the unit system
        that corresponds to the Accept-Language header provided and get a response
        in the format requested.
      operationId: postUserBodyLogWeight.json
      x-api-path-slug: userbodylogweight-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Weight.json
  /user/-/body.json:
    post:
      summary: Post User Body.json
      description: Log body measurements using units in the unit system that corresponds
        to the Accept-Language header provided.
      operationId: postUserBody.json
      x-api-path-slug: userbody-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body.json
  /user/{user-id}/body/weight/date/{start-date-or-end-date}/{end-date-or-period}.json:
    get:
      summary: Get User User Body Weight Date Start Date Or End Date End Date Or Period
        .json
      description: Get time series in the specified range for a given resource in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserBodyWeightDateStartDateOrEndDateEndDateOrPeriod.json
      x-api-path-slug: useruseridbodyweightdatestartdateorenddateenddateorperiod-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Body
      - Weight
      - Date
      - Start-date-or-end-date
      - End-date-or-period.json
  /user/{user-id}/activities/calories/date/{start-date-or-end-date}/{end-date-or-period}.json:
    get:
      summary: Get User User Activities Calories Date Start Date Or End Date End Date
        Or Period .json
      description: Get time series in the specified range for a given resource in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserActivitiesCaloriesDateStartDateOrEndDateEndDateOrPeriod.json
      x-api-path-slug: useruseridactivitiescaloriesdatestartdateorenddateenddateorperiod-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Activities
      - Calories
      - Date
      - Start-date-or-end-date
      - End-date-or-period.json
  /user/-/bp/{bp-log-id}.json:
    delete:
      summary: Delete User Bp Bp Log .json
      description: Delete user's blood pressure log entry with the given id.
      operationId: deleteUserBpBpLog.json
      x-api-path-slug: userbpbplogid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Bp
      - Bp-log-id.json
  /user/-/heart/{heart-log-id}.json:
    delete:
      summary: Delete User Heart Heart Log .json
      description: Delete user's heart rate log entry with the given id.
      operationId: deleteUserHeartHeartLog.json
      x-api-path-slug: userheartheartlogid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Heart
      - Heart-log-id.json
  /user/-/sleep/{sleep-log-id}.json:
    delete:
      summary: Delete User Sleep Sleep Log .json
      description: Delete user's sleep log entry with the given id.
      operationId: deleteUserSleepSleepLog.json
      x-api-path-slug: usersleepsleeplogid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Sleep
      - Sleep-log-id.json
  /user/{user-id}/badges.json:
    get:
      summary: Get User User Badges.json
      description: Get user's badges in the format requested. Response includes all
        badges for the user as seen on the Fitbit website badge locker (both activity
        and weight related). We return weight and distance badges based on the user's
        unit profile preference as on the website.
      operationId: getUserUserBadges.json
      x-api-path-slug: useruseridbadges-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Badges.json
  /user/-/activities/{activity-log-id}.json:
    delete:
      summary: Delete User Activities Activity Log .json
      description: Delete user's activity log entry with the given id.
      operationId: deleteUserActivitiesActivityLog.json
      x-api-path-slug: useractivitiesactivitylogid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Activities
      - Activity-log-id.json
  /user/-/foods/log/{food-log-id}.json:
    delete:
      summary: Delete User Foods Log Food Log .json
      description: Delete the user's food log entry with the given id.
      operationId: deleteUserFoodsLogFoodLog.json
      x-api-path-slug: userfoodslogfoodlogid-json-delete
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log
      - Food-log-id.json
  /user/-/glucose.json:
    post:
      summary: Post User Glucose.json
      description: Create log entry for a blood glucose measurement and/or HbA1c using
        units in the unit system which corresponds to the Accept-Language header provided
        and get a response in the format requested.
      operationId: postUserGlucose.json
      x-api-path-slug: userglucose-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Glucose.json
  /user/-/bp.json:
    post:
      summary: Post User Bp.json
      description: Create log entry for a blood pressure measurement and get a response
        in the format requested.
      operationId: postUserBp.json
      x-api-path-slug: userbp-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Bp.json
  /user/-/heart.json:
    post:
      summary: Post User Heart.json
      description: Create log entry for a heart rate measurement and get a response
        in the format requested.
      operationId: postUserHeart.json
      x-api-path-slug: userheart-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Heart.json
  /user/-/sleep.json:
    post:
      summary: Post User Sleep.json
      description: Create log entry for a sleep and get a response in the format requested.
      operationId: postUserSleep.json
      x-api-path-slug: usersleep-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Sleep.json
  /user/-/foods/log.json:
    post:
      summary: Post User Foods Log.json
      description: Create log entry for a food. You need to select one of the unit
        ids to create a food log entry. It is possible to fetch unit ids allowed for
        specific food via previous calls to endpoints that retrieve food lists of
        the user. Each unit id maps to a unit in the list returned via the Get Food
        Units API call.
      operationId: postUserFoodsLog.json
      x-api-path-slug: userfoodslog-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Foods
      - Log.json
  /user/-/activities.json:
    get:
      summary: Get User Activities.json
      description: Get user's activity statistics in the format requested using units
        in the unit system which corresponds to the Accept-Language header provided.
        Response contains both lifetime statistics from the tracker device and total
        numbers including the manual activity log entries as seen on the Fitbit website
        dashboard.
      operationId: getUserActivities.json
      x-api-path-slug: useractivities-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Activities.json
    post:
      summary: Post User Activities.json
      description: Create log entry for an activity using units in the unit system
        which corresponds to the Accept-Language header provided (or using optional
        custom distanceUnit).
      operationId: postUserActivities.json
      x-api-path-slug: useractivities-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Activities.json
  /user/-/friends/leaderboard.json:
    get:
      summary: Get User Friends Leaderboard.json
      description: Get a leaderboard of user's friends progress in the format requested
        using units in the unit system which corresponds to the Accept-Language header
        provided. Authorized user himself is also included in the response.
      operationId: getUserFriendsLeaderboard.json
      x-api-path-slug: userfriendsleaderboard-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Friends
      - Leaderboard.json
  /user/{user-id}/friends.json:
    get:
      summary: Get User User Friends.json
      description: Get user's friends in the format requested using units in the unit
        system which corresponds to the Accept-Language header provided.
      operationId: getUserUserFriends.json
      x-api-path-slug: useruseridfriends-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Friends.json
  /user/-/glucose/date/{date}.json:
    get:
      summary: Get User Glucose Date Date .json
      description: Get a list of user's blood glucose and HbA1C measurements for a
        given day in the format requested using units in the unit system which corresponds
        to the Accept-Language header provided. Glucose measurement log entries are
        available only to authorized user. We always include all glucose trackers
        in the response body (with zero glucose value for the days with no measurements)
        to allow to seamlessly fetch a list of all additional user created custom
        trackers.
      operationId: getUserGlucoseDateDate.json
      x-api-path-slug: userglucosedatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Glucose
      - Date
      - Date.json
  /user/-/bp/date/{date}.json:
    get:
      summary: Get User Bp Date Date .json
      description: Get an average value and a list of user's blood pressure log entries
        for a given day in the format requested. Blood pressure log entries are available
        only to authorized user. Blood pressure log entries in response are sorted
        exactly the same as they are presented on the Fitbit website.
      operationId: getUserBpDateDate.json
      x-api-path-slug: userbpdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Bp
      - Date
      - Date.json
  /user/-/heart/date/{date}.json:
    get:
      summary: Get User Heart Date Date .json
      description: Get an average values and a list of user's heart rate log entries
        for a given day in the format requested. Heart rate data available only to
        the authorized user. Heart rate log entries in response are sorted exactly
        the same as they are presented on the Fitbit website. We always include all
        heart rate trackers in the "average" section of the response body (with zero
        average values for the days with no measurements) to allow to seamlessly fetch
        a list of all additional user created custom trackers.
      operationId: getUserHeartDateDate.json
      x-api-path-slug: userheartdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Heart
      - Date
      - Date.json
  /user/{user-id}/sleep/date/{date}.json:
    get:
      summary: Get User User Sleep Date Date .json
      description: Get a summary and list of a user's sleep log entries for a given
        day in the format requested. Endpoint returns summary for all sleep log entries
        for the given day (including naps). If you need data only for the main sleep
        you can fetch entry with "isMainSleep" = true or use Get-Time-Series calls.
      operationId: getUserUserSleepDateDate.json
      x-api-path-slug: useruseridsleepdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Sleep
      - Date
      - Date.json
  /user/{user-id}/foods/log/date/{date}.json:
    get:
      summary: Get User User Foods Log Date Date .json
      description: Get a summary and list of a user's food log entries for a given
        day in the format requested.
      operationId: getUserUserFoodsLogDateDate.json
      x-api-path-slug: useruseridfoodslogdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Foods
      - Log
      - Date
      - Date.json
  /user/{user-id}/activities/date/{date}.json:
    get:
      summary: Get User User Activities Date Date .json
      description: Get a summary and list of a user's activities and activity log
        entries for a given day in the format requested using units in the unit system
        which corresponds to the Accept-Language header provided.
      operationId: getUserUserActivitiesDateDate.json
      x-api-path-slug: useruseridactivitiesdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Activities
      - Date
      - Date.json
  /user/-/body/log/fat/date/{date}.json:
    get:
      summary: Get User Body Log Fat Date Date .json
      description: Get a list of all user's body fat log entries for a given day in
        the format requested.
      operationId: getUserBodyLogFatDateDate.json
      x-api-path-slug: userbodylogfatdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Fat
      - Date
      - Date.json
  /user/-/body/log/weight/date/{date}.json:
    get:
      summary: Get User Body Log Weight Date Date .json
      description: Get a list of all user's body weight log entries for a given day
        in the format requested using units in the unit system which corresponds to
        the Accept-Language header provided.
      operationId: getUserBodyLogWeightDateDate.json
      x-api-path-slug: userbodylogweightdatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Body
      - Log
      - Weight
      - Date
      - Date.json
  /user/{user-id}/body/date/{date}.json:
    get:
      summary: Get User User Body Date Date .json
      description: Get a summary of a user's body measurements for a given day in
        the format requested using units in the unit system which corresponds to the
        Accept-Language header provided.
      operationId: getUserUserBodyDateDate.json
      x-api-path-slug: useruseridbodydatedate-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Body
      - Date
      - Date.json
  /user/-/profile.json:
    post:
      summary: Post User Profile.json
      description: Update user's profile using units in the unit system that corresponds
        to the Accept-Language header provided and get a response in the format requested.
      operationId: postUserProfile.json
      x-api-path-slug: userprofile-json-post
      responses:
        200:
          description: OK
      tags:
      - User
      - '-'
      - Profile.json
  /user/{user-id}/profile.json:
    get:
      summary: Get User User Profile.json
      description: Get user's profile in the format requested using units in the unit
        system which corresponds to the Accept-Language header provided.
      operationId: getUserUserProfile.json
      x-api-path-slug: useruseridprofile-json-get
      responses:
        200:
          description: OK
      tags:
      - User
      - User-id
      - Profile.json