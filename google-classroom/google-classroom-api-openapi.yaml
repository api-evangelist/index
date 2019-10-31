swagger: "2.0"
x-collection-name: Google Classroom
x-complete: 1
info:
  title: Google Classroom
  description: manages-classes-rosters-and-invitations-in-google-classroom-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: classroom.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/courses:
    get:
      summary: Get Courses
      description: |-
        Returns a list of courses that the requesting user is permitted to view,
        restricted to those that match the request.

        This method returns the following error codes:

        * `PERMISSION_DENIED` for access errors.
        * `INVALID_ARGUMENT` if the query argument is malformed.
        * `NOT_FOUND` if any users specified in the query arguments do not exist.
      operationId: classroom.courses.list
      x-api-path-slug: v1courses-get
      parameters:
      - in: query
        name: courseStates
        description: Restricts returned courses to those in one of the specified statesThe
          default value is ACTIVE, ARCHIVED, PROVISIONED, DECLINED
      - in: query
        name: pageSize
        description: Maximum number of items to return
      - in: query
        name: pageToken
        description: nextPageTokenvalue returned from a previouslist call,indicating
          that the subsequent page of results should be returned
      - in: query
        name: studentId
        description: Restricts returned courses to those having a student with the
          specifiedidentifier
      - in: query
        name: teacherId
        description: Restricts returned courses to those having a teacher with the
          specifiedidentifier
      responses:
        200:
          description: OK
      tags:
      - Course
    post:
      summary: Create Course
      description: |-
        Creates a course.

        The user specified in `ownerId` is the owner of the created course
        and added as a teacher.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to create
        courses or for access errors.
        * `NOT_FOUND` if the primary teacher is not a valid user.
        * `FAILED_PRECONDITION` if the course owner's account is disabled or for
        the following request errors:
            * UserGroupsMembershipLimitReached
        * `ALREADY_EXISTS` if an alias was specified in the `id` and
        already exists.
      operationId: classroom.courses.create
      x-api-path-slug: v1courses-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Course
  /v1/courses/{courseId}/aliases:
    get:
      summary: Get Aliases
      description: |-
        Returns a list of aliases for a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        course or for access errors.
        * `NOT_FOUND` if the course does not exist.
      operationId: classroom.courses.aliases.list
      x-api-path-slug: v1coursescourseidaliases-get
      parameters:
      - in: path
        name: courseId
        description: The identifier of the course
      - in: query
        name: pageSize
        description: Maximum number of items to return
      - in: query
        name: pageToken
        description: nextPageTokenvalue returned from a previouslist call,indicating
          that the subsequent page of results should be returned
      responses:
        200:
          description: OK
      tags:
      - Alias
    post:
      summary: Create Alias
      description: |-
        Creates an alias for a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to create the
        alias or for access errors.
        * `NOT_FOUND` if the course does not exist.
        * `ALREADY_EXISTS` if the alias already exists.
        * `FAILED_PRECONDITION` if the alias requested does not make sense for the
          requesting user or course (for example, if a user not in a domain
          attempts to access a domain-scoped alias).
      operationId: classroom.courses.aliases.create
      x-api-path-slug: v1coursescourseidaliases-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: courseId
        description: Identifier of the course to alias
      responses:
        200:
          description: OK
      tags:
      - Alias
  /v1/courses/{courseId}/aliases/{alias}:
    delete:
      summary: Delete Alias
      description: |-
        Deletes an alias of a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to remove the
        alias or for access errors.
        * `NOT_FOUND` if the alias does not exist.
        * `FAILED_PRECONDITION` if the alias requested does not make sense for the
          requesting user or course (for example, if a user not in a domain
          attempts to delete a domain-scoped alias).
      operationId: classroom.courses.aliases.delete
      x-api-path-slug: v1coursescourseidaliasesalias-delete
      parameters:
      - in: path
        name: alias
        description: Alias to delete
      - in: path
        name: courseId
        description: Identifier of the course whose alias should be deleted
      responses:
        200:
          description: OK
      tags:
      - Alias
  /v1/courses/{courseId}/courseWork:
    get:
      summary: Get Course Work
      description: |-
        Returns a list of course work that the requester is permitted to view.

        Course students may only view `PUBLISHED` course work. Course teachers
        and domain administrators may view all course work.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access
        the requested course or for access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course does not exist.
      operationId: classroom.courses.courseWork.list
      x-api-path-slug: v1coursescourseidcoursework-get
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: query
        name: courseWorkStates
        description: Restriction on the work status to return
      - in: query
        name: orderBy
        description: Optional sort ordering for results
      - in: query
        name: pageSize
        description: Maximum number of items to return
      - in: query
        name: pageToken
        description: nextPageTokenvalue returned from a previouslist call,indicating
          that the subsequent page of results should be returned
      responses:
        200:
          description: OK
      tags:
      - Alias
    post:
      summary: Create Course Work
      description: |-
        Creates course work.

        The resulting course work (and corresponding student submissions) are
        associated with the Developer Console project of the
        [OAuth client ID](https://support.google.com/cloud/answer/6158849) used to
        make the request. Classroom API requests to modify course work and student
        submissions must be made with an OAuth client ID from the associated
        Developer Console project.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        requested course, create course work in the requested course, share a
        Drive attachment, or for access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course does not exist.
        * `FAILED_PRECONDITION` for the following request error:
            * AttachmentNotVisible
      operationId: classroom.courses.courseWork.create
      x-api-path-slug: v1coursescourseidcoursework-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: courseId
        description: Identifier of the course
      responses:
        200:
          description: OK
      tags:
      - Course Work
  /v1/courses/{courseId}/courseWork/{courseWorkId}/studentSubmissions:
    get:
      summary: Get Student Submissions
      description: |-
        Returns a list of student submissions that the requester is permitted to
        view, factoring in the OAuth scopes of the request.
        `-` may be specified as the `course_work_id` to include student
        submissions for multiple course work items.

        Course students may only view their own work. Course teachers
        and domain administrators may view all student submissions.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        requested course or course work, or for access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course does not exist.
      operationId: classroom.courses.courseWork.studentSubmissions.list
      x-api-path-slug: v1coursescourseidcourseworkcourseworkidstudentsubmissions-get
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: courseWorkId
        description: Identifer of the student work to request
      - in: query
        name: late
        description: Requested lateness value
      - in: query
        name: pageSize
        description: Maximum number of items to return
      - in: query
        name: pageToken
        description: nextPageTokenvalue returned from a previouslist call,indicating
          that the subsequent page of results should be returned
      - in: query
        name: states
        description: Requested submission states
      - in: query
        name: userId
        description: Optional argument to restrict returned student work to those
          owned by thestudent with the specified identifier
      responses:
        200:
          description: OK
      tags:
      - Student Submission
  /v1/courses/{courseId}/courseWork/{courseWorkId}/studentSubmissions/{id}:
    get:
      summary: Get Student Submission
      description: |-
        Returns a student submission.

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        requested course, course work, or student submission or for
        access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course, course work, or student submission
        does not exist.
      operationId: classroom.courses.courseWork.studentSubmissions.get
      x-api-path-slug: v1coursescourseidcourseworkcourseworkidstudentsubmissionsid-get
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: courseWorkId
        description: Identifier of the course work
      - in: path
        name: id
        description: Identifier of the student submission
      responses:
        200:
          description: OK
      tags:
      - Student Submission
    patch:
      summary: Update Fields
      description: |-
        Updates one or more fields of a student submission.

        See google.classroom.v1.StudentSubmission for details
        of which fields may be updated and who may change them.

        This request must be made by the Developer Console project of the
        [OAuth client ID](https://support.google.com/cloud/answer/6158849) used to
        create the corresponding course work item.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting developer project did not create
        the corresponding course work, if the user is not permitted to make the
        requested modification to the student submission, or for
        access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course, course work, or student submission
        does not exist.
      operationId: classroom.courses.courseWork.studentSubmissions.patch
      x-api-path-slug: v1coursescourseidcourseworkcourseworkidstudentsubmissionsid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: courseWorkId
        description: Identifier of the course work
      - in: path
        name: id
        description: Identifier of the student submission
      - in: query
        name: updateMask
        description: Mask that identifies which fields on the student submission to
          update
      responses:
        200:
          description: OK
      tags:
      - Field
  /v1/courses/{courseId}/courseWork/{courseWorkId}/studentSubmissions/{id}:modifyAttachments:
    post:
      summary: Modify Attachments
      description: |-
        Modifies attachments of student submission.

        Attachments may only be added to student submissions belonging to course
        work objects with a `workType` of `ASSIGNMENT`.

        This request must be made by the Developer Console project of the
        [OAuth client ID](https://support.google.com/cloud/answer/6158849) used to
        create the corresponding course work item.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        requested course or course work, if the user is not permitted to modify
        attachments on the requested student submission, or for
        access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course, course work, or student submission
        does not exist.
      operationId: classroom.courses.courseWork.studentSubmissions.modifyAttachments
      x-api-path-slug: v1coursescourseidcourseworkcourseworkidstudentsubmissionsidmodifyattachments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: courseWorkId
        description: Identifier of the course work
      - in: path
        name: id
        description: Identifier of the student submission
      responses:
        200:
          description: OK
      tags:
      - Attachment
  /v1/courses/{courseId}/courseWork/{courseWorkId}/studentSubmissions/{id}:reclaim:
    post:
      summary: Reclaim Student Submission
      description: |-
        Reclaims a student submission on behalf of the student that owns it.

        Reclaiming a student submission transfers ownership of attached Drive
        files to the student and update the submission state.

        Only the student that owns the requested student submission may call this
        method, and only for a student submission that has been turned in.

        This request must be made by the Developer Console project of the
        [OAuth client ID](https://support.google.com/cloud/answer/6158849) used to
        create the corresponding course work item.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        requested course or course work, unsubmit the requested student submission,
        or for access errors.
        * `FAILED_PRECONDITION` if the student submission has not been turned in.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course, course work, or student submission
        does not exist.
      operationId: classroom.courses.courseWork.studentSubmissions.reclaim
      x-api-path-slug: v1coursescourseidcourseworkcourseworkidstudentsubmissionsidreclaim-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: courseWorkId
        description: Identifier of the course work
      - in: path
        name: id
        description: Identifier of the student submission
      responses:
        200:
          description: OK
      tags:
      - Student Submission
  /v1/courses/{courseId}/courseWork/{courseWorkId}/studentSubmissions/{id}:return:
    post:
      summary: Get Student Submission
      description: |-
        Returns a student submission.

        Returning a student submission transfers ownership of attached Drive
        files to the student and may also update the submission state.
        Unlike the Classroom application, returning a student submission does not
        set assignedGrade to the draftGrade value.

        Only a teacher of the course that contains the requested student submission
        may call this method.

        This request must be made by the Developer Console project of the
        [OAuth client ID](https://support.google.com/cloud/answer/6158849) used to
        create the corresponding course work item.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        requested course or course work, return the requested student submission,
        or for access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course, course work, or student submission
        does not exist.
      operationId: classroom.courses.courseWork.studentSubmissions.return
      x-api-path-slug: v1coursescourseidcourseworkcourseworkidstudentsubmissionsidreturn-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: courseWorkId
        description: Identifier of the course work
      - in: path
        name: id
        description: Identifier of the student submission
      responses:
        200:
          description: OK
      tags:
      - Student Submission
  /v1/courses/{courseId}/courseWork/{courseWorkId}/studentSubmissions/{id}:turnIn:
    post:
      summary: Turn in Student Submission
      description: |-
        Turns in a student submission.

        Turning in a student submission transfers ownership of attached Drive
        files to the teacher and may also update the submission state.

        This may only be called by the student that owns the specified student
        submission.

        This request must be made by the Developer Console project of the
        [OAuth client ID](https://support.google.com/cloud/answer/6158849) used to
        create the corresponding course work item.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        requested course or course work, turn in the requested student submission,
        or for access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course, course work, or student submission
        does not exist.
      operationId: classroom.courses.courseWork.studentSubmissions.turnIn
      x-api-path-slug: v1coursescourseidcourseworkcourseworkidstudentsubmissionsidturnin-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: courseWorkId
        description: Identifier of the course work
      - in: path
        name: id
        description: Identifier of the student submission
      responses:
        200:
          description: OK
      tags:
      - Student Submission
  /v1/courses/{courseId}/courseWork/{id}:
    delete:
      summary: Delete Course Work
      description: |-
        Deletes a course work.

        This request must be made by the Developer Console project of the
        [OAuth client ID](https://support.google.com/cloud/answer/6158849) used to
        create the corresponding course work item.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting developer project did not create
        the corresponding course work, if the requesting user is not permitted
        to delete the requested course or for access errors.
        * `FAILED_PRECONDITION` if the requested course work has already been
        deleted.
        * `NOT_FOUND` if no course exists with the requested ID.
      operationId: classroom.courses.courseWork.delete
      x-api-path-slug: v1coursescourseidcourseworkid-delete
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: id
        description: Identifier of the course work to delete
      responses:
        200:
          description: OK
      tags:
      - Course Work
    get:
      summary: Get Course Work
      description: |-
        Returns course work.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        requested course or course work, or for access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `NOT_FOUND` if the requested course or course work does not exist.
      operationId: classroom.courses.courseWork.get
      x-api-path-slug: v1coursescourseidcourseworkid-get
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: id
        description: Identifier of the course work
      responses:
        200:
          description: OK
      tags:
      - Course Work
    patch:
      summary: Update Fields
      description: |-
        Updates one or more fields of a course work.

        See google.classroom.v1.CourseWork for details
        of which fields may be updated and who may change them.

        This request must be made by the Developer Console project of the
        [OAuth client ID](https://support.google.com/cloud/answer/6158849) used to
        create the corresponding course work item.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting developer project did not create
        the corresponding course work, if the user is not permitted to make the
        requested modification to the student submission, or for
        access errors.
        * `INVALID_ARGUMENT` if the request is malformed.
        * `FAILED_PRECONDITION` if the requested course work has already been
        deleted.
        * `NOT_FOUND` if the requested course, course work, or student submission
        does not exist.
      operationId: classroom.courses.courseWork.patch
      x-api-path-slug: v1coursescourseidcourseworkid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: id
        description: Identifier of the course work
      - in: query
        name: updateMask
        description: Mask that identifies which fields on the course work to update
      responses:
        200:
          description: OK
      tags:
      - Field
  /v1/courses/{courseId}/students:
    get:
      summary: Get Students
      description: |-
        Returns a list of students of this course that the requester
        is permitted to view.

        This method returns the following error codes:

        * `NOT_FOUND` if the course does not exist.
        * `PERMISSION_DENIED` for access errors.
      operationId: classroom.courses.students.list
      x-api-path-slug: v1coursescourseidstudents-get
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: query
        name: pageSize
        description: Maximum number of items to return
      - in: query
        name: pageToken
        description: nextPageTokenvalue returned from a previouslist call, indicating
          thatthe subsequent page of results should be returned
      responses:
        200:
          description: OK
      tags:
      - Student
    post:
      summary: Add Student
      description: |-
        Adds a user as a student of a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to create
        students in this course or for access errors.
        * `NOT_FOUND` if the requested course ID does not exist.
        * `FAILED_PRECONDITION` if the requested user's account is disabled,
        for the following request errors:
            * CourseMemberLimitReached
            * CourseNotModifiable
            * UserGroupsMembershipLimitReached
        * `ALREADY_EXISTS` if the user is already a student or teacher in the
        course.
      operationId: classroom.courses.students.create
      x-api-path-slug: v1coursescourseidstudents-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: courseId
        description: Identifier of the course to create the student in
      - in: query
        name: enrollmentCode
        description: Enrollment code of the course to create the student in
      responses:
        200:
          description: OK
      tags:
      - Student
  /v1/courses/{courseId}/students/{userId}:
    delete:
      summary: Delete Student
      description: |-
        Deletes a student of a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to delete
        students of this course or for access errors.
        * `NOT_FOUND` if no student of this course has the requested ID or if the
        course does not exist.
      operationId: classroom.courses.students.delete
      x-api-path-slug: v1coursescourseidstudentsuserid-delete
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: userId
        description: Identifier of the student to delete
      responses:
        200:
          description: OK
      tags:
      - Student
    get:
      summary: Get Student
      description: |-
        Returns a student of a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to view
        students of this course or for access errors.
        * `NOT_FOUND` if no student of this course has the requested ID or if the
        course does not exist.
      operationId: classroom.courses.students.get
      x-api-path-slug: v1coursescourseidstudentsuserid-get
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: userId
        description: Identifier of the student to return
      responses:
        200:
          description: OK
      tags:
      - Student
  /v1/courses/{courseId}/teachers:
    get:
      summary: Get Teachers
      description: |-
        Returns a list of teachers of this course that the requester
        is permitted to view.

        This method returns the following error codes:

        * `NOT_FOUND` if the course does not exist.
        * `PERMISSION_DENIED` for access errors.
      operationId: classroom.courses.teachers.list
      x-api-path-slug: v1coursescourseidteachers-get
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: query
        name: pageSize
        description: Maximum number of items to return
      - in: query
        name: pageToken
        description: nextPageTokenvalue returned from a previouslist call, indicating
          thatthe subsequent page of results should be returned
      responses:
        200:
          description: OK
      tags:
      - Teacher
    post:
      summary: Create Teacher
      description: |-
        Creates a teacher of a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not  permitted to create
        teachers in this course or for access errors.
        * `NOT_FOUND` if the requested course ID does not exist.
        * `FAILED_PRECONDITION` if the requested user's account is disabled,
        for the following request errors:
            * CourseMemberLimitReached
            * CourseNotModifiable
            * CourseTeacherLimitReached
            * UserGroupsMembershipLimitReached
        * `ALREADY_EXISTS` if the user is already a teacher or student in the
        course.
      operationId: classroom.courses.teachers.create
      x-api-path-slug: v1coursescourseidteachers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: courseId
        description: Identifier of the course
      responses:
        200:
          description: OK
      tags:
      - Teacher
  /v1/courses/{courseId}/teachers/{userId}:
    delete:
      summary: Delete Teacher
      description: |-
        Deletes a teacher of a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to delete
        teachers of this course or for access errors.
        * `NOT_FOUND` if no teacher of this course has the requested ID or if the
        course does not exist.
        * `FAILED_PRECONDITION` if the requested ID belongs to the primary teacher
        of this course.
      operationId: classroom.courses.teachers.delete
      x-api-path-slug: v1coursescourseidteachersuserid-delete
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: userId
        description: Identifier of the teacher to delete
      responses:
        200:
          description: OK
      tags:
      - Teacher
    get:
      summary: Get Teacher
      description: |-
        Returns a teacher of a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to view
        teachers of this course or for access errors.
        * `NOT_FOUND` if no teacher of this course has the requested ID or if the
        course does not exist.
      operationId: classroom.courses.teachers.get
      x-api-path-slug: v1coursescourseidteachersuserid-get
      parameters:
      - in: path
        name: courseId
        description: Identifier of the course
      - in: path
        name: userId
        description: Identifier of the teacher to return
      responses:
        200:
          description: OK
      tags:
      - Teacher
  /v1/courses/{id}:
    delete:
      summary: Delete Course
      description: |-
        Deletes a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to delete the
        requested course or for access errors.
        * `NOT_FOUND` if no course exists with the requested ID.
      operationId: classroom.courses.delete
      x-api-path-slug: v1coursesid-delete
      parameters:
      - in: path
        name: id
        description: Identifier of the course to delete
      responses:
        200:
          description: OK
      tags:
      - Course
    get:
      summary: Get Course
      description: |-
        Returns a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access the
        requested course or for access errors.
        * `NOT_FOUND` if no course exists with the requested ID.
      operationId: classroom.courses.get
      x-api-path-slug: v1coursesid-get
      parameters:
      - in: path
        name: id
        description: Identifier of the course to return
      responses:
        200:
          description: OK
      tags:
      - Course
    patch:
      summary: Update Fields
      description: |-
        Updates one or more fields in a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to modify the
        requested course or for access errors.
        * `NOT_FOUND` if no course exists with the requested ID.
        * `INVALID_ARGUMENT` if invalid fields are specified in the update mask or
        if no update mask is supplied.
        * `FAILED_PRECONDITION` for the following request errors:
            * CourseNotModifiable
      operationId: classroom.courses.patch
      x-api-path-slug: v1coursesid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Identifier of the course to update
      - in: query
        name: updateMask
        description: Mask that identifies which fields on the course to update
      responses:
        200:
          description: OK
      tags:
      - Field
    put:
      summary: Update Course
      description: |-
        Updates a course.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to modify the
        requested course or for access errors.
        * `NOT_FOUND` if no course exists with the requested ID.
        * `FAILED_PRECONDITION` for the following request errors:
            * CourseNotModifiable
      operationId: classroom.courses.update
      x-api-path-slug: v1coursesid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Identifier of the course to update
      responses:
        200:
          description: OK
      tags:
      - Course
  /v1/invitations:
    get:
      summary: Get Invitations
      description: |-
        Returns a list of invitations that the requesting user is permitted to
        view, restricted to those that match the list request.

        *Note:* At least one of `user_id` or `course_id` must be supplied. Both
        fields can be supplied.

        This method returns the following error codes:

        * `PERMISSION_DENIED` for access errors.
      operationId: classroom.invitations.list
      x-api-path-slug: v1invitations-get
      parameters:
      - in: query
        name: courseId
        description: Restricts returned invitations to those for a course with the
          specifiedidentifier
      - in: query
        name: pageSize
        description: Maximum number of items to return
      - in: query
        name: pageToken
        description: nextPageTokenvalue returned from a previouslist call, indicatingthat
          the subsequent page of results should be returned
      - in: query
        name: userId
        description: Restricts returned invitations to those for a specific user
      responses:
        200:
          description: OK
      tags:
      - Invitation
    post:
      summary: Create Invitation
      description: |-
        Creates an invitation. Only one invitation for a user and course may exist
        at a time. Delete and re-create an invitation to make changes.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to create
        invitations for this course or for access errors.
        * `NOT_FOUND` if the course or the user does not exist.
        * `FAILED_PRECONDITION` if the requested user's account is disabled or if
        the user already has this role or a role with greater permissions.
        * `ALREADY_EXISTS` if an invitation for the specified user and course
        already exists.
      operationId: classroom.invitations.create
      x-api-path-slug: v1invitations-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Invitation
  /v1/invitations/{id}:
    delete:
      summary: Delete Invitation
      description: |-
        Deletes an invitation.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to delete the
        requested invitation or for access errors.
        * `NOT_FOUND` if no invitation exists with the requested ID.
      operationId: classroom.invitations.delete
      x-api-path-slug: v1invitationsid-delete
      parameters:
      - in: path
        name: id
        description: Identifier of the invitation to delete
      responses:
        200:
          description: OK
      tags:
      - Invitation
    get:
      summary: Get Invitation
      description: |-
        Returns an invitation.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to view the
        requested invitation or for access errors.
        * `NOT_FOUND` if no invitation exists with the requested ID.
      operationId: classroom.invitations.get
      x-api-path-slug: v1invitationsid-get
      parameters:
      - in: path
        name: id
        description: Identifier of the invitation to return
      responses:
        200:
          description: OK
      tags:
      - Invitation
  /v1/invitations/{id}:accept:
    post:
      summary: Accept Invitation
      description: |-
        Accepts an invitation, removing it and adding the invited user to the
        teachers or students (as appropriate) of the specified course. Only the
        invited user may accept an invitation.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to accept the
        requested invitation or for access errors.
        * `FAILED_PRECONDITION` for the following request errors:
            * CourseMemberLimitReached
            * CourseNotModifiable
            * CourseTeacherLimitReached
            * UserGroupsMembershipLimitReached
        * `NOT_FOUND` if no invitation exists with the requested ID.
      operationId: classroom.invitations.accept
      x-api-path-slug: v1invitationsidaccept-post
      parameters:
      - in: path
        name: id
        description: Identifier of the invitation to accept
      responses:
        200:
          description: OK
      tags:
      - Invitation
  /v1/userProfiles/{studentId}/guardianInvitations:
    get:
      summary: Get Guardian Invitations
      description: |-
        Returns a list of guardian invitations that the requesting user is
        permitted to view, filtered by the parameters provided.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if a `student_id` is specified, and the requesting
          user is not permitted to view guardian invitations for that student, if
          `"-"` is specified as the `student_id` and the user is not a domain
          administrator, if guardians are not enabled for the domain in question,
          or for other access errors.
        * `INVALID_ARGUMENT` if a `student_id` is specified, but its format cannot
          be recognized (it is not an email address, nor a `student_id` from the
          API, nor the literal string `me`). May also be returned if an invalid
          `page_token` or `state` is provided.
        * `NOT_FOUND` if a `student_id` is specified, and its format can be
          recognized, but Classroom has no record of that student.
      operationId: classroom.userProfiles.guardianInvitations.list
      x-api-path-slug: v1userprofilesstudentidguardianinvitations-get
      parameters:
      - in: query
        name: invitedEmailAddress
        description: If specified, only results with the specified `invited_email_address`will
          be returned
      - in: query
        name: pageSize
        description: Maximum number of items to return
      - in: query
        name: pageToken
        description: nextPageTokenvalue returned from a previouslist call,indicating
          that the subsequent page of results should be returned
      - in: query
        name: states
        description: If specified, only results with the specified `state` values
          will bereturned
      - in: path
        name: studentId
        description: The ID of the student whose guardian invitations are to be returned
      responses:
        200:
          description: OK
      tags:
      - Guardian Invitation
    post:
      summary: Create Guardian Invitation
      description: |-
        Creates a guardian invitation, and sends an email to the guardian asking
        them to confirm that they are the student's guardian.

        Once the guardian accepts the invitation, their `state` will change to
        `COMPLETED` and they will start receiving guardian notifications. A
        `Guardian` resource will also be created to represent the active guardian.

        The request object must have the `student_id` and
        `invited_email_address` fields set. Failing to set these fields, or
        setting any other fields in the request, will result in an error.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the current user does not have permission to
          manage guardians, if the guardian in question has already rejected
          too many requests for that student, if guardians are not enabled for the
          domain in question, or for other access errors.
        * `RESOURCE_EXHAUSTED` if the student or guardian has exceeded the guardian
          link limit.
        * `INVALID_ARGUMENT` if the guardian email address is not valid (for
          example, if it is too long), or if the format of the student ID provided
          cannot be recognized (it is not an email address, nor a `user_id` from
          this API). This error will also be returned if read-only fields are set,
          or if the `state` field is set to to a value other than `PENDING`.
        * `NOT_FOUND` if the student ID provided is a valid student ID, but
          Classroom has no record of that student.
        * `ALREADY_EXISTS` if there is already a pending guardian invitation for
          the student and `invited_email_address` provided, or if the provided
          `invited_email_address` matches the Google account of an existing
          `Guardian` for this user.
      operationId: classroom.userProfiles.guardianInvitations.create
      x-api-path-slug: v1userprofilesstudentidguardianinvitations-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: studentId
        description: ID of the student (in standard format)
      responses:
        200:
          description: OK
      tags:
      - Guardian Invitation
  /v1/userProfiles/{studentId}/guardianInvitations/{invitationId}:
    get:
      summary: Get Guardian Invitation
      description: |-
        Returns a specific guardian invitation.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to view
          guardian invitations for the student identified by the `student_id`, if
          guardians are not enabled for the domain in question, or for other
          access errors.
        * `INVALID_ARGUMENT` if a `student_id` is specified, but its format cannot
          be recognized (it is not an email address, nor a `student_id` from the
          API, nor the literal string `me`).
        * `NOT_FOUND` if Classroom cannot find any record of the given student or
          `invitation_id`. May also be returned if the student exists, but the
          requesting user does not have access to see that student.
      operationId: classroom.userProfiles.guardianInvitations.get
      x-api-path-slug: v1userprofilesstudentidguardianinvitationsinvitationid-get
      parameters:
      - in: path
        name: invitationId
        description: The `id` field of the `GuardianInvitation` being requested
      - in: path
        name: studentId
        description: The ID of the student whose guardian invitation is being requested
      responses:
        200:
          description: OK
      tags:
      - Guardian Invitation
    patch:
      summary: Update Guardian Invitations
      description: |-
        Modifies a guardian invitation.

        Currently, the only valid modification is to change the `state` from
        `PENDING` to `COMPLETE`. This has the effect of withdrawing the invitation.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the current user does not have permission to
          manage guardians, if guardians are not enabled for the domain in question
          or for other access errors.
        * `FAILED_PRECONDITION` if the guardian link is not in the `PENDING` state.
        * `INVALID_ARGUMENT` if the format of the student ID provided
          cannot be recognized (it is not an email address, nor a `user_id` from
          this API), or if the passed `GuardianInvitation` has a `state` other than
          `COMPLETE`, or if it modifies fields other than `state`.
        * `NOT_FOUND` if the student ID provided is a valid student ID, but
          Classroom has no record of that student, or if the `id` field does not
          refer to a guardian invitation known to Classroom.
      operationId: classroom.userProfiles.guardianInvitations.patch
      x-api-path-slug: v1userprofilesstudentidguardianinvitationsinvitationid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: invitationId
        description: The `id` field of the `GuardianInvitation` to be modified
      - in: path
        name: studentId
        description: The ID of the student whose guardian invitation is to be modified
      - in: query
        name: updateMask
        description: Mask that identifies which fields on the course to update
      responses:
        200:
          description: OK
      tags:
      - Guardian Invitation
  /v1/userProfiles/{studentId}/guardians:
    get:
      summary: Get Guardians
      description: |-
        Returns a list of guardians that the requesting user is permitted to
        view, restricted to those that match the request.

        To list guardians for any student that the requesting user may view
        guardians for, use the literal character `-` for the student ID.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if a `student_id` is specified, and the requesting
          user is not permitted to view guardian information for that student, if
          `"-"` is specified as the `student_id` and the user is not a domain
          administrator, if guardians are not enabled for the domain in question,
          if the `invited_email_address` filter is set by a user who is not a
          domain administrator, or for other access errors.
        * `INVALID_ARGUMENT` if a `student_id` is specified, but its format cannot
          be recognized (it is not an email address, nor a `student_id` from the
          API, nor the literal string `me`). May also be returned if an invalid
          `page_token` is provided.
        * `NOT_FOUND` if a `student_id` is specified, and its format can be
          recognized, but Classroom has no record of that student.
      operationId: classroom.userProfiles.guardians.list
      x-api-path-slug: v1userprofilesstudentidguardians-get
      parameters:
      - in: query
        name: invitedEmailAddress
        description: Filter results by the email address that the original invitation
          was sentto, resulting in this guardian link
      - in: query
        name: pageSize
        description: Maximum number of items to return
      - in: query
        name: pageToken
        description: nextPageTokenvalue returned from a previouslist call,indicating
          that the subsequent page of results should be returned
      - in: path
        name: studentId
        description: Filter results by the student who the guardian is linked to
      responses:
        200:
          description: OK
      tags:
      - Guardian
  /v1/userProfiles/{studentId}/guardians/{guardianId}:
    delete:
      summary: Delete Guardian
      description: |-
        Deletes a guardian.

        The guardian will no longer receive guardian notifications and the guardian
        will no longer be accessible via the API.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if no user that matches the provided `student_id`
          is visible to the requesting user, if the requesting user is not
          permitted to manage guardians for the student identified by the
          `student_id`, if guardians are not enabled for the domain in question,
          or for other access errors.
        * `INVALID_ARGUMENT` if a `student_id` is specified, but its format cannot
          be recognized (it is not an email address, nor a `student_id` from the
          API).
        * `NOT_FOUND` if the requesting user is permitted to modify guardians for
          the requested `student_id`, but no `Guardian` record exists for that
          student with the provided `guardian_id`.
      operationId: classroom.userProfiles.guardians.delete
      x-api-path-slug: v1userprofilesstudentidguardiansguardianid-delete
      parameters:
      - in: path
        name: guardianId
        description: The `id` field from a `Guardian`
      - in: path
        name: studentId
        description: The student whose guardian is to be deleted
      responses:
        200:
          description: OK
      tags:
      - Guardian
    get:
      summary: Get Guardian
      description: |-
        Returns a specific guardian.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if no user that matches the provided `student_id`
          is visible to the requesting user, if the requesting user is not
          permitted to view guardian information for the student identified by the
          `student_id`, if guardians are not enabled for the domain in question,
          or for other access errors.
        * `INVALID_ARGUMENT` if a `student_id` is specified, but its format cannot
          be recognized (it is not an email address, nor a `student_id` from the
          API, nor the literal string `me`).
        * `NOT_FOUND` if the requesting user is permitted to view guardians for
          the requested `student_id`, but no `Guardian` record exists for that
          student that matches the provided `guardian_id`.
      operationId: classroom.userProfiles.guardians.get
      x-api-path-slug: v1userprofilesstudentidguardiansguardianid-get
      parameters:
      - in: path
        name: guardianId
        description: The `id` field from a `Guardian`
      - in: path
        name: studentId
        description: The student whose guardian is being requested
      responses:
        200:
          description: OK
      tags:
      - Guardian
  /v1/userProfiles/{userId}:
    get:
      summary: Get User
      description: |-
        Returns a user profile.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to access
        this user profile, if no profile exists with the requested ID, or for
        access errors.
      operationId: classroom.userProfiles.get
      x-api-path-slug: v1userprofilesuserid-get
      parameters:
      - in: path
        name: userId
        description: Identifier of the profile to return
      responses:
        200:
          description: OK
      tags:
      - User