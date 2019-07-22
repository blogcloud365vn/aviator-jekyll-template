---
title: User Change Password
position: 3.3
type: post
description: /user/change_password/
parameters:
  - name: old_password
    content: Mật khẩu cũ
  - name: new_password
    content: Mật khẩu mới muốn thay đổi
  - name: re_password
    content: Nhập lại mật khẩu muốn thay đổi
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/user/change_password/',
        headers: {
            'Authorization':'Token $TOKEN',
        },
        data: {
          'old_password': "string",
          'new_password': "string",
          're_password': "string"
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
      url = /user/change_password/
      headers = {"Authorization":"Bearer " + "YOUR_TOKEN_KEY","Content-Type":"application/json"}
      data = {
        'old_password': "string",
        'new_password': "string",
        're_password': "string"
      }
      r = requests.post(url, headers = headers, data = data);
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
        {
          "old_password": "string",
          "new_password": "string",
          "re_password": "string"
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





