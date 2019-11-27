---
title: Server Get Action Log
position: 2.11
type: get
description: /api/v1/server/{instance_id}/get_action_log/
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/api/v1/server/{instance_id}/get_action_log/',
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
      r = requests.get("/api/v1/server/{instance_id}/get_action_log/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      [
        {
          "instance_uuid": "string",
          "user_id": "string",
          "start_time": "string",
          "action": "string",
          "message": "string",
          "project_id": "string"
        }
      ]
      

    title: Response
    language: json
---