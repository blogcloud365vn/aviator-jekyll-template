---
title: /server
position: 4.5
type: get
description: Lấy thông tin console log
left_code_blocks:
  - code_block: |-
      r = requests.get("http://portalurl/api/v1/server/{instance_id}/get_console_log/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      {
        "console_log": "string"
      }

    title: Response
    language: json
---