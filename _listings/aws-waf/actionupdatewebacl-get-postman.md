{
  "info": {
    "name": "AWS WAF API Update Web ACL",
    "_postman_id": "eea29fd9-bb62-4ca8-a7bf-5910f6dd1a6a",
    "description": "Service: AWS WAFInserts or deletes.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Web ACL",
      "item": [
        {
          "id": "ae16c63a-63a8-49eb-af47-cd42acf5e3a5",
          "name": "associateWebACL",
          "request": {
            "url": "http://example.com/api/?Action=AssociateWebACL?ResourceArn=ResourceArn&WebACLId=WebACLId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAF RegionalAssociates a web ACL with a resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "794fea79-ba6b-4059-90da-43dbdb54deac"
            }
          ]
        },
        {
          "id": "9ed17a4a-0176-419d-8ecb-082a306f1651",
          "name": "createWebACL",
          "request": {
            "url": "http://example.com/api/?Action=CreateWebACL?ChangeToken=ChangeToken&DefaultAction=DefaultAction&MetricName=MetricName&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates a WebACL, which contains the Rules that identify the CloudFront web requests that you want to allow, block, or count."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0667f78a-2cc8-4d98-abbf-6adbe1a7d591"
            }
          ]
        },
        {
          "id": "fa0b3591-0b32-4ca7-b066-f0399086d1b2",
          "name": "deleteWebACL",
          "request": {
            "url": "http://example.com/api/?Action=DeleteWebACL?ChangeToken=ChangeToken&WebACLId=WebACLId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes a."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f41666b-995c-4e94-91b3-98863679f040"
            }
          ]
        },
        {
          "id": "03c2300c-7b74-4109-b10c-8f8048fd07a5",
          "name": "disassociateWebACL",
          "request": {
            "url": "http://example.com/api/?Action=DisassociateWebACL?ResourceArn=ResourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAF RegionalRemoves a web ACL from the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30874f82-42f5-4e00-8132-d71b076aba63"
            }
          ]
        },
        {
          "id": "16add93c-f4da-4ebb-b7db-c96b3dc21f86",
          "name": "getWebACL",
          "request": {
            "url": "http://example.com/api/?Action=GetWebACL?WebACLId=WebACLId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5c72fe3-a308-4800-a38e-6bd65778e9c4"
            }
          ]
        },
        {
          "id": "c6a8a810-5f14-44cd-986d-cad7a693d3e6",
          "name": "getWebACLForResource",
          "request": {
            "url": "http://example.com/api/?Action=GetWebACLForResource?ResourceArn=ResourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAF RegionalReturns the web ACL for the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3081b3ba-f755-4b93-98a9-592251c67138"
            }
          ]
        },
        {
          "id": "f1d49552-edc6-4dc3-9e75-d886b00e7d73",
          "name": "listResourcesForWebACL",
          "request": {
            "url": "http://example.com/api/?Action=ListResourcesForWebACL?WebACLId=WebACLId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAF RegionalReturns an array of resources associated with the specified web ACL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e395308b-ca5e-4bcf-bfcf-eead6540f2e8"
            }
          ]
        },
        {
          "id": "60a075f3-495f-452b-b48e-3b9ba6b0256d",
          "name": "listWebACLs",
          "request": {
            "url": "http://example.com/api/?Action=ListWebACLs?Limit=Limit&NextMarker=NextMarker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns an array of."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a6e22ed-7731-4f9e-b2ae-4cc75af0f47f"
            }
          ]
        },
        {
          "id": "0af395e7-3556-4526-983f-a28d6160022d",
          "name": "updateWebACL",
          "request": {
            "url": "http://example.com/api/?Action=UpdateWebACL?ChangeToken=ChangeToken&DefaultAction=DefaultAction&Updates=Updates&WebACLId=WebACLId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFInserts or deletes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f74e88c1-4c58-4d43-9679-eb1e0d40dfe7"
            }
          ]
        }
      ]
    },
    {
      "name": "Byte Match Set",
      "item": [
        {
          "id": "02deebe5-b082-4184-acef-1a7967ce96e9",
          "name": "createByteMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateByteMatchSet?ChangeToken=ChangeToken&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates a ByteMatchSet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e8a7dd6-9093-449e-8b61-bd9360a21fa5"
            }
          ]
        },
        {
          "id": "a57704b5-b3d5-4f8e-b4c5-ea50b6e50733",
          "name": "deleteByteMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteByteMatchSet?ByteMatchSetId=ByteMatchSetId&ChangeToken=ChangeToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes a."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcbc0941-d290-4948-954f-a75f83d0b5cb"
            }
          ]
        },
        {
          "id": "4208a4c9-b626-4a76-957f-edc4b241079b",
          "name": "getByteMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=GetByteMatchSet?ByteMatchSetId=ByteMatchSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f496500-70f1-4645-8cc7-9937fae13004"
            }
          ]
        },
        {
          "id": "e4e9a3aa-ebb0-4b7f-a862-b03e430f6706",
          "name": "updateByteMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=UpdateByteMatchSet?ByteMatchSetId=ByteMatchSetId&ChangeToken=ChangeToken&Updates=Updates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFInserts or deletes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c51e683b-e4ad-4591-a615-f9539989e40b"
            }
          ]
        }
      ]
    },
    {
      "name": "IP Sets",
      "item": [
        {
          "id": "a0d7cadb-b1df-43ac-afa5-4b9611a9b847",
          "name": "createIPSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateIPSet?ChangeToken=ChangeToken&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates an."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d56a246b-da5f-4330-83ca-26bd5612654a"
            }
          ]
        },
        {
          "id": "64ed1460-173f-4be9-9694-8bbd448144d1",
          "name": "deleteIPSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIPSet?ChangeToken=ChangeToken&IPSetId=IPSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes an."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60150b29-deb8-4ec4-9e8c-0e4790fe4032"
            }
          ]
        },
        {
          "id": "e7a6a379-47e5-4bbc-9de5-cfd214a3897d",
          "name": "getIPSet",
          "request": {
            "url": "http://example.com/api/?Action=GetIPSet?IPSetId=IPSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4876c036-e336-420d-92df-f89bc043d258"
            }
          ]
        },
        {
          "id": "032f2c79-e892-400f-a610-0f06e0c187fd",
          "name": "listIPSets",
          "request": {
            "url": "http://example.com/api/?Action=ListIPSets?Limit=Limit&NextMarker=NextMarker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns an array of."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1751a006-2805-4428-89b1-b1ef90072f33"
            }
          ]
        },
        {
          "id": "809247a8-4210-435b-8be2-798fc864528d",
          "name": "updateIPSet",
          "request": {
            "url": "http://example.com/api/?Action=UpdateIPSet?ChangeToken=ChangeToken&IPSetId=IPSetId&Updates=Updates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFInserts or deletes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e3a2ca6-391a-405b-b32b-87b935551d2a"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules",
      "item": [
        {
          "id": "f5645a4e-e200-4624-8db4-0974f7009827",
          "name": "createRule",
          "request": {
            "url": "http://example.com/api/?Action=CreateRule?ChangeToken=ChangeToken&MetricName=MetricName&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates a Rule, which contains the IPSet objects, ByteMatchSet objects, and \n\t\t\tother predicates that identify the requests that you want to block."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e61df6cb-8915-4809-84c0-19ccaa6b5caf"
            }
          ]
        },
        {
          "id": "ce4fcbd2-092f-4086-84f1-b0113d2ac6cf",
          "name": "deleteRule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRule?ChangeToken=ChangeToken&RuleId=RuleId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes a."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09ee682f-67d8-48e0-ba50-1b1b215ca814"
            }
          ]
        },
        {
          "id": "f79ffdfc-a495-4cfb-86d5-14b2feee325b",
          "name": "getRule",
          "request": {
            "url": "http://example.com/api/?Action=GetRule?RuleId=RuleId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e2026ae-2925-478d-89c2-6ad684d00b82"
            }
          ]
        },
        {
          "id": "f1b418e9-5f09-4223-9d36-07bc285179ce",
          "name": "listRules",
          "request": {
            "url": "http://example.com/api/?Action=ListRules?Limit=Limit&NextMarker=NextMarker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns an array of."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bdc8488-d228-4aba-8d08-fc5f6ad3008c"
            }
          ]
        },
        {
          "id": "70ec9088-362d-4ee1-94bb-f2e4e956685c",
          "name": "updateRule",
          "request": {
            "url": "http://example.com/api/?Action=UpdateRule?ChangeToken=ChangeToken&RuleId=RuleId&Updates=Updates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFInserts or deletes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "122ade41-c235-4bc9-b822-68218f7ba0fd"
            }
          ]
        }
      ]
    },
    {
      "name": "Size Constraint Set",
      "item": [
        {
          "id": "305117c0-4b90-4a4e-8074-09f84a708d19",
          "name": "createSizeConstraintSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateSizeConstraintSet?ChangeToken=ChangeToken&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates a SizeConstraintSet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ad3e6fa-64a7-4618-a38d-d2c3dd796c50"
            }
          ]
        },
        {
          "id": "6fd3c2b3-c50e-442c-852f-35cd3b3f41c5",
          "name": "deleteSizeConstraintSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSizeConstraintSet?ChangeToken=ChangeToken&SizeConstraintSetId=SizeConstraintSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes a."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf1dfada-9ade-4df6-91b9-c229f4e251a9"
            }
          ]
        },
        {
          "id": "53d4a11e-dbdd-4240-903e-7b4010ad8c18",
          "name": "getSizeConstraintSet",
          "request": {
            "url": "http://example.com/api/?Action=GetSizeConstraintSet?SizeConstraintSetId=SizeConstraintSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ad48007-27d1-413f-ae85-bbcd8e9b381f"
            }
          ]
        },
        {
          "id": "a4961343-b29f-4994-ba33-0bb32ed4f939",
          "name": "updateSizeConstraintSet",
          "request": {
            "url": "http://example.com/api/?Action=UpdateSizeConstraintSet?ChangeToken=ChangeToken&SizeConstraintSetId=SizeConstraintSetId&Updates=Updates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFInserts or deletes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ca40b75-e2fd-404c-b0d5-3c89fa1cc9bc"
            }
          ]
        }
      ]
    },
    {
      "name": "SQL Injection Match Set",
      "item": [
        {
          "id": "e3cc811e-38a9-42c5-9421-5e66a63e191a",
          "name": "createSqlInjectionMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateSqlInjectionMatchSet?ChangeToken=ChangeToken&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates a."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a78bfdb9-4c5b-4152-a780-685e8337bd3a"
            }
          ]
        },
        {
          "id": "00cb461d-eb47-423a-aa54-f429c73a2029",
          "name": "deleteSqlInjectionMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSqlInjectionMatchSet?ChangeToken=ChangeToken&SqlInjectionMatchSetId=SqlInjectionMatchSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes a."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3bdf559b-c826-4b66-835a-10c18ff6eb86"
            }
          ]
        },
        {
          "id": "63e2964a-bb5b-4e64-96b1-4dff8deae0e8",
          "name": "getSqlInjectionMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=GetSqlInjectionMatchSet?SqlInjectionMatchSetId=SqlInjectionMatchSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d67b0fe-581b-45b2-85ad-347f6df7c626"
            }
          ]
        }
      ]
    },
    {
      "name": "XSS Match Set",
      "item": [
        {
          "id": "924f3004-698f-4286-81ca-48bdb0c7097a",
          "name": "createXssMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateXssMatchSet?ChangeToken=ChangeToken&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFCreates an."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3de6bef3-e0cf-4d97-9e4b-d42b4910694b"
            }
          ]
        },
        {
          "id": "4d785566-51f5-4d0f-8808-8cf7697c91b2",
          "name": "deleteXssMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteXssMatchSet?ChangeToken=ChangeToken&XssMatchSetId=XssMatchSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFPermanently deletes an."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "966cac0d-ef88-4b0c-84b7-79748192e610"
            }
          ]
        },
        {
          "id": "04c599ca-4f39-4be1-9184-5bea4249384f",
          "name": "getXssMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=GetXssMatchSet?XssMatchSetId=XssMatchSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9891725f-2428-4cc7-957f-dc95d1d04ce8"
            }
          ]
        },
        {
          "id": "8737a977-4dea-49ba-b8a1-c24b92f17239",
          "name": "listXssMatchSets",
          "request": {
            "url": "http://example.com/api/?Action=ListXssMatchSets?Limit=Limit&NextMarker=NextMarker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns an array of."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "887d8ced-8240-45d4-8ae6-7ff73f77dffe"
            }
          ]
        }
      ]
    },
    {
      "name": "Change Token",
      "item": [
        {
          "id": "20e8c80d-f763-48ae-8f06-ea8cd6b0bb90",
          "name": "getChangeToken",
          "request": {
            "url": "http://example.com/api/?Action=GetChangeToken?ChangeToken=ChangeToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFWhen you want to create, update, or delete AWS WAF objects, get a change token and include the change token in the create, update, or delete request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66417fe2-3ccf-42cf-a927-44022480824d"
            }
          ]
        },
        {
          "id": "2dad17b6-0102-479d-9c14-48a0e7974053",
          "name": "getChangeTokenStatus",
          "request": {
            "url": "http://example.com/api/?Action=GetChangeTokenStatus?ChangeToken=ChangeToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns the status of a ChangeToken that you got by calling."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4f6cb57-0703-48af-a39a-4166d2061362"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "71216465-16bf-4d02-9246-636e4ef8924c",
          "name": "getSampledRequests",
          "request": {
            "url": "http://example.com/api/?Action=GetSampledRequests?MaxItems=MaxItems&RuleId=RuleId&TimeWindow=TimeWindow&WebAclId=WebAclId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFGets detailed information about a specified number of requests--a sample--that AWS WAF randomly selects from among the first 5,000 requests that your AWS resource received during a time range that you choose."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5382ea08-752d-4b05-8e6a-e152c08a4e91"
            }
          ]
        }
      ]
    },
    {
      "name": "Byte Match Sets",
      "item": [
        {
          "id": "99a600b7-8a62-4c6c-8159-af03a31520c3",
          "name": "listByteMatchSets",
          "request": {
            "url": "http://example.com/api/?Action=ListByteMatchSets?Limit=Limit&NextMarker=NextMarker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns an array of."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a907008-af27-46ad-b827-1c9c9a7fdf67"
            }
          ]
        }
      ]
    },
    {
      "name": "Size Constraint Sets",
      "item": [
        {
          "id": "d05533ec-e66a-430c-9642-befc180aaf4c",
          "name": "listSizeConstraintSets",
          "request": {
            "url": "http://example.com/api/?Action=ListSizeConstraintSets?Limit=Limit&NextMarker=NextMarker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns an array of."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e09a8c93-a786-463a-89f2-2d1d10dfc517"
            }
          ]
        }
      ]
    },
    {
      "name": "SQL Injection Match Sets",
      "item": [
        {
          "id": "da6b0b49-4061-4955-ba6e-8049de8a1ea2",
          "name": "listSqlInjectionMatchSets",
          "request": {
            "url": "http://example.com/api/?Action=ListSqlInjectionMatchSets?Limit=Limit&NextMarker=NextMarker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFReturns an array of."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2056c474-e258-487c-b85b-976f1fef5f52"
            }
          ]
        },
        {
          "id": "ca2f586f-34cd-4e56-aca5-ca2257009c3a",
          "name": "updateSqlInjectionMatchSet",
          "request": {
            "url": "http://example.com/api/?Action=UpdateSqlInjectionMatchSet?ChangeToken=ChangeToken&SqlInjectionMatchSetId=SqlInjectionMatchSetId&Updates=Updates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Service: AWS WAFInserts or deletes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1da98099-685f-4ee2-8cdb-46bc2cb119e6"
            }
          ]
        }
      ]
    }
  ]
}