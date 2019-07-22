---
title: User Update
position: 3.2
type: patch
description: /user/update_profile/
parameters:
  - name: first_name
    content: Họ và tên đệm
  - name: last_name
    content: Tên thật
  - name: gender
    content: Giới tính, 1 => Nam, 2 => Nữ, 3=> Cônng ty
  - name: phone_number
    content: Số điện thoại của người sở hữu
  - name: address
    content: Địa chỉ
  - name: company
    content: Tên công ty
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/user/update_profile/',
        headers: {
            'Authorization':'Token $TOKEN',
        },
        data: {
          'first_name': "string",
          'last_name': "string",
          'gender': 0,
          'phone_number': "string",
          'address': "string",
          'company': "string"
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
      url = /user/update_profile/
      headers = {"Authorization":"Bearer " + "YOUR_TOKEN_KEY","Content-Type":"application/json"}
      data = {
        'first_name': "string",
        'last_name': "string",
        'gender': 0,
        'phone_number': "string",
        'address': "string",
        'company': "string"
      }
      r = requests.post(url, headers = headers, data = data);
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
        {
          "first_name": "string",
          "last_name": "string",
          "gender": 0,
          "phone_number": "string",
          "address": "string",
          "company": "string"
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





