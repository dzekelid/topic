{
  "info": {
    "name": "AWS Simple Email Service API Set Identity Notification Topic",
    "_postman_id": "814ab8f1-e78e-4e73-abb0-b6f7c0e349a5",
    "description": "Given an identity (an email address or a domain), sets the Amazon Simple Notification Service (Amazon SNS) topic to which Amazon SES will publish\n        bounce, complaint, and/or delivery notifications for emails sent with that identity as the Source.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Rule Sets",
      "item": [
        {
          "id": "3dae6c44-a0f8-46c4-b530-930ab5f80972",
          "name": "cloneReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=CloneReceiptRuleSet?OriginalRuleSetName=OriginalRuleSetName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a receipt rule set by cloning an existing one."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9568c814-c840-43c6-a004-ee66e34ba068"
            }
          ]
        },
        {
          "id": "c6cb967c-bfa3-4a23-8de9-47dfe4664404",
          "name": "createReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an empty receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f601b02c-1268-44f4-856c-df9a4cc1f620"
            }
          ]
        },
        {
          "id": "bf4c2775-afba-4f3d-a2d7-17011dc9d7f5",
          "name": "deleteReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified receipt rule set and all of the receipt rules it contains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62e4a3bb-1c0c-4a6b-aa5c-043d3ed1d3f8"
            }
          ]
        },
        {
          "id": "86c696ca-5b12-434d-827c-608a75f50d04",
          "name": "describeActiveReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActiveReceiptRuleSet?Metadata=Metadata&Rules.member.N=Rules.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the metadata and receipt rules for the receipt rule set that is currently active."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "977d6bdb-a275-4882-a778-9a1d6bcc2aa1"
            }
          ]
        },
        {
          "id": "3ee11061-28cb-47a0-a8b2-2d578d7fe839",
          "name": "describeReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6f5b806-d254-405c-b926-4ccc169d2533"
            }
          ]
        },
        {
          "id": "8b126332-07b2-44b7-a1dc-03216e28b243",
          "name": "listReceiptRuleSets",
          "request": {
            "url": "http://example.com/api/?Action=ListReceiptRuleSets?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the receipt rule sets that exist under your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7530dc9f-0d68-4941-a3ed-96d6091bdb36"
            }
          ]
        },
        {
          "id": "805c1be5-d182-4f26-b88e-72dd613b6a6a",
          "name": "reorderReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=ReorderReceiptRuleSet?RuleNames.member.N=RuleNames.member.N&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Reorders the receipt rules within a receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e40f88b9-fe1e-450a-9c5c-af580d294c68"
            }
          ]
        },
        {
          "id": "c4c77dfb-9618-4f35-a177-3529cd0aa5f4",
          "name": "setActiveReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=SetActiveReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the specified receipt rule set as the active receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a599e8b4-ee40-4e5c-b531-48f55260ba59"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Sets",
      "item": [
        {
          "id": "d2ecf7fa-1521-4a04-9f4c-b6ca02ede765",
          "name": "createConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationSet?ConfigurationSet=ConfigurationSet",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3fa1b2c-9775-4601-b4c5-c5cba1e3ad3f"
            }
          ]
        },
        {
          "id": "176561a7-6c5f-49bd-aac8-c0724933b30b",
          "name": "deleteConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationSet?ConfigurationSetName=ConfigurationSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eec8aba0-7b4d-426c-a491-022ddc9133f2"
            }
          ]
        },
        {
          "id": "b5209900-42e8-4573-8ec8-e1dde097587b",
          "name": "describeConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConfigurationSet?ConfigurationSetAttributeNames.member.N=ConfigurationSetAttributeNames.member.N&ConfigurationSetName=ConfigurationSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee1485cb-d545-4b02-8578-f566324e55fe"
            }
          ]
        },
        {
          "id": "26137927-8be7-481c-801a-51d3abd0f49b",
          "name": "listConfigurationSets",
          "request": {
            "url": "http://example.com/api/?Action=ListConfigurationSets?MaxItems=MaxItems&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the configuration sets associated with your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f8ceb7c-f940-4b53-a488-682d58e5e3dc"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Set Event Destination",
      "item": [
        {
          "id": "55fd12bf-0ebe-484a-ae65-31fa2a019c3f",
          "name": "createConfigurationSetEventDestination",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationSetEventDestination?ConfigurationSetName=ConfigurationSetName&EventDestination=EventDestination",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration set event destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54fbcaef-4c6b-4365-8638-2d599b512c32"
            }
          ]
        },
        {
          "id": "7007b510-cb5f-4763-828a-1bf4982d0e25",
          "name": "deleteConfigurationSetEventDestination",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationSetEventDestination?ConfigurationSetName=ConfigurationSetName&EventDestinationName=EventDestinationName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a configuration set event destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3192163c-4b87-4008-9c0a-5b2e4e875899"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "da2758f9-bc32-4d6c-937e-eb1e61d1b6a5",
          "name": "createReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptFilter?Filter=Filter",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d92d6c4-1f40-4be2-8963-1f566403f565"
            }
          ]
        },
        {
          "id": "2858b01f-292e-47a6-8438-8bfd57a2f6df",
          "name": "deleteReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptFilter?FilterName=FilterName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9a098cb-b4c0-4a35-b842-a2a5a1c52f0c"
            }
          ]
        },
        {
          "id": "300fc26d-bd50-4fdf-888b-b4236b980d12",
          "name": "listReceiptFilters",
          "request": {
            "url": "http://example.com/api/?Action=ListReceiptFilters?Filters.member.N=Filters.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the IP address filters associated with your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "725663de-2c7b-468a-afbe-2fe959fd0bd6"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Rules",
      "item": [
        {
          "id": "118a8956-0215-4048-8a0e-1668a5bd375a",
          "name": "createReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptRule?After=After&Rule=Rule&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15acf42d-1c86-4400-994b-cce85951b3f8"
            }
          ]
        },
        {
          "id": "ba855762-42ad-4153-9335-e9de21fa9cb3",
          "name": "deleteReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptRule?RuleName=RuleName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "740b0dc8-ebd4-489e-9226-f3b5e22d5db8"
            }
          ]
        },
        {
          "id": "e273a4b8-daee-432d-a712-0c1237b003f0",
          "name": "describeReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReceiptRule?RuleName=RuleName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c6e74fd-aed1-4537-83db-490eed686b1b"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "225e9d42-abc4-46df-89f6-976acba89bac",
          "name": "deleteIdentity",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentity?Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified identity (an email address or a domain) from the list of verified identities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fb949f9-186d-45f8-9771-29644a69802f"
            }
          ]
        },
        {
          "id": "2b9039ae-43be-4736-8e45-cec0580a4934",
          "name": "deleteIdentityPolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentityPolicy?Identity=Identity&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified sending authorization policy for the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e733f367-b41c-4a47-ad79-f45bafbb873a"
            }
          ]
        },
        {
          "id": "6d2b63a8-a999-4290-93ca-2a39a4c0025a",
          "name": "getIdentityDkimAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityDkimAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current status of Easy DKIM signing for an entity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d14c881e-9e26-403b-8094-ea76c86d2f83"
            }
          ]
        },
        {
          "id": "48731eed-dd71-49f7-ac4e-566218e96744",
          "name": "getIdentityMailFromDomainAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityMailFromDomainAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the custom MAIL FROM attributes for a list of identities (email addresses and/or domains)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b8e7bc6-9bcc-439b-bc9b-bd482f10416d"
            }
          ]
        },
        {
          "id": "4cc259d2-a0e7-4586-9c06-48c617022f21",
          "name": "getIdentityNotificationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityNotificationAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a list of verified identities (email addresses and/or domains), returns a structure describing identity notification attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0fdfee0-2432-4e8f-aaa9-56957c88d559"
            }
          ]
        },
        {
          "id": "bd1ebf3b-4fdf-4379-a01a-b0b7fb0b88f2",
          "name": "getIdentityPolicies",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityPolicies?Identity=Identity&PolicyNames.member.N=PolicyNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the requested sending authorization policies for the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a86d1c01-9416-467b-b84e-557a0c842996"
            }
          ]
        },
        {
          "id": "889ce090-4ab6-4cbc-813e-e62a2d8dd3d0",
          "name": "getIdentityVerificationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityVerificationAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a list of identities (email addresses and/or domains), returns the verification status and (for domain identities) the verification token for each identity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33f77901-1716-432b-b6ca-eb84c220c9a6"
            }
          ]
        },
        {
          "id": "d40082dc-a41a-4830-8e1a-fa3db7b6f2bb",
          "name": "listIdentities",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentities?IdentityType=IdentityType&MaxItems=MaxItems&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list containing all of the identities (email addresses and domains) for your AWS account, regardless of verification status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b5ad451-abc8-454f-8879-81ab8eb95b8b"
            }
          ]
        },
        {
          "id": "7adf3b07-573d-4a42-a1aa-a165fb6683fc",
          "name": "listIdentityPolicies",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentityPolicies?Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of sending authorization policies that are attached to the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69bc702b-e028-4b54-81b6-ad2b10da48f5"
            }
          ]
        },
        {
          "id": "20f21560-5a74-4d40-b77a-73344f67a233",
          "name": "putIdentityPolicy",
          "request": {
            "url": "http://example.com/api/?Action=PutIdentityPolicy?Identity=Identity&Policy=Policy&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or updates a sending authorization policy for the specified identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a0e9b32-ccfb-4da5-92b5-3b7d837dec7c"
            }
          ]
        },
        {
          "id": "60a94436-ccf1-4fb2-89b3-6bc9bfdcc943",
          "name": "setIdentityDkimEnabled",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityDkimEnabled?DkimEnabled=DkimEnabled&Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables or disables Easy DKIM signing of email sent from an identity:If Easy DKIM\n            signing is enabled for a domain name identity (e."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c72ae152-2db7-4e8c-baa2-17098252a3e6"
            }
          ]
        },
        {
          "id": "32fd3e03-667a-4443-a595-7bd81d5a04b1",
          "name": "setIdentityFeedbackForwardingEnabled",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityFeedbackForwardingEnabled?ForwardingEnabled=ForwardingEnabled&Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given an identity (an email address or a domain), enables or disables whether Amazon SES forwards bounce and complaint notifications as email."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27b689aa-a2b6-427d-930a-3f307b0f8b17"
            }
          ]
        },
        {
          "id": "f9b1e727-9f5e-4ba0-869a-90d106a78f14",
          "name": "setIdentityHeadersInNotificationsEnabled",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityHeadersInNotificationsEnabled?Enabled=Enabled&Identity=Identity&NotificationType=NotificationType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given an identity (an email address or a domain), sets whether Amazon SES includes \n            the original email headers in the Amazon Simple Notification Service (Amazon SNS) notifications \n            of a specified type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7235541-64cf-4404-b344-2ab49e77af00"
            }
          ]
        },
        {
          "id": "d5c7ac4d-6201-4fd7-8b1c-cf64aae07a4b",
          "name": "setIdentityMailFromDomain",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityMailFromDomain?BehaviorOnMXFailure=BehaviorOnMXFailure&Identity=Identity&MailFromDomain=MailFromDomain",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables or disables the custom MAIL FROM domain setup for a verified identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4236b325-76a4-440a-8f40-900cbfc84a79"
            }
          ]
        },
        {
          "id": "596c0e89-d057-4a9e-b780-4508d6880b05",
          "name": "setIdentityNotificationTopic",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityNotificationTopic?Identity=Identity&NotificationType=NotificationType&SnsTopic=SnsTopic",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given an identity (an email address or a domain), sets the Amazon Simple Notification Service (Amazon SNS) topic to which Amazon SES will publish\n        bounce, complaint, and/or delivery notifications for emails sent with that identity as the Source."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0f7d9a2-13cd-419d-b17c-a55a98445ef6"
            }
          ]
        }
      ]
    },
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "3fc403b8-bd5d-497c-9b2e-f926fbc2919c",
          "name": "deleteVerifiedEmailAddress",
          "request": {
            "url": "http://example.com/api/?Action=DeleteVerifiedEmailAddress?EmailAddress=EmailAddress",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified email address from the list of verified addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff257311-a241-46f7-95cd-5028f14a7677"
            }
          ]
        },
        {
          "id": "105cd421-30e0-4f92-9ff4-5d60814f8322",
          "name": "listVerifiedEmailAddresses",
          "request": {
            "url": "http://example.com/api/?Action=ListVerifiedEmailAddresses?VerifiedEmailAddresses.member.N=VerifiedEmailAddresses.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list containing all of the email addresses that have been verified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0fbccaa0-afab-4769-b53c-028d7929de6c"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Quota",
      "item": [
        {
          "id": "3323870d-ca5f-4887-a680-53b4e0dd8d46",
          "name": "getSendQuota",
          "request": {
            "url": "http://example.com/api/?Action=GetSendQuota?Max24HourSend=Max24HourSend&MaxSendRate=MaxSendRate&SentLast24Hours=SentLast24Hours",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the user's current sending limits."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04915fa2-e590-4055-930c-ef0703cb0258"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Statistics",
      "item": [
        {
          "id": "cf25f6ba-92c8-41e9-806b-73195a14ab7f",
          "name": "getSendStatistics",
          "request": {
            "url": "http://example.com/api/?Action=GetSendStatistics?SendDataPoints.member.N=SendDataPoints.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the user's sending statistics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91e2e5cb-5dc8-423d-8b1b-df37d1d954d3"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "9b7c31d4-f63d-4a08-98b1-789fade609a0",
          "name": "sendBounce",
          "request": {
            "url": "http://example.com/api/?Action=SendBounce?BouncedRecipientInfoList.member.N=BouncedRecipientInfoList.member.N&BounceSender=BounceSender&BounceSenderArn=BounceSenderArn&Explanation=Explanation&MessageDsn=MessageDsn&OriginalMessageId=OriginalMessageId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Generates and sends a bounce message to the sender of an email you received through Amazon SES."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2dba02c-8e14-4bb1-ad9b-48b66cb591b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Email",
      "item": [
        {
          "id": "500333c4-aadc-4149-82bb-bfc2e5bf492e",
          "name": "sendEmail",
          "request": {
            "url": "http://example.com/api/?Action=SendEmail?ConfigurationSetName=ConfigurationSetName&Destination=Destination&Message=Message&ReplyToAddresses.member.N=ReplyToAddresses.member.N&ReturnPath=ReturnPath&ReturnPathArn=ReturnPathArn&Source=Source&SourceArn=SourceArn&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Composes an email message based on input data, and then immediately queues the message for sending."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "251d483c-91a1-4920-aae9-91e3b8b72731"
            }
          ]
        },
        {
          "id": "45058620-2813-470b-99d7-f90c740e2714",
          "name": "sendRawEmail",
          "request": {
            "url": "http://example.com/api/?Action=SendRawEmail?ConfigurationSetName=ConfigurationSetName&Destinations.member.N=Destinations.member.N&FromArn=FromArn&RawMessage=RawMessage&ReturnPathArn=ReturnPathArn&Source=Source&SourceArn=SourceArn&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sends an email message, with header and content specified by the client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "088e4ed2-e7a5-46ca-8155-f3e102818549"
            }
          ]
        }
      ]
    }
  ]
}