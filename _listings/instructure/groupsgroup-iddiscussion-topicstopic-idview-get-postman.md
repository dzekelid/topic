{
  "info": {
    "name": "Instructure Canvas Groups API Get the full topic",
    "_postman_id": "b82bb1df-658c-4fe2-b3f8-b9c7c3bb185c",
    "description": "Get the full topic.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "92c1e960-6511-407e-a53f-95938bc68ba3",
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
              "id": "af38816b-1cac-48ff-a2e3-fdf04f63eeed"
            }
          ]
        },
        {
          "id": "0d286cf4-6982-4325-a5b6-1d75699c095c",
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
              "id": "a138dc53-4f27-4ed3-95a4-ea58abf6395c"
            }
          ]
        },
        {
          "id": "e9a453fd-6703-412e-9f21-aaa04904da5a",
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
              "id": "169d4f40-155d-48fa-8e4e-b16fa07ae254"
            }
          ]
        },
        {
          "id": "df9be796-7d47-4551-a399-efb742385e11",
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
              "id": "0c780107-e3d0-4614-b58d-022753ef5273"
            }
          ]
        },
        {
          "id": "6a220ccd-02c1-4f1a-ae58-eea68e072475",
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
              "id": "8063e5e8-8913-454e-99bf-e5d8ae186e5b"
            }
          ]
        },
        {
          "id": "d6807826-8fa5-4f4c-9423-31726e41ff03",
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
              "id": "0879f707-6e81-4a98-b542-f34a3cef1edf"
            }
          ]
        },
        {
          "id": "a1eb69e2-2d82-42f8-86a7-c3ecc38a649c",
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
              "id": "6b0d6892-5f11-4a5a-8765-462a928f544e"
            }
          ]
        },
        {
          "id": "52022e8f-f8ba-4726-bbf7-23be34c6d2f2",
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
              "id": "3610b6fd-156e-4e81-881b-f821f0110784"
            }
          ]
        },
        {
          "id": "bd09256b-befc-4cbc-96b7-46696f0da398",
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
              "id": "adc0fe55-a73f-49ce-9afb-52c3f568450f"
            }
          ]
        },
        {
          "id": "edbd2419-ec52-4797-a92b-3a971f439efa",
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
              "id": "00168256-8c5e-4c27-be56-3ef741ea5e42"
            }
          ]
        },
        {
          "id": "28d7c4dc-dd14-4796-8798-e011eec6e206",
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
              "id": "40803fa2-f4a4-4093-ad71-c57ac02bab84"
            }
          ]
        },
        {
          "id": "383ad11f-12e3-4373-8f8a-152712557311",
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
              "id": "4a19b35e-b599-4250-b3aa-ee13a9a06607"
            }
          ]
        },
        {
          "id": "dd9f1a93-799d-4820-be16-2f27e1640e1c",
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
              "id": "400afc45-e0c9-4e1d-af12-305e12aaf26d"
            }
          ]
        },
        {
          "id": "3b3cdafb-e37a-402d-9792-9fe70b0f683b",
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
              "id": "2b70aadc-bf1f-469e-92b6-e9b2c2637d5d"
            }
          ]
        },
        {
          "id": "29865aa1-6c3a-4b29-b76e-ef9f5cfe4edf",
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
              "id": "48a71215-2a4b-4981-8dc0-f9400fbd1e2e"
            }
          ]
        },
        {
          "id": "2f38fb83-83be-4141-8bd9-0575d2af3b11",
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
              "id": "675cadf9-ee32-4f2c-9487-83d32f971e04"
            }
          ]
        },
        {
          "id": "de572c91-ef43-4890-963f-6bb8a84ebb36",
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
              "id": "ae9c5859-3e3c-48c1-96c9-eb34fa6e08fc"
            }
          ]
        },
        {
          "id": "fa9369a2-9665-4f30-84bc-df27211c7e8d",
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
              "id": "d9a71071-e95c-4cbf-8ea0-d824ee327ffc"
            }
          ]
        },
        {
          "id": "09bc97dc-cb3e-494b-8b27-8b525a5825ed",
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
              "id": "22692edc-dd4f-4c26-986a-9fda10bab677"
            }
          ]
        },
        {
          "id": "7b2a65f1-4714-427d-835b-9c9e30c60351",
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
              "id": "117c8ea2-6950-4aea-84ff-89da45d6d2d4"
            }
          ]
        },
        {
          "id": "a7220d8a-486a-482a-8fea-797a79dfdfe8",
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
              "id": "6ea16769-d3bd-4fe4-aab6-7c1087d719dd"
            }
          ]
        },
        {
          "id": "cba19e35-4e8c-483b-9d61-e66938e20a4b",
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
              "id": "07ab8e04-43e1-44cb-9cae-538f707c361f"
            }
          ]
        },
        {
          "id": "1425ea16-f53d-4936-b910-0c01976fdc44",
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
              "id": "4aa84ad2-d4ec-469f-bd5b-f1666173284a"
            }
          ]
        },
        {
          "id": "8e44ce4c-8bfc-4e64-895c-db161f64fd0a",
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
              "id": "58b105d1-e4b3-482a-903f-8e026a1e9e05"
            }
          ]
        },
        {
          "id": "3c645969-1e2a-47dc-af11-fdfb5b420da4",
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
              "id": "3c09a92f-ec4c-4cf5-9e0e-450ad254d815"
            }
          ]
        },
        {
          "id": "8a2e64c8-92fe-4870-9da1-edb2d5616089",
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
              "id": "9ce34143-d95d-4a2f-8ace-6b98ffd9d77e"
            }
          ]
        },
        {
          "id": "ae36bea2-7eba-4abf-b75b-084927a3d4b3",
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
              "id": "063b1184-3712-4dcd-bfc0-9eb795af4dcb"
            }
          ]
        },
        {
          "id": "3f33b5fa-2aaf-4d7d-9bfe-6ecdab9b4a86",
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
              "id": "075d469b-df2b-4dde-b6d5-e7bd0c48dc86"
            }
          ]
        },
        {
          "id": "c25c03b7-aa1f-431d-9624-8d5aeee8b8ac",
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
              "id": "37fdcf31-acd7-47e0-a0b4-ec83b0d32984"
            }
          ]
        },
        {
          "id": "b3700625-07e3-4a78-8631-b3e14c1846db",
          "name": "mark-entry-as-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/read"
              ],
              "query": [
                {
                  "key": "forced_read_state",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Mark entry as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3f8d2ce-95e4-4a95-a398-36aec4f3b3c5"
            }
          ]
        },
        {
          "id": "117f68e9-c331-4521-a0c9-bf3579950e86",
          "name": "mark-entry-as-unread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/read"
              ],
              "query": [
                {
                  "key": "forced_read_state",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Mark entry as unread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f9bbc6e-b290-458a-8475-e012960f6415"
            }
          ]
        },
        {
          "id": "ae625b4c-9576-43e6-8328-f79552ace1b4",
          "name": "list-entry-replies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/replies"
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List entry replies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b87abcd2-90cf-4dd4-ae48-58622f484d32"
            }
          ]
        },
        {
          "id": "966f3853-fc3f-4757-b72e-cc02ad05c912",
          "name": "post-a-reply",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/replies"
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
            "description": "Post a reply."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c7845c0-c2eb-42aa-832a-3bb3418073d4"
            }
          ]
        },
        {
          "id": "7709b6c1-d8b6-4f04-8825-6f323327b943",
          "name": "update-an-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:id"
              ],
              "query": [
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
            "description": "Update an entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "655821af-677d-4cf2-b26c-2bde6b8c29ff"
            }
          ]
        },
        {
          "id": "666363af-5b9b-417f-92b7-46a7550c7368",
          "name": "delete-an-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:id"
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "271a1a09-d163-456f-b9be-9fbd0efa53b1"
            }
          ]
        },
        {
          "id": "2aefb305-a093-4af3-9f53-eb1fa89ea775",
          "name": "list-entries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entry_list"
              ],
              "query": [
                {
                  "key": "ids",
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
            "description": "List entries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "423ce8be-ffd8-4256-b82b-1684866e55ab"
            }
          ]
        },
        {
          "id": "f02f90b6-3e96-4f0b-b37d-ce5bec803959",
          "name": "mark-topic-as-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read"
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
            "description": "Mark topic as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37b59de7-fd1b-4d5f-b198-ae4317badf6e"
            }
          ]
        },
        {
          "id": "3aae2970-828e-4ca4-927c-3cfdf12c5d0b",
          "name": "mark-topic-as-unread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read"
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
            "description": "Mark topic as unread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1bf11534-d1e2-4ab7-85e7-cd541ab8b5bf"
            }
          ]
        },
        {
          "id": "faaa51f7-e434-4246-a595-14e5678845b5",
          "name": "mark-all-entries-as-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read_all"
              ],
              "query": [
                {
                  "key": "forced_read_state",
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
            "description": "Mark all entries as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e57838cc-eae1-4159-9881-1f34dc622fb9"
            }
          ]
        },
        {
          "id": "1d9af393-d169-4b75-8a85-94f6998b7de0",
          "name": "mark-all-entries-as-unread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read_all"
              ],
              "query": [
                {
                  "key": "forced_read_state",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Mark all entries as unread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c42680c-7bf0-4125-b27e-b1742de25b68"
            }
          ]
        },
        {
          "id": "b05c493a-3201-4d03-af16-da88627377cd",
          "name": "subscribe-to-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/subscribed"
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
            "description": "Subscribe to a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfef873b-da95-4d40-8145-a65e9a266903"
            }
          ]
        },
        {
          "id": "38c25d48-84ef-4535-ac24-3dca81637396",
          "name": "unsubscribe-from-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/subscribed"
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
            "description": "Unsubscribe from a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95e4f769-1507-48a5-8fea-302b897cb0f9"
            }
          ]
        },
        {
          "id": "b77c2f61-f3f1-41fe-a1fe-7c9d3ffb9472",
          "name": "get-the-full-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/view"
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
            "description": "Get the full topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bdc961f3-88bd-42a6-a9ba-e71cef5491aa"
            }
          ]
        }
      ]
    }
  ]
}