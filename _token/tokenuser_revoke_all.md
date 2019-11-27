---
title: Revoke All Token
position: 4.3
type: post
description: /api/v1/api/v1/token/revoke_all_token/
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/api/v1/api/v1/token/revoke_all_token/',
        headers: {
            'Authorization':'Token $TOKEN',
        },
        method: 'POST',
        dataType: 'json',
        success: function(result){
          console.log(result);
        }
      });
    title: jQuery
    language: javascript
  - code_block: |-
      url = /api/v1/api/v1/token/revoke_all_token/
      headers = {"Authorization":"Bearer " + "YOUR_TOKEN_KEY","Content-Type":"application/json"}
      r = requests.post(url, headers = headers);
      print r.text
    title: Python
    language: python
---