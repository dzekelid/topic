{
  "info": {
    "name": "Instructure Canvas Groups API Rate entry",
    "_postman_id": "89bbcef3-9919-46ff-85d8-e78f527d3875",
    "description": "Rate entry.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "8e9e099f-99e1-4083-8285-8bbc6693b1f8",
          "name": "create-a-group",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/groups?description=%7B%7D&is_public=%7B%7D&join_level=%7B%7D&name=%7B%7D&storage_quota_mb=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22f11ca1-240c-457e-9cdc-89c1468a7353"
            }
          ]
        },
        {
          "id": "3a4bd77e-bd8e-43f5-bd81-8baa540a6ebe",
          "name": "get-a-single-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id"
              ],
              "query": [
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e4d0f82-64b9-43a0-8541-aa229734bc08"
            }
          ]
        },
        {
          "id": "62a7490a-fa50-4d06-80dd-ea89022ae440",
          "name": "edit-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id"
              ],
              "query": [
                {
                  "key": "avatar_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_public",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "join_level",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "members",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "storage_quota_mb",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Edit a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48ce1fab-4e34-4a92-9f2e-522851f0daf8"
            }
          ]
        },
        {
          "id": "287df31c-8622-48f4-bdf2-732dedb3870e",
          "name": "delete-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b4a8d1f-4c1a-40cd-8039-f7ec9c4e5b71"
            }
          ]
        },
        {
          "id": "49a87156-5c12-46de-86ac-ca081be870e3",
          "name": "group-activity-stream",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/activity_stream"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Group activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f717a021-b64e-4439-9e41-1e772662405c"
            }
          ]
        },
        {
          "id": "290b163e-dd7f-4ae7-8792-3fe19a4252c3",
          "name": "group-activity-stream-summary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/activity_stream/summary"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Group activity stream summary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e97a535-5a17-408f-ba2f-f0b32738da9f"
            }
          ]
        },
        {
          "id": "ea6323ab-2dbe-4335-9fdb-7bd4fb6d0dd8",
          "name": "redirect-to-the-assignment-override-for-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/assignments/assignment_id/override"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Redirect to the assignment override for a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df358dd1-2bd4-486d-a8cb-e572a8ce56a3"
            }
          ]
        },
        {
          "id": "6ace8689-ce2f-40df-a825-10afbac0c66c",
          "name": "list-conferences",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/conferences"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List conferences."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64919270-3167-4120-befd-6bddd06a7cc1"
            }
          ]
        },
        {
          "id": "79eb047d-5a24-4d2b-bc26-48848567ebed",
          "name": "list-content-exports",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_exports"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List content exports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ddb4407-4f75-41a4-9b82-2d8c4c8274fc"
            }
          ]
        },
        {
          "id": "947eb055-dcaf-4f96-966f-fec9688e8d76",
          "name": "export-content",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_exports"
              ],
              "query": [
                {
                  "key": "export_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip_notifications",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Export content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d20d0f7f-94bb-489b-905b-330fc477c622"
            }
          ]
        },
        {
          "id": "46f23bc9-29d0-4616-a6f7-57afada1e64e",
          "name": "show-content-export",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_exports/id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Show content export."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95ac380e-10e3-4bf1-a3a1-aa67243caa2f"
            }
          ]
        },
        {
          "id": "25890f23-122b-47d8-8521-37efc97a8cd2",
          "name": "list-licenses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_licenses"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List licenses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd4ce33e-4862-4b6c-aa59-98e3a43beb3d"
            }
          ]
        },
        {
          "id": "2d8c96e2-d65f-4364-9987-1b3369a962a7",
          "name": "list-content-migrations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List content migrations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f521d257-4702-4f8b-a861-b09e2bfdc57e"
            }
          ]
        },
        {
          "id": "b216c86d-d783-455c-af6a-a8ef0223a1bf",
          "name": "create-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations"
              ],
              "query": [
                {
                  "key": "date_shift_options[day_substitutions][X]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[new_end_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[new_start_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[old_end_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[old_start_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[remove_dates]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[shift_dates]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "migration_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pre_attachment[*]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pre_attachment[name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[file_url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[folder_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[overwrite_quizzes]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[question_bank_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[question_bank_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[source_course_id]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3265afb-8c71-4f83-8447-52796b1ed708"
            }
          ]
        },
        {
          "id": "ef48dd82-12f4-4aa5-abde-ad8e3cc41c06",
          "name": "list-migration-issues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/content_migration_id/migration_issues"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List migration issues."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4fdac877-de60-41fd-9e1e-13dffec680a7"
            }
          ]
        },
        {
          "id": "bcffbe95-16be-43ea-b472-09501fe57f6b",
          "name": "get-a-migration-issue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/content_migration_id/migration_issues/:id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a migration issue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3947405a-abae-4e27-9028-98df1a5733b6"
            }
          ]
        },
        {
          "id": "518ed8f6-f3c8-4039-a1ba-09d2c216feb0",
          "name": "update-a-migration-issue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/content_migration_id/migration_issues/:id"
              ],
              "query": [
                {
                  "key": "workflow_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a migration issue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "feed6530-15d1-445c-b987-1282b220fe3f"
            }
          ]
        },
        {
          "id": "4cc6d2f6-5250-4ca2-95e2-7071fd12a653",
          "name": "get-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8cd5a208-15c2-459c-a21a-c8522034fb63"
            }
          ]
        },
        {
          "id": "3305fe6c-bdeb-4cf6-bc04-4c28a3679ab3",
          "name": "update-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04da3eca-cbf6-4e59-879b-a4c1ddbef876"
            }
          ]
        },
        {
          "id": "90b4a882-dc34-47fb-a03a-114a264b03e6",
          "name": "list-migration-systems",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/migrators"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List migration systems."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11a2c49e-0cdf-45f7-8d6f-93abdfb209d1"
            }
          ]
        },
        {
          "id": "2525e436-7645-4bd7-86a3-1c7d6577f85b",
          "name": "list-discussion-topics",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics"
              ],
              "query": [
                {
                  "key": "only_announcements",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "order_by",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "scope",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "search_term",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List discussion topics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41fdeae8-bdc4-46dd-a4e9-3137683add5d"
            }
          ]
        },
        {
          "id": "916526d5-b468-4d7a-8191-1207d6d942c3",
          "name": "create-a-new-discussion-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics"
              ],
              "query": [
                {
                  "key": "allow_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "attachment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "delayed_post_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "discussion_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "group_category_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_announcement",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lock_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "only_graders_can_rate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pinned",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_enabled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_has_student_posts",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "published",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "require_initial_post",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_by_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new discussion topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3999b1c2-3ceb-4501-827f-d03d5937c8b4"
            }
          ]
        },
        {
          "id": "045d0bfd-391a-44f5-a7f2-875c03474f79",
          "name": "reorder-pinned-topics",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/reorder"
              ],
              "query": [
                {
                  "key": "order",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reorder pinned topics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ffbea86-4917-44e7-b976-6ed5955e19b7"
            }
          ]
        },
        {
          "id": "f2ea0637-05c4-4f7a-a2ba-1acdcbc08a3c",
          "name": "get-a-single-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7e02081-e6fd-4b09-bd84-93bb3a6349b1"
            }
          ]
        },
        {
          "id": "0c159164-3825-4dd4-beab-ee1cf939f543",
          "name": "update-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id"
              ],
              "query": [
                {
                  "key": "allow_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "delayed_post_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "discussion_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "group_category_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_announcement",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lock_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "only_graders_can_rate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pinned",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_enabled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_has_student_posts",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "published",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "require_initial_post",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_by_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1456a464-1a08-4718-a322-7ee84d4aaf11"
            }
          ]
        },
        {
          "id": "fca02626-f821-49eb-98ad-ef22a03be7de",
          "name": "delete-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20a0e14e-e696-4743-82f9-a1b475766d2f"
            }
          ]
        },
        {
          "id": "2a13b73f-3986-48ad-ae40-21aa75d868a0",
          "name": "list-topic-entries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List topic entries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e46b14dc-e13c-4af8-b642-e1e74bb8affa"
            }
          ]
        },
        {
          "id": "ee941fcc-8c96-4368-b3ec-5b6ef52adcf4",
          "name": "post-an-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries"
              ],
              "query": [
                {
                  "key": "attachment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post an entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58f95fcb-ea91-44d4-aa4e-c728dd17ff27"
            }
          ]
        },
        {
          "id": "4f7a4b01-0cab-4ab4-a235-91e2af11e16a",
          "name": "rate-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/rating"
              ],
              "query": [
                {
                  "key": "rating",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Rate entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61d8f416-cf44-4d66-babe-a055f7ae5e74"
            }
          ]
        }
      ]
    }
  ]
}