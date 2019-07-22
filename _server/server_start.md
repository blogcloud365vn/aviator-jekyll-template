---
title: Server Start
position: 2.7
type: post
description: /server/{instance_id}/start/
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/server/{instance_id}/start/',
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
      r = requests.get("/server/{instance_id}/start/", token="YOUR_TOKEN_KEY")
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