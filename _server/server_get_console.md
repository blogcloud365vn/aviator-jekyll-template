---
title: Server Console
position: 2.4
type: get
description: /api/v1/server/{instance_id}/console/

left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/api/v1/server/{instance_id}/console/',
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
      r = requests.get("/api/v1/server/{instance_id}/console/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      {
        "message": "string",
        "url": "example.com"
      }

    title: Response
    language: json
---