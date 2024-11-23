{
  "type": "ParseJson",
  "inputs": {
    "content": "@variables('GroupArray')",
    "schema": {
      "type": "array",
      "items": {
        "type": "object",
        "properties": {
          "value": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {
                "id": {},
                "createdDateTime": {},
                "description": {},
                "displayName": {},
                "mail": {},
                "mailEnabled": {},
                "mailNickname": {},
                "securityEnabled": {}
              },
              "required": [
                "id"
              ]
            }
          }
        },
        "required": [
          "value"
        ]
      }
    }
  },
  "runAfter": {
    "Select": [
      "TIMEDOUT"
    ]
  },
  "metadata": {
    "operationMetadataId": "6b201c7f-1b2a-4f7a-953f-0893e1a138b7"
  }
}
