---
title: Token Detail
position: 1.2
type: get
description: /api/v1/auth/tokens

left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/api/v1/auth/tokens',
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
      r = requests.get("/api/v1/auth/tokens", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      {
        "project_id": string,
        "token_created": "YYYY-MM-DDTh:i:s+07:00",
        "token_expired": "YYYY-MM-DDTh:i:s+07:00",
        "token_key": "user@example.com"
      }
    title: Response
    language: json
---