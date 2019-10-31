swagger: "2.0"
x-collection-name: Pivotal Tracker
x-complete: 1
info:
  title: Pivotal Tracker
  description: access-and-manipulate-agile-project-management-data-including-projects-stories-and-tasks-
  version: 1.0.0
host: www.pivotaltracker.com
basePath: /services/v3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tokens/active:
    get:
      summary: Get Tokens Active
      description: Returns an API token associated with the user. This method requires
        HTTP Basic authentication.
      operationId: getTokensActive
      x-api-path-slug: tokensactive-get
      responses:
        200:
          description: OK
      tags:
      - Tokens
      - Active
    post:
      summary: Post Tokens Active
      description: Returns an API token associated with the user.
      operationId: postTokensActive
      x-api-path-slug: tokensactive-post
      parameters:
      - in: query
        name: password
        description: The users password
      - in: query
        name: username
        description: The users name
      responses:
        200:
          description: OK
      tags:
      - Tokens
      - Active
  /activities:
    get:
      summary: Get Activities
      description: Retrieves the recent activity of all your projects.
      operationId: getActivities
      x-api-path-slug: activities-get
      parameters:
      - in: query
        name: limit
        description: Limits the number of activity feed items
      - in: query
        name: newer_than_version
        description: Restricts the activity feed to only those items that have a greater
          than supplied version
      - in: query
        name: occurred_since_date
        description: 'Restricts the activity feed to only those items that occurred
          after a supplied date (example format: 2009/12/18 21:00:00 UTC)'
      responses:
        200:
          description: OK
      tags:
      - Activities
  /projects/{PROJECT_ID}/activities:
    get:
      summary: Get Projects Project Activities
      description: Retrieves the recent activity of a specific project.
      operationId: getProjectsProjectActivities
      x-api-path-slug: projectsproject-idactivities-get
      parameters:
      - in: query
        name: limit
        description: Limits the number of activity feed items
      - in: query
        name: occurred_since_date
        description: 'Restricts the activity feed to only those items that occurred
          after a supplied date (example format: 2009/12/18 21:00:00 UTC)'
      - in: path
        name: PROJECT_ID
        description: The ID of the project to retrieve the activity for
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Activities
  /projects/{PROJECT_ID}:
    get:
      summary: Get Projects Project
      description: Retrieves information about a project.
      operationId: getProjectsProject
      x-api-path-slug: projectsproject-id-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project to retrieve
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
  /projects:
    get:
      summary: Get Projects
      description: Retrieves all of the user's projects.
      operationId: getProjects
      x-api-path-slug: projects-get
      responses:
        200:
          description: OK
      tags:
      - Projects
    post:
      summary: Post Projects
      description: Adds a new project.
      operationId: postProjects
      x-api-path-slug: projects-post
      responses:
        200:
          description: OK
      tags:
      - Projects
  /projects/{PROJECT_ID}/memberships:
    get:
      summary: Get Projects Project Memberships
      description: Retrieves all memberships for a project.
      operationId: getProjectsProjectMemberships
      x-api-path-slug: projectsproject-idmemberships-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Memberships
    post:
      summary: Post Projects Project Memberships
      description: Adds a new membership to a project.
      operationId: postProjectsProjectMemberships
      x-api-path-slug: projectsproject-idmemberships-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Memberships
  /projects/{PROJECT_ID}/memberships/{MEMBERSHIP_ID}:
    get:
      summary: Get Projects Project Memberships Membership
      description: Retrieves information about a single membership.
      operationId: getProjectsProjectMembershipsMembership
      x-api-path-slug: projectsproject-idmembershipsmembership-id-get
      parameters:
      - in: path
        name: MEMBERSHIP_ID
        description: The ID of the membership
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Memberships
      - MEMBERSHIP
      - ID
    delete:
      summary: Delete Projects Project Memberships Membership
      description: Delete projects project memberships membership.
      operationId: deleteProjectsProjectMembershipsMembership
      x-api-path-slug: projectsproject-idmembershipsmembership-id-delete
      parameters:
      - in: path
        name: MEMBERSHIP_ID
        description: The ID of the membership
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Memberships
      - MEMBERSHIP
      - ID
  /projects/{PROJECT_ID}/iterations:
    get:
      summary: Get Projects Project Iterations
      description: Retrieves all iterations, with stories.
      operationId: getProjectsProjectIterations
      x-api-path-slug: projectsproject-iditerations-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Iterations
  /projects/{PROJECT_ID}/iterations/done:
    get:
      summary: Get Projects Project Iterations Done
      description: Retrieves iterations from the "done" group, with stories.
      operationId: getProjectsProjectIterationsDone
      x-api-path-slug: projectsproject-iditerationsdone-get
      parameters:
      - in: query
        name: limit
        description: Controls the maximum number of iterations returned
      - in: query
        name: offset
        description: Controls the number of iterations to skip from the beginning
          of the result
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Iterations
      - Done
  /projects/{PROJECT_ID}/iterations/current:
    get:
      summary: Get Projects Project Iterations Current
      description: Retrieves iterations from the "current" group, with stories.
      operationId: getProjectsProjectIterationsCurrent
      x-api-path-slug: projectsproject-iditerationscurrent-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Iterations
      - Current
  /projects/{PROJECT_ID}/iterations/backlog:
    get:
      summary: Get Projects Project Iterations Backlog
      description: Retrieves iterations from the "backlog" group, with stories.
      operationId: getProjectsProjectIterationsBacklog
      x-api-path-slug: projectsproject-iditerationsbacklog-get
      parameters:
      - in: query
        name: limit
        description: Controls the maximum number of iterations returned
      - in: query
        name: offset
        description: Controls the number of iterations to skip from the beginning
          of the result
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Iterations
      - Backlog
  /projects/{PROJECT_ID}/iterations/current_backlog:
    get:
      summary: Get Projects Project Iterations Current Backlog
      description: Retrieves iterations from the "current" and "backlog" groups, with
        stories.
      operationId: getProjectsProjectIterationsCurrentBacklog
      x-api-path-slug: projectsproject-iditerationscurrent-backlog-get
      parameters:
      - in: query
        name: limit
        description: Controls the maximum number of iterations returned
      - in: query
        name: offset
        description: Controls the number of iterations to skip from the beginning
          of the result
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Iterations
      - Current
      - Backlog
  /projects/{PROJECT_ID}/stories/{STORY_ID}:
    get:
      summary: Get Projects Project Stories Story
      description: Retrieves information about a single story.
      operationId: getProjectsProjectStoriesStory
      x-api-path-slug: projectsproject-idstoriesstory-id-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
    put:
      summary: Put Projects Project Stories Story
      description: Put projects project stories story.
      operationId: putProjectsProjectStoriesStory
      x-api-path-slug: projectsproject-idstoriesstory-id-put
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
    delete:
      summary: Delete Projects Project Stories Story
      description: Delete projects project stories story.
      operationId: deleteProjectsProjectStoriesStory
      x-api-path-slug: projectsproject-idstoriesstory-id-delete
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
  /projects/{PROJECT_ID}/stories:
    get:
      summary: Get Projects Project Stories
      description: Retrieves all stories for a project, or those matching filter(s)
      operationId: getProjectsProjectStories
      x-api-path-slug: projectsproject-idstories-get
      parameters:
      - in: query
        name: filter
        description: A filter for the returned stories to match
      - in: query
        name: limit
        description: Controls the maximum number of stories returned
      - in: query
        name: offset
        description: Controls the number of stories to skip from the beginning of
          the result
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
    post:
      summary: Post Projects Project Stories
      description: Post projects project stories.
      operationId: postProjectsProjectStories
      x-api-path-slug: projectsproject-idstories-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
  /projects/{PROJECT_ID}/stories/{STORY_ID}/notes:
    put:
      summary: Put Projects Project Stories Story Notes
      description: Put projects project stories story notes.
      operationId: putProjectsProjectStoriesStoryNotes
      x-api-path-slug: projectsproject-idstoriesstory-idnotes-put
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Notes
  /projects/{PROJECT_ID}/stories/deliver_all_finished:
    post:
      summary: Post Projects Project Stories Deliver All Finished
      description: Takes all finished stories and marks them as delivered. This could
        be used to automate a demo deploy process. The updated stories are returned
        as the result.
      operationId: postProjectsProjectStoriesDeliverAllFinished
      x-api-path-slug: projectsproject-idstoriesdeliver-all-finished-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - Deliver
      - ""
      - Finished
  /projects/{PROJECT_ID}/stories/{STORY_ID}/moves:
    post:
      summary: Post Projects Project Stories Story Moves
      description: Moves a story before or after another story. The moved story is
        returned in the response.
      operationId: postProjectsProjectStoriesStoryMoves
      x-api-path-slug: projectsproject-idstoriesstory-idmoves-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Moves
  /projects/{PROJECT_ID}/stories/{STORY_ID}/tasks/{TASK_ID}:
    get:
      summary: Get Projects Project Stories Story Tasks Task
      description: Get projects project stories story tasks task.
      operationId: getProjectsProjectStoriesStoryTasksTask
      x-api-path-slug: projectsproject-idstoriesstory-idtaskstask-id-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      - in: path
        name: TASK_ID
        description: The ID of the task
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
      - TASK
      - ID
    put:
      summary: Put Projects Project Stories Story Tasks Task
      description: Put projects project stories story tasks task.
      operationId: putProjectsProjectStoriesStoryTasksTask
      x-api-path-slug: projectsproject-idstoriesstory-idtaskstask-id-put
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      - in: path
        name: TASK_ID
        description: The ID of the task
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
      - TASK
      - ID
    delete:
      summary: Delete Projects Project Stories Story Tasks Task
      description: Delete projects project stories story tasks task.
      operationId: deleteProjectsProjectStoriesStoryTasksTask
      x-api-path-slug: projectsproject-idstoriesstory-idtaskstask-id-delete
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      - in: path
        name: TASK_ID
        description: The ID of the task
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
      - TASK
      - ID
  /projects/{PROJECT_ID}/stories/{STORY_ID}/tasks:
    get:
      summary: Get Projects Project Stories Story Tasks
      description: Get projects project stories story tasks.
      operationId: getProjectsProjectStoriesStoryTasks
      x-api-path-slug: projectsproject-idstoriesstory-idtasks-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
    post:
      summary: Post Projects Project Stories Story Tasks
      description: Post projects project stories story tasks.
      operationId: postProjectsProjectStoriesStoryTasks
      x-api-path-slug: projectsproject-idstoriesstory-idtasks-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
  /projects/{PROJECT_ID}/stories/{STORY_ID}/attachments:
    post:
      summary: Post Projects Project Stories Story Attachments
      description: Post projects project stories story attachments.
      operationId: postProjectsProjectStoriesStoryAttachments
      x-api-path-slug: projectsproject-idstoriesstory-idattachments-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Attachments
  /source_commits:
    post:
      summary: Post Source Commits
      description: Allows integration with post-commit hooks of Source Control Management
        (SCM) systems such as Subversion, Git, etc.
      operationId: postSourceCommits
      x-api-path-slug: source-commits-post
      responses:
        200:
          description: OK
      tags:
      - Source
      - Commits