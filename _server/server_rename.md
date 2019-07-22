---
title: Server Rename
position: 2.9
type: post
description: /server/{instance_id}/rename/
parameters:
  - name: server_name
    content: Tên máy chủ ảo muốn thay đổi
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/server/{instance_id}/rename/',
        headers: {
            'Authorization':'Token $TOKEN',
        },
        data: {
          'server_name': "string"
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
      url = /server/{instance_id}/rename/
      headers = {"Authorization":"Bearer " + "YOUR_TOKEN_KEY","Content-Type":"application/json"}
      data = {
        'server_name': "string"
      }
      r = requests.post(url, headers = headers, data = data);
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
        {
          "server_name": "string"
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
