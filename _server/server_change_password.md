---
title: Server Change Password
position: 2.3
type: post
description: /api/v1/server/{instance_id}/change_password/
parameters:
  - name: password
    content: Password muốn thay đổi
  - name: re_password
    content: Nhập lại password muốn thay đổi
left_code_blocks:
  - code_block: |-
      $.ajax({
        url = /api/v1/server/{instance_id}/change_password/
        headers = {"Authorization":"Bearer " + $TOKEN,"Content-Type":"application/json"}
        data = {
          'password': "string",
          're_password': "string"
        }
        r = requests.post(url, headers = headers, data = data);
        print r.text
    title: jQuery
    language: javascript
  - code_block: |-
      $.ajax({
        url: '/api/v1/server/{instance_id}/change_password/',
        headers: {
            'Authorization':'Token $TOKEN',
        },
        method: 'POST',
        dataType: 'json',
        data: {
          "password": "string",
          "re_password": "string"
        },
        success: function(data){
          console.log(data);
        }
      });
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
        {
          "password": "string",
          "re_password": "string"
        }
    title: Request
    language: json
  - code_block: |-
      {
        "message": string
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





