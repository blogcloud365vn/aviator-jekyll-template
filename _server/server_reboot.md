---
title: Server Reboot
position: 2.6
type: post
description: /api/v1/server/{instance_id}/reboot/
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/api/v1/server/{instance_id}/reboot/',
        headers: {
            'Authorization':'Token $TOKEN',
        },
        method: 'POST',
        dataType: 'json',
        success: function(data){
          console.log(data);
        }
      });
    title: jQuery
    language: javascript
  - code_block: |-
      r = requests.get("/api/v1/server/{instance_id}/reboot/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      {
        "message": "string"
      }

    title: Response
    language: json
---