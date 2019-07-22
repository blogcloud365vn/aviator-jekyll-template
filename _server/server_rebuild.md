---
title: Server Rebuild
position: 2.10
type: post
description: /server/{instance_id}/rebuild/
parameters:
  - name: os_image
    content: ID của hệ điều hành muốn thay đổi
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/server/{instance_id}/rebuild/',
        headers: {
            'Authorization':'Token $TOKEN',
        },
        data: {
          'os_image': 0
        }
        method: 'POST',
        dataType: 'json',
        success: function(data){
          console.log(data);
        }
      });
    title: jQuery
    language: javascript
  - code_block: |-
      url = /server/{instance_id}/rebuild/
      headers = {"Authorization":"Bearer " + $TOKEN,"Content-Type":"application/json"}
      data = {
        'os_image': 0
      }
      r = requests.post(url, headers = headers, data = data);
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
        {
          "os_image": 0
        }
    title: Request
    language: json
  - code_block: |-
      {
        "message": "string"
      }
    title: Response
    language: json
  - code_block: |-
      {
        "error": true,
        "message": "string"
      }
    title: Error
    language: json
---
