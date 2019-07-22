---
title: Server List
position: 2.1
type: get
description: /api/v1/server/

left_code_blocks:
  - code_block: |-
      $.ajax({
        url: 'http://localhost:8000/api/v1/accounts/',
        headers: {
            'Authorization':'Token $TOKEN',
        },
        method: 'GET',
        success: function(data){
          console.log(data);
        }
      });
    title: jQuery
    language: javascript
  - code_block: |-
      r = requests.get("/api/v1/server/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      {
        "count": 0,
        "next": "http://example.com",
        "previous": "http://example.com",
        "results": [
            {
              "instance_id": "string",
              "status": "string",
              "addresses": "string",
              "name": "string",
              "created": "2019-07-18T06:41:10Z",
              "expired": "2019-07-18T06:41:10Z",
              "ip_addresses": [
                "string"
              ],
              "region": "string"
            }
          ]
      }
    title: Response
    language: json
---