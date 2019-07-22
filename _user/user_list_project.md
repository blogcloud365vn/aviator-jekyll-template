---
title: User List Project
position: 3.4
type: get
description: /api/v1/user/list_project/
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/api/v1/user/list_project/',
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
      r = requests.get("/api/v1/user/list_project/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      {
        "is_available": true,
        "project": "string",
        "project_user_name": "string"
      }

    title: Response
    language: json
---