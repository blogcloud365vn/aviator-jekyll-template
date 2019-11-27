---
title: Get List Token
possition: 4.1
type: get
description: /api/v1/api/v1/token/
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/api/v1/api/v1/token/',
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
      r = requests.get("/api/v1/api/v1/token/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      {
        "next": null,
        "previous": null,
        "count": 0,
        "page_num": 0,
        "page_size": 0,
        "results": [
            {
              "short_key": "string",
              "project_id": "string",
              "project_name": "string",
              "created": "2019-10-25T08:54:56.949917+07:00",
              "expired": "2019-10-25T10:32:44.799191+07:00",
              "real_ip": null,
              "browser_user_agent": null
            }
        ]
      }

    title: Response
    language: json
---