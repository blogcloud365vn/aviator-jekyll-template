---
title: Revoke Token
position: 4.2
type: post
description: /api/v1/api/v1/token/revoke_token/
parameters:
  - name: token_key
    content: Nhập token key để xác định token muốn xóa
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/api/v1/api/v1/token/revoke_token/',
        headers: {
            'Authorization':'Token $TOKEN',
        },
        data: {
          'token_key': "string"
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
      url = /api/v1/api/v1/token/revoke_token/
      headers = {"Authorization":"Bearer " + "YOUR_TOKEN_KEY","Content-Type":"application/json"}
      data = {
        'token_key': "string",
      }
      r = requests.post(url, headers = headers, data = data);
      print r.text
    title: Python
    language: python
---