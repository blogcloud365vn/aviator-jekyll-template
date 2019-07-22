---
title: /user
position: 3.4
type: get
description: Hiển thị thông tin cá nhân của user
left_code_blocks:
  - code_block: |-
      r = requests.get("http://portalurl/api/v1/user/list_project/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      {
        "is_available": true,
        "project": "string",
        "project_user_name": "string"
      }

    title: Response
    language: json
---