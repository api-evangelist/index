{
  "info": {
    "name": "Open Skills API Skill Name Normalization",
    "_postman_id": "ec28c516-73fb-4835-b9b0-5ae29f705afe",
    "description": "Retrieves the canonical skill name for a synonymous skill name",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Job",
      "item": [
        {
          "id": "88246ad4-bf0f-4823-a6dd-b18c086ceb59",
          "name": "retrieves-the-names-descriptions-and-uuids-of-all-job-titles",
          "request": {
            "url": "http://api.dataatwork.org/v1/jobs?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the names, descriptions, and UUIDs of all job titles."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2352f0d-4621-4cb8-a717-6263acaa0e10"
            }
          ]
        },
        {
          "id": "4676520f-e1ba-4c26-ad1b-1f1f970cd26b",
          "name": "retrieves-the-name-description-and-uuid-of-a-job-by-specifying-its-onet-soc-code-or-uuid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "jobs/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the name, description, and UUID of a job by specifying its O*NET SOC Code or UUID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e1fec5e-93b8-4219-8848-eb03df4acb70"
            }
          ]
        },
        {
          "id": "2a7ad2ba-86b2-4de8-8b6b-ffc527d316cd",
          "name": "retrieves-the-names-descriptions-and-uuids-of-all-job-titles-matching-a-given-search-criteria",
          "request": {
            "url": "http://api.dataatwork.org/v1/jobs/autocomplete?begins_with=%7B%7D&contains=%7B%7D&ends_with=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the names, descriptions, and UUIDs of all job titles matching a given search criteria."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3d4c91c-4d6e-421a-b197-7715c943e169"
            }
          ]
        },
        {
          "id": "015c4fb4-8406-4653-9ec8-f36e591bd9e6",
          "name": "retrieves-the-canonical-job-title-for-a-synonymous-job-title",
          "request": {
            "url": "http://api.dataatwork.org/v1/jobs/normalize?job_title=%7B%7D&limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the canonical job title for a synonymous job title"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4909fbb6-524d-41c2-b16b-4057665b4aa1"
            }
          ]
        }
      ]
    },
    {
      "name": "Skills",
      "item": [
        {
          "id": "db72708b-dfb1-404e-8bdf-14a30fb7a070",
          "name": "retrieves-a-collection-of-skills-associated-with-a-specified-job",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "jobs/:id/related_skills"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a collection of skills associated with a specified job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea2c2455-52e8-4529-b2cb-e38632aef7b0"
            }
          ]
        },
        {
          "id": "f2a7477d-755c-4ac1-954b-8c5f2a33f3ff",
          "name": "retrieves-a-collection-of-skills-associated-with-a-specified-skill",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "skills/:id/related_skills"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a collection of skills associated with a specified skill."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1b0dbaa-7e9c-4dee-9c0a-a47d5bfb6418"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "ee1da02e-c3b6-4066-ae8e-77969cfe82c2",
          "name": "retrieves-a-collection-of-jobs-associated-with-a-specified-job",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "jobs/:id/related_jobs"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a collection of jobs associated with a specified job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a19c7b27-fb71-4308-a9ac-18d2cd8ef0cf"
            }
          ]
        },
        {
          "id": "f28df96a-c0d0-485d-ab49-616cb2cab39f",
          "name": "retrieves-a-collection-of-jobs-associated-with-a-specified-skill",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "skills/:id/related_jobs"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a collection of jobs associated with a specified skill."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ef4b81f-245e-4069-92a9-857cb8e13fe5"
            }
          ]
        }
      ]
    },
    {
      "name": "Unusual",
      "item": [
        {
          "id": "7a52ac36-7d8a-4842-96c9-d238e509c037",
          "name": "retrieves-a-list-of-unusual-job-titles-and-the-uuids-of-their-canonical-jobs",
          "request": {
            "url": "http://api.dataatwork.org/v1/jobs/unusual_titles",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of unusual job titles and the UUIDs of their canonical jobs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a7541e8-f53c-4e3a-a6ec-233072cc8775"
            }
          ]
        }
      ]
    },
    {
      "name": "Skill",
      "item": [
        {
          "id": "2fa9f64c-93cd-49dc-81dd-bf35e73f4169",
          "name": "retrieve-the-names-descriptions-and-uuids-of-all-skills",
          "request": {
            "url": "http://api.dataatwork.org/v1/skills?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the names, descriptions, and UUIDs of all skills."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69366a32-dac9-463f-b91d-648ffd3d085f"
            }
          ]
        },
        {
          "id": "f03ccb79-ddc3-4ff7-a204-9093ed93c769",
          "name": "retrieves-the-name-description-and-uuid-of-a-job-by-specifying-its-uuid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "skills/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the name, description, and UUID of a job by specifying its UUID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd5d9790-3207-48c5-a906-a26bf5e2706d"
            }
          ]
        },
        {
          "id": "a7e4c664-09f6-42ca-82ff-b6bb191bd38b",
          "name": "retrieves-the-names-descriptions-and-uuids-of-all-skills-matching-a-given-search-criteria",
          "request": {
            "url": "http://api.dataatwork.org/v1/skills/autocomplete?begins_with=%7B%7D&contains=%7B%7D&ends_with=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the names, descriptions, and UUIDs of all skills matching a given search criteria."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "010e5977-bb69-4f37-96a4-5f3a91d33f27"
            }
          ]
        },
        {
          "id": "7d91a5d7-01e0-427f-9597-e4fdd846be9e",
          "name": "retrieves-the-canonical-skill-name-for-a-synonymous-skill-name",
          "request": {
            "url": "http://api.dataatwork.org/v1/skills/normalize?skill_name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the canonical skill name for a synonymous skill name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3076234c-e925-4171-b332-1de47af9f33c"
            }
          ]
        }
      ]
    }
  ]
}