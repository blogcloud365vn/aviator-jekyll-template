---
title: User Detail
position: 3.1
type: get
description: /user/detail_user/
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/user/detail_user/',
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
      r = requests.get("/user/detail_user/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      {
        "address": "string",
        "birthday": "YYYY-MM-DD",
        "company": "string",
        "date_joined": "YYYY-MM-DDTh:i:s+07:00",
        "email": "user@example.com",
        "first_name": "string",
        "gender": "gender",
        "last_login": "YYYY-MM-DDTh:i:s+07:00",
        "last_name": "string",
        "phone_number": "00000000"
      }

    title: Response
    language: json
---