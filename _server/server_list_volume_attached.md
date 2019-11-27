---
title: Server List Volume Attached
position: 2.13
type: get
description: /api/v1/server/{instance_id}/list_volume_attached/
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/api/v1/server/{instance_id}/list_volume_attached/',
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
      r = requests.get("/api/v1/server/{instance_id}/list_volume_attached/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      [
        {
          "name": "string",
          "volume_id": "string",
          "bootable": false,
          "size": 0000000
        }
      ]

    title: Response
    language: json
---